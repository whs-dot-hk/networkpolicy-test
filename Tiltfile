def create_namespace(name):
    k8s_yaml(blob("""apiVersion: v1
kind: Namespace
metadata:
  name: %s
""" % name))

create_namespace("test")

k8s_yaml(["nginx.yaml", "busybox.yaml", "nc.yaml"])
