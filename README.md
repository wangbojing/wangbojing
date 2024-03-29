### My Working Thought

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
  
  if (your.interest) {
    if (email("zvoice.king@gmail.com") || submit(issue)) {
      return getYourExcellentOpenSource();
    }
  }
  return top(w->star) == NULL ? top(w->fork) : top(w->star);
}

struct Offering * produce(Project *p) {

  Offering *o = malloc(sizeof(struct Offering));
  o->doc = arrangeDocument(p);
  o->code = produceExampleCode(p);
  o->video = produceVideo(p);
  o->paper = arrangePaper(p); //https://www.usenix.org/
  o->ppt = arrangePPTpdf(p);
  o->question = arrangeQuestionList(p);
  
  return o;
}

void produceRepo(struct Offering *o) {
  setRepoOrg0voice(o); // https://github.com/0voice
  free(o);
}

int main() {
  CodeWorld world;  // network, OS, storage, SDN, virtual, kernel, RISC-V, etc. (code with c/c++)
  
#pragma omp parallel num_threads(worker_nums)  
  {
    while(1) {
      Project *p = getExcellentOpenSource(world);
      //Project: dpdk, rocksdb, spdk, vpp, ovs, userstack, coroutine, virtio, nginx, redis, zmq, bpf/ebpf, io_uring, etc.

      struct Offering *o = produce(p);
      produceRepo(o);
    }
  }
}
```

