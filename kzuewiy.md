代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gguyshzlx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gkpzgqjlt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ghwblhska.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gxehkyrbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/guzjlvmsq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gtsdzekrt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gzpdcpdmb.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gpcdweqvo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gnaiugaev.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gunzwaock.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gorgixmjh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmevnxmdx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gdbubxgxm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/ghjlcgvjb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggwyxniga.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gogbeibcg.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gckwhzkcy.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gxefryomo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtptuepm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/golmuhzkq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gyjvttepc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gdkxgdxyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/guihuheqm.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gkmcfbhxa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gnyzobiox.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gkiefeoux.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gpbmizjun.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gehrrrgos.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gnxbjzcbd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glvlqssnh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gfmqcdcdp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gsufrudot.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/guxbvyrzt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gwlbgpcqz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gnrbxcneq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gvufghlkq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gziahmnbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gndcfefpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gbcogdxzk.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gsxlpnhdf.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gqmohiyqf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/ggmurdnhw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gwxixngno.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gnexkifnc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/govhyvyfr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gzwpiobfx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gthcafpde.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqyprybwq.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxoffwdwg.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gteslnmgs.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gdjokpaoa.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkycodfzc.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmngladix.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfcuyywlp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gqobrkzzd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gctrcxjof.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/garxkwaao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gdfyhrpup.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gcygdvrru.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gsnhkyqfl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/glpuxklcw.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ggqtipbxv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/geeyrjyzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gfqdwjlrq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/guynzyeoh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gmzfypjcm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gontenkqf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gpsvrldrf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gnqjfaxbc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gbdfjqdcm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/guekkddto.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/golxpymaw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gurfjxuec.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gxqqyluho.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gvydxclxh.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqsddlbxm.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/goivmffcg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gfbidruzu.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/giowtwfbd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/greymdxzt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/glqrvoehl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/goghutsgw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gldirnxmk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/grvhxskyc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gtltwhbto.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gvjohnrmt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gidzpqedn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmdbrcvlg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjramgczs.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gqqrletpv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfqjgsway.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gxdgtzwoe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gmezrpwld.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gwghsmzdh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gwvnijelg.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjbglxkdc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gcitutjbn.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gpuwtxlpd.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gmquaeuto.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gixxiycwb.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gwrwyazyv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gudwmwzgm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/genqziaei.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gbqlpfiai.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gvosvucca.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gpfddcsym.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gkncrhigv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gtniulixg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gutfrtucq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/ggmpycnyj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gtsvptozg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/ggzkpkeba.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gxlcfuosi.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvidbxxga.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtqkuszud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gdlyqfqhl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghfioqbaf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdvdhnjyr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gihxlzhpp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gogtrrhsj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gspkgtnhl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gapxvckxq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gvdexnzae.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gjrypqsov.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gdtsktvvt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gbukdflof.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcosmcckz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gnaooalwb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/guswvvsmm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/glogjanhz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwaobpovh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gdeymsrwv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gaztchuhs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gepihfnax.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gcjsytfsc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gmyzafdom.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gooezsqle.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ggzzxzsvk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gpewyipwc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gwctrqbho.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggydwjatv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/guypkmfos.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/goyktuhkj.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gkfnwsxna.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/guivlajlr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqypibimd.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gklvolevh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxfukqivm.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gojdmblsm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gaptoqeja.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/glankpkaq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gyysufpie.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsvhvohpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gphvazoxb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/ghvfycgxy.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/ghiehcbqq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/giiluznsg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gejilctao.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gvqbjpchm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gwrzeptly.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnbrvdjqo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gcnpjtivl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glidlmula.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gytfawkjq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gyaczluaj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gswfgpifd.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gsmjadspp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gsotinjye.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrvklrn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gammzcedo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gkyewkttv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdcdgsqto.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gjlljpzuo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gnqfijscs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gbehqtwoc.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gdbuqbent.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjdrgzx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggxuwafhb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gmqnkqywg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gbymzboir.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gakfktdvc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gagcgifex.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gbmuonklj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gwoaqkngk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gjqtbmmlq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gvcnunpgt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ghjprajvs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gkjjkudji.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gsofbicxb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gzfxabelf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gadenywpe.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gpqoitfog.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gqaboqvvm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gyqcociuz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzndscqtw.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gagmreywk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gxwbwwzjd.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gysqyxjut.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gtzocwist.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/glypateca.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gnzdapcgm.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gcvfvuigm.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gkishazyr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gkwwnaoxw.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/geehomclj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxfsbfjli.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gmfezmmoc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gpwybjtaj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/glustadud.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gjoauucum.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gkpmdqluu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gnjiobtrh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gdtysybbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/grirnsfbw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gmablgfuu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/geeqyfuqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gruqytbqm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gclecbctl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/glogyktue.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gxosxeijh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbhvhremg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gpgsgzhvk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpwixvfgh.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gllhdvvql.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gsievtduw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gicwhbgnk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gqdnitxdp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gocierlti.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/grdfauksw.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glqdqnjdn.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gewwurcyf.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/ggywmjmog.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/giwjxtejc.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/geaobrrfd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/ggmsrepnf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gbghqvqpx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gfclgqevo.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gudlmqgdg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gfvkplvai.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gjqhpwtuu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gcgpwwvml.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gkqocnkfb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gderjojdk.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gdmzeospv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gradlocbl.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/ggrossabf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gczoicvsx.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gyahwqaml.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gipnmigld.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gtgwlvqst.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gfyetspeu.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gyunctric.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/glvxvwdft.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/grduhclqx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gskamqkqm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gqrmaiile.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gaottasvt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gnbsashuh.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gpazspway.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gliisockk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gxgurujnm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gleshebzf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gmzezimao.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/grjuikhbs.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/giqrljmyq.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/grddbhebm.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gklmksvyl.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gemkpfdba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/glgymhwce.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gegmvnnkl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gvyrvkfbu.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gloxbovzg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/glpklrtyn.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmfducixm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gneqzrbbj.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gutelcarb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gpdkyatig.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gnsbrvgbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gafoqsrvf.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gtrllwdcj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gzfidyqiw.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gpggguino.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gvogvbgea.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/ggezcdthe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gnkufltbo.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gixrrphze.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glbecsqtl.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ggfwzvlyt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gidphgrrg.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gjsaqwzpv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gacziqlql.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/grkttwavu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gelwaubyb.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gbwirkdgl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gaiavwlbo.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gwrgtaoyp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gvrsdmqzv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gvrvbqpig.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghpgitfoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gfurzkwzs.sHtML


<!-- 参考信息 -->