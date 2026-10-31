代发 wailian999

JS:   process.exit(1)
来源：http://lt.chemitech.net.cn

TS:   process.exit(1)
来源：http://my.9csxet.cn

Java: System.exit(1)
来源：http://dm.huanxung.cn

Go:   os.Exit(1)
来源：http://db.asd995.cn

Ruby: exit 1
来源：http://tt.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zg.asd995.cn

[M06] 向标准错误输出
来源：http://xd.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://qj.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ls.bjjhwx.cn

JS:   console.error("err")
来源：http://nu.hnjuh.cn

TS:   console.error("err")
来源：http://fp.lnxyls.cn

Java: System.err.println("err")
来源：http://lz.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ku.gzmigu.cn

Ruby: warn "err"
来源：http://uf.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ri.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://lg.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://pf.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://la.nicolike.cn

JS:   require.main === module
来源：http://ms.colortex.cn

TS:   require.main === module
来源：http://rp.9csxet.cn

Java: public static void main(String[] args)
来源：http://la.nszjky.cn

Go:   func main()
来源：http://jj.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bb.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://sz.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://bm.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://qd.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://du.hnjuh.cn

JS:   process.platform;  process.version
来源：http://lq.shxzukj.cn

TS:   process.platform;  process.version
来源：http://sj.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zf.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aa.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ev.huixinmuqiang.cn

================================================================================
来源：http://rf.huixiangedu.cn

N. 数据结构与算法
来源：http://ev.chemitech.net.cn

================================================================================
来源：http://gb.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://kk.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yn.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kr.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gn.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nr.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wp.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://se.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hm.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gy.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://sl.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://pb.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nh.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cw.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uk.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dd.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://ug.wgjwhj.cn

Ruby: arr.sort
来源：http://fg.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bi.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://bg.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ee.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://jm.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pf.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ys.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lk.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tq.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pj.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iz.shxzukj.cn

[N04] 斐波那契数列
来源：http://ld.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://to.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://af.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dk.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zv.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mg.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jf.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://re.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gt.szxytkj.cn

[N05] 最大公约数
来源：http://iq.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://hh.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yq.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vi.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vr.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xx.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qa.szsharing.cn

Ruby: a.gcd(b)
来源：http://hk.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rx.szxytkj.cn

[N06] 判断回文字符串
来源：http://hs.gzmigu.cn

Py:   s == s[::-1]
来源：http://bk.9csxet.cn

PHP:  $s === strrev($s);
来源：http://ad.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://oh.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://jq.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://un.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://va.huixiangedu.cn

Ruby: s == s.reverse
来源：http://gg.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://us.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://ob.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rd.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yl.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zj.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://pd.hahajie.cn

Java: // 手写 HashMap
来源：http://vm.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://mm.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://nw.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jx.hnjuh.cn

[N08] 生成全排列
来源：http://zv.colortex.cn

Py:   itertools.permutations(arr)
来源：http://yr.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://nd.gzmigu.cn

JS:   // 手写回溯递归
来源：http://bj.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://ih.asd995.cn

Java: // 手写回溯递归
来源：http://xx.nszjky.cn

Go:   // 手写回溯递归
来源：http://yb.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://mn.colortex.cn

C#:   // 手写回溯递归
来源：http://ar.shxzskj.cn

[N09] 栈与队列
来源：http://sk.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kl.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rw.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ze.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gv.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jf.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ns.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gk.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wd.bookmarksfly.cn

[N10] 链表节点定义
来源：http://tg.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ld.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lw.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zg.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qw.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://oc.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://km.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wx.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ta.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://wq.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sr.huanxung.cn

PHP:  // 手写递归函数
来源：http://nq.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://di.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bm.521024.cn

Java: // 手写递归
来源：http://na.huixinmuqiang.cn

Go:   // 手写递归
来源：http://mi.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eh.521024.cn

C#:   // 手写递归
来源：http://mh.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tw.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hf.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lk.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ke.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rp.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cx.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cz.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rm.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ml.newstarts.cn

================================================================================
来源：http://qk.wgjwhj.cn

O. 并发与异步
来源：http://xh.521024.cn

================================================================================
来源：http://zw.yuexingan06.cn

[O01] 启动一个线程
来源：http://xo.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qy.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jk.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mm.szsharing.cn

TS:   // 同 JS
来源：http://ti.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://wi.szxytkj.cn

Go:   go f()
来源：http://an.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://pe.newstarts.cn

C#:   Task.Run(() => F());
来源：http://uh.gzmigu.cn

[O02] 使用线程池
来源：http://ep.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jj.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xf.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://cr.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://yd.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zw.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qj.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tf.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zn.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://sq.szxytkj.cn

Py:   with lock: shared += 1
来源：http://tw.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://lq.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ag.huixiangedu.cn

TS:   // 同 JS
来源：http://qn.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://pr.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ri.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://my.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://yo.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://hg.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://jv.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dg.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://nu.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hw.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qw.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://na.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sg.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://zr.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://nx.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://uc.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sz.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://kz.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://or.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sl.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oj.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://vg.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bn.jctech888.com.cn

[O06] 使用进程池
来源：http://bs.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zt.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sk.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://td.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://zc.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cg.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pm.hahajie.cn

Ruby: // fork 块
来源：http://gh.yuntaijiaju.cn

C#:   Parallel.For
来源：http://xs.jctech888.com.cn

================================================================================
来源：http://ti.9csxet.cn

P. 常用工具函数
来源：http://gn.shtwfgs.cn

================================================================================
来源：http://mo.nszjky.cn

[P01] 生成 UUID
来源：http://fx.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://yu.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pc.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://fr.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://jl.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://gb.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://bt.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://oc.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://xu.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://cx.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ug.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eq.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://py.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://td.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wk.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ww.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://up.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nc.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://oo.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zp.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sd.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ih.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gr.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xe.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pg.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zr.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://io.521024.cn

[P04] 求长度
来源：http://ht.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://id.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ze.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://us.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lk.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://tx.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://kt.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://oo.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tg.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://ws.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zi.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://on.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jq.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kx.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ot.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ru.9csxet.cn

Ruby: a == b
来源：http://rw.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gn.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aa.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ok.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://zb.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sh.haigaiapp.cn

TS:   if (x == null) {}
来源：http://nt.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vc.521024.cn

Go:   if x == nil {}
来源：http://yt.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qh.9csxet.cn

C#:   if (x is null) {}
来源：http://tl.haigaiapp.cn

[P07] 防抖与节流
来源：http://ze.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ju.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ub.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nx.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lx.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://og.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wk.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ff.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hc.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://yg.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ak.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ci.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kz.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qf.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ow.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ri.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zn.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bz.yuexingan06.cn

================================================================================
来源：http://rm.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://if.panjiajie.cn

================================================================================
来源：http://nk.huanxung.cn

[Q01] 创建表
来源：http://xn.szsharing.cn

CREATE TABLE users (
来源：http://hy.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eb.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://id.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://xs.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ai.jianghongdianzi.cn

);
来源：http://hq.newstarts.cn

[Q02] 创建带外键的表
来源：http://rg.szsharing.cn

CREATE TABLE orders (
来源：http://dc.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kn.colortex.cn

user_id INT NOT NULL,
来源：http://ps.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://wr.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lb.yuexingan06.cn

);
来源：http://bq.muxihuayi.cn

[Q03] 增加列
来源：http://gu.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lp.newstarts.cn

[Q04] 修改列类型
来源：http://rw.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qv.haigaiapp.cn

[Q05] 重命名列
来源：http://ou.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oh.gzmigu.cn

[Q06] 删除列
来源：http://zt.yuntaijiaju.cn


<!-- 参考信息 -->