### My Private Thought

``` c
struct Offering {
  void *doc;
  void *code;
  void *paper;
  void *video;
  void *ppt;
  void *question;
};

Project * getExcellentOpenSource(CodeWorld *w) {
  Project *p = top(w.star && w.fork);
  if (NULL! = p) return p;
  
  if (your.interest) {
    if (email("wangbojing@0voice.com") || submit(issue)) {
      return getYourExcellentOpenSource();
    }
  }
}

struct Offering * produce(Project *p) {

  Offering *o = malloc(sizeof(struct Offering));
  o->doc = arrangeDocument(p);
  o->code = produceExampleCode(p);
  o->video = produceVideo(p);
  o->paper = arrangePaper(p);
  o->ppt = arrangePPTpdf(p);
  o->question = arrangeQuestionList(p);
  
  return o;
}

void produceRepo(struct Offering *o) {
  setRepoOrg0voice(o); // https://github.com/0voice
  free(o);
}

int main() {
  CodeWorld world;  // network, OS, stroage, SDN, virtual, kernel, RISC-V, etc. (code with c/c++)
  while(1) {
      Project *p = getExcellentOpenSource(world);
      //Project: dpdk, rocksdb, spdk, vpp, ovs, userstack, coroutine, virtio, nginx, redis, zmq, bpf/ebpf, io_uring, etc.
      
      struct Offering *o = produce(p);
      produceRepo(o);
      sleep(1); // 2 * 7 * 24 * 60 * 60s, 2 weeks
  }
}
```

