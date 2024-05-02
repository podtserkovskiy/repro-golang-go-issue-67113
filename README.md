# repro-golang-go-issue-67113
Repro cmd:
```bash
CGO_ENABLED=0 GO111MODULE=off GOARCH=amd64 GOEXPERIMENT=nocoverageredesign GOOS=darwin go list -e '-json=GoFiles,CgoFiles,HFiles,CFiles,CXXFiles,SFiles,EmbedFiles,CgoCFLAGS,CgoCPPFLAGS' -tags .
```
