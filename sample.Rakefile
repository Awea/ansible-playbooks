task :test  do
  system %{
    source ~/.zshrc
    vre
  }
  system "ssh-copy-id vagrant@192.168.0.22"
  system "ansible-playbook site.yml -vvv"
end