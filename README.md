[Unit]
Description=Prometheus Service
After=network.target

[Service]
Type=simple
ExceStart=/usr/local/bin/prometheus/prometheus --config.file=/usr/local/bin/prometheus/prometheus.yml

[Install]
WantedBy=multi.user.target
