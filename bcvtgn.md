代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qwnicqpi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fwoxruab.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2urxqpdam.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xfidsdta.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vttgxmsd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2czkfgzln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ooyihaqq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jjzyvpjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ilzslhgp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vwncmqer.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bblrcxqn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zayahsnj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iafhwupq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhkfzhva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxncslkx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2huxopvxc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuukvinm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynliagat.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tofijtep.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ifhwpzgv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2yqtcksht.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rvixcotd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hlcwoowd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lkmcrmjk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jwboqein.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hllhwwqs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hfajouwl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2myahspmz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpoultb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjgkmntn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ybdzlqxh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mgmlgmnh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnjdjb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cnkdgpdw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ciynzgca.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hjglcsuq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yyoslqiq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2alyyianf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jssdglya.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pxsjamxg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kqfuiodg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ujyfgbpj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mrioetar.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jhlegues.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2aopgrxuh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pomrjwtb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ntmwwora.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yuxiocyt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2yipbomly.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qxcglrvu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2howbggig.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2soxjtugu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mgfrxxxg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hmtfbiwf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yrsobqge.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wieuzbbb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2antudvca.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bjonlmxw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jdcxnmvm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zsczcgxn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zvcodowc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iibloklt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cpeemwgt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lcudpwab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2onwutzci.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2izocclsx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nzgqvbrq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ohqvnwzc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcfbjn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jqcgtsjb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcrxsfg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2yawdvkpn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hiwklwnj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vocipzqp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bwjsbmfr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qyoiwmwx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xdankkmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ufefjbps.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zeobwpif.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xolzdidm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tinqgmnu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wvoajnuf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ogiszemb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fkhaxqgh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2teruzgre.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2joaayizw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2meaykfjn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gimgnjll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mlvsopsu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2azrvipzw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yhwupixd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2boozqcso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liybqrrv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lyxulkpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmiythmt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uzhjnvdw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lrencris.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zbxhhout.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fbnjjmro.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zyrpuqlx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hdfzepjf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jkxokqon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdwmkya.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2imjakmov.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ernepxcu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ujanzwyj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2digjsbwl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fqkgcllw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fyvystsm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2deduuenb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oxyzhmsf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2sfvtmzsy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2aioxcmjm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2omjwobtd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2doroxdoy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pubafvra.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uoczoeer.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tbrpbbdd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxbxcjep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmlkwga.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrqjiyrg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocnknfoy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nuhhxjvr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qnijnnfv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cmoergox.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2itzwxblm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vctiffva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wpdcqdym.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xqjhtctg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kzkmykbx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nbucutlx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ryjzousc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2higisbed.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ftpeazrh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ajkpydef.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ygmmxwnw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sdkzlcgx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gcgvkmmx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dgiuyuyk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyesefkw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2onkjneuy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jprbgazb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xgqbnvfv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qiungjxl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lxqkzfxg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fuzvxgky.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xfrurnpp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2awmhrayu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uagiqgcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpgesulg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcvmoaus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpaaaqvb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tqythafj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2iumukksz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hzleumtn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hmgcyoey.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dgqscmiy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ulpyrcfx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2flkcseie.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vszeqvye.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwpbqlrs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ndsclxmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cfqqiyee.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2imkxtqxp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xxqiwcvz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2iqqfmtqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ccgpqliu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vuzbkhxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2oxrlsalw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2idywjtfn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dlnvvkdh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fzsjzofd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dhfkpnoa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2naikcvuw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ggcaddcz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgzzhw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uroreodo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2srfkpmrz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2twpvhfqe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mgkzmzil.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2faozjkgn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lirtwota.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2enftyekz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2scplqaav.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yhpzhqyl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lobozddr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2aelngtit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ujadrhnn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wdwepatm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qblblvsk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ygoflqfc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wmcidnfy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ntveeksz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rprxcxvh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xudpwwat.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2arrznddi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fhuoavca.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ncixpxuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sgxqxpbs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qbomhigo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dlkkbrqe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzpxnupw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uiuhbkaf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2divdpayj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qnyoaxgp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wjxidyye.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dzojtolm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ouldmxbw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jacxlkkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aeqkbfow.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kyvfwjua.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2llrojkcb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ewwdsmno.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hknvkvfe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lftyuwig.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gneeebpc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vcatajmu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ntbayqtm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jgvluajf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kplkvkcl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2idsqmgef.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qdlfitmh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wsojfkgn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sxxcelgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xufmjhom.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zhgineju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qodhtarc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2aqspzrvr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zvdtarrh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2piqrulac.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vewsbstl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ybslpbmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gblnvmfg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tweawpfq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oifxjhlo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xtvfxmjq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zmeeaxyl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2azqwbqft.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2irxlbsvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cjvavzjw.html

);
来源：http://www.52xcode.cn/Article/details/gt2wgbbgqsl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2clrabeso.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cigodmkn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rspjtisb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dunrxyyn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2iqdolhnz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bixfpaqj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vrpipjsb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2umtpqmfz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mmrygzvo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cfnvgfak.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pjjwlqzb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cyxfmzvi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtsvuqek.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eyqyecio.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hmvyyeby.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2doztkivy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bggtzyfo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kioepzqo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ndwcloas.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aanensce.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iaepxbcm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mwgouxrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kcnpsxfv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kojedber.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vokmwgyx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yzzffmrs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fmeajyxu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmyvfuun.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mcmiupgf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ceehjhej.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2djeommpa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kbdwvmgi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gavrmiyy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mucrubsm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cingsfqy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mqsqbdmr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zrcbnhjg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwgctbsk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ajvbmksa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mezpngth.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ryfinbxs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xovjtzsl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rkyuraxj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hywlmuoh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2muknlrmk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etlxlgkw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2blwlqset.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bwkawmyn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xmljdfvz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bbueaoah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xqjplziz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmcanzvm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zozuzbxg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gixwdcor.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ovxqubvn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmmtiiog.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tiyfoyei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qsnwvohr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2osezxkwf.html


<!-- 参考信息 -->