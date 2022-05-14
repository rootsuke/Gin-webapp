FROM golang:1.18

WORKDIR /workspace
ADD . .

RUN go install golang.org/x/tools/gopls@latest && \
  go install github.com/go-delve/delve/cmd/dlv@latest && \
  go install github.com/fatih/gomodifytags@latest && \
  go install github.com/josharian/impl@latest && \
  go install github.com/cweill/gotests/...@latest && \
  go install honnef.co/go/tools/cmd/staticcheck@latest
