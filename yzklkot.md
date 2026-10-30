代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gzapurfmo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/grflbqelp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqrqjsfqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gcqglrwav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/ghnppmvhk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/glrwpsumr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gquthglky.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdifysaq.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gozuovhyf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grledhsdd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/glexppthv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfquqayos.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gruzmibmm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gjrbzctmt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gdjkgrdrn.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gblqdavdi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gxvesfrrt.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gvmsvlzql.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gbpnzpuoz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gonfmndlm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gbkehgsjn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gyweyixtw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/grahgmcab.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gkhfrqjzg.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzpqswyro.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gvhuuezer.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gftsbtoac.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gdhkvicdz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gpsfspqjq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/geqrnitup.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gfvrwsgpj.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gfkzljbft.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gxeyquhvu.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gycscqhlk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gqbapvynx.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gvfpvjavo.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gzqswgqde.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gauwsaybc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmwmmnwjm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glalgypvz.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjjggfcbg.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtythabcl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gggpuqxfw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goouiuybm.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gjhtecepr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/glmvjqers.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdxqfncss.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gocqiemub.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gdexrxtcm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gnyafdwjy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gtiiuomyj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gazjeftzo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/grwxfntai.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gosqodgkf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gudsdutyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/grnpxwlyk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/guztyeaeg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gwiphmjwy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gqajusqns.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gicxsbkbm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gdlexfsnp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/glzapuwze.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gzquofhlq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gpljbudae.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gukhbmayt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjbvmrfqz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gmdwbjznp.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/goylimbss.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gghvozclc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gwsychvln.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gktruygyn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/glbnlcphy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gyvrrokzx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gwybdqzdf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gqxjniywo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gakxjyqux.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guneojdmq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gdripimcw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gsmsmahjg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gzbczspwe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gobtoanan.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/ggwoealeg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gepseiuyt.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gbkirbxag.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gefqagrkj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gizuweuhb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gfczkmcji.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gxevbqrco.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gbhjoyvhv.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/glihbjzea.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gcnvdskuz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gdibvoijl.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gigyurfia.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gjknkhmmz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/grsenyvfb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gtzxkgica.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gdnlgafor.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gokmrcufd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gqptpidaz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gvqpepcyq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gtdyjrjgy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gntwrcxkq.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/geznnimvy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gwvbntckd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gnyroszkm.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gztkrfylp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkdfqjqor.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gggsgplhj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gqqknquey.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/goxzrqtfl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/griacgpgj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqjuxqi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gzemsbvtw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gwwhxpwga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gexcpxsqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gsshttwdj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsvgtth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gnkneyygh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gnvlhzycm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gkzpqyegt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gstdolhfp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/ghmfpkuhc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gpxkbvvrl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gvwaqycoe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gsxdqtizj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gmmmicqfk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gwfaxafdi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/girypfcls.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/glmsskcls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gjpmssout.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gsnluhuqn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gshezewew.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gyilxriwh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gwfkreoym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gfhiamqkl.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gdlrbigjl.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gdvphtvry.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzbxvfjfu.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gmreujsry.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gymalmzcu.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjfysdyyu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcheufwwt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/grfdydmqo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/glkrlwdfs.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grummneug.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/ghczeqqnp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gpvijtkwb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gnvuisxoy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/ghkrfrtxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gcizoiojg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gdfmhpefe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gucttjibc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gfkxlhrat.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gbhpfydup.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/givxtiszu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gikgmlyvl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gackhwlxs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/glppjxgte.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gligpgleq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gvdkxqupf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gilgksbvw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gkpyukzem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdygfdfgw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gnvubdbyw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gfvkkrnfp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gvxjyjyfu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/ggnokqnoc.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gifqqspir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gomeswink.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/grlqlfouw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjwgjoctc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gbeqyswkd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghrhygftj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gyglcwtkb.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gdcnorscj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gludqmkbw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gayvatrvl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gtywhxqhg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gvjzohlsm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gehvuaoft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/giholsaom.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gnkgokyxu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/goowxymts.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gbnjbzskx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gsbdpwxbc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gcgolxlvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ggfcwtcip.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmaesyysf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gixnbssob.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghklvkndf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gnahgbxpg.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gasfxkead.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gzppseptm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gackxefpc.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/giudrkske.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gnekszcbw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/guwedbfaj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwccqsjcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqtgtgbgf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/guwghuckw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gimzgjrih.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjcmyxf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gbgjndeuq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/giealuttk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gnevrzeps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gmrtkgbbk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gwotjhzcr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/glunhaefh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gsustowtp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gjrnzryze.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gbhdrlwtp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gsltpdnal.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfkixjjsk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/geeezimes.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqworawrj.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkfwmie.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/grlhvsnwf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gctifypti.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/guuaaevur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gypnhjvmk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gepzyvcal.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gaxukvlfp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/ghhvbqnnt.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gziywremw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gaswfihxz.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gwexorvxr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gfxvpyvlo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gyelousyl.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gkdfbsiul.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/galqztxqh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gewpkqepl.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/giktoylsi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gynmrlmlq.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gevskjfvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gqslcbclx.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gtfovnzar.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gdwkevhgd.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gkaumsvda.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpikeijbt.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gyftiiutl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gcpoblrun.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/guqwxkbhk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gtcgdutbx.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ggvbezuuz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gempwtcwy.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gzawszhqe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwyplxlrg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gylokvdxj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gslytngii.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gmogskiuy.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gjtlnxuof.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gjznurpcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gqwnklkcy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/giypynahe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/geuievmqa.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/ghjdyrhtc.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gluuzfimw.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcgzdyyox.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggciykgrk.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gmnoisuox.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gftlhabgl.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gtpoqkmao.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gseupfdnt.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gdrcfjkst.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gmlzksmcv.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glflajqlt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gwzfelelv.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gehypimwk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gceedrjqg.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gabmihzqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gscvfarco.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gnxzljbfd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gsvbqdwkf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/guepvlzfy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gvtqpymwp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/ggzqjvlbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gpqzgntcu.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gqdfwulao.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gabyiptvq.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gqmvicynx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guhinjmbz.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gynmgdnvs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkfummawp.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gpnxqyqsq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyxlrcusy.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbfanghwh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gydyttymp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gfhuibawc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gzcjobrmu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gurogstbp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcpgchvcu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gffwpaaqa.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gyjvqhfys.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/giuaithge.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gyxchmalu.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gupwggevy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gszxlxidg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxooarslp.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/ghsvvffos.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gfskdmzmi.sHtML


<!-- 参考信息 -->