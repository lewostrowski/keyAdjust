mkdir /usr/local/sbin/keyAdjustScrpit; 
touch keyAdjust.service
cp [script]
cd /etc/systemd/system/
ln -s /usr/local/sbin/keyAdjust.service keyAdjust.service

systemctl start keyAdjust.service
systemctl enable keyAdjust.service