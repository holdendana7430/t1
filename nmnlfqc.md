代发 wailian999

JS:   process.exit(1)
来源：http://wu.shxzukj.cn

TS:   process.exit(1)
来源：http://nb.huixinmuqiang.cn

Java: System.exit(1)
来源：http://hc.panjiajie.cn

Go:   os.Exit(1)
来源：http://rh.bookmarksfly.cn

Ruby: exit 1
来源：http://lw.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fy.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://mt.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://gy.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://at.shtwfgs.cn

JS:   console.error("err")
来源：http://oj.chemitech.net.cn

TS:   console.error("err")
来源：http://vq.asd995.cn

Java: System.err.println("err")
来源：http://rl.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rc.asd995.cn

Ruby: warn "err"
来源：http://yo.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://kn.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ww.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://xr.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://in.muxihuayi.cn

JS:   require.main === module
来源：http://xb.shxzukj.cn

TS:   require.main === module
来源：http://ja.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://zw.521024.cn

Go:   func main()
来源：http://nx.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bc.huanxung.cn

C#:   static void Main(string[] args)
来源：http://tx.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://ib.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://es.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://pk.colortex.cn

JS:   process.platform;  process.version
来源：http://pd.nicolike.cn

TS:   process.platform;  process.version
来源：http://ge.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://to.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vc.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://le.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qt.shxzukj.cn

================================================================================
来源：http://le.shxzskj.cn

N. 数据结构与算法
来源：http://hq.szxytkj.cn

================================================================================
来源：http://vl.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://dj.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jg.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hy.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oo.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xw.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xv.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://dh.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hu.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zy.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ir.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://db.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yk.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ss.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://id.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://om.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://kh.wgjwhj.cn

Ruby: arr.sort
来源：http://xp.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gd.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ft.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://et.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://br.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yn.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nh.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cp.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qm.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dz.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jl.huanxung.cn

[N04] 斐波那契数列
来源：http://tz.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ev.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ui.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rx.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yi.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://li.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ld.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wo.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nt.9csxet.cn

[N05] 最大公约数
来源：http://yj.nicolike.cn

Py:   math.gcd(a, b)
来源：http://eb.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zo.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rx.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yc.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://po.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rx.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://ic.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lk.bjjhwx.cn

[N06] 判断回文字符串
来源：http://qc.huanxung.cn

Py:   s == s[::-1]
来源：http://yj.asd995.cn

PHP:  $s === strrev($s);
来源：http://ae.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ab.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://ig.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yk.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://mc.chemitech.net.cn

Ruby: s == s.reverse
来源：http://df.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mg.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ph.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hf.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mt.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xe.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://qt.shxzukj.cn

Java: // 手写 HashMap
来源：http://vi.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://va.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://tb.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yy.szxytkj.cn

[N08] 生成全排列
来源：http://ib.colortex.cn

Py:   itertools.permutations(arr)
来源：http://wp.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://re.szsharing.cn

JS:   // 手写回溯递归
来源：http://uv.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://is.hnjuh.cn

Java: // 手写回溯递归
来源：http://rq.colortex.cn

Go:   // 手写回溯递归
来源：http://qe.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://mn.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://zo.521024.cn

[N09] 栈与队列
来源：http://gp.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ae.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eq.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ej.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lq.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://df.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sq.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xo.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wt.panjiajie.cn

[N10] 链表节点定义
来源：http://ge.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mb.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zv.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://te.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ae.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://cd.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mo.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ah.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xz.asd995.cn

[N11] 二叉树中序遍历
来源：http://ie.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pe.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://wm.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://be.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rg.haigaiapp.cn

Java: // 手写递归
来源：http://oe.gzmigu.cn

Go:   // 手写递归
来源：http://pd.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://js.haigaiapp.cn

C#:   // 手写递归
来源：http://pz.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kk.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bg.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ax.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kr.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cr.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nc.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dx.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yq.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zh.panjiajie.cn

================================================================================
来源：http://xp.newstarts.cn

O. 并发与异步
来源：http://gz.huanxung.cn

================================================================================
来源：http://mv.colortex.cn

[O01] 启动一个线程
来源：http://nc.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rq.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sl.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qr.lnxyls.cn

TS:   // 同 JS
来源：http://xf.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://rm.wgjwhj.cn

Go:   go f()
来源：http://ce.colortex.cn

Ruby: Thread.new { f }
来源：http://yw.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://zn.nszjky.cn

[O02] 使用线程池
来源：http://rj.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wh.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eg.newstarts.cn

JS:   // worker_threads 线程池
来源：http://xt.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://an.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jq.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ck.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aj.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://po.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://mq.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://gm.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://po.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qm.huanxung.cn

TS:   // 同 JS
来源：http://es.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ls.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pr.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fz.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://bq.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://ph.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://nj.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kd.nicolike.cn

JS:   async function f() { await g(); }
来源：http://gk.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yb.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tj.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tx.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qt.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://ly.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://sp.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://um.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kn.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://yo.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://nu.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ij.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fc.nicolike.cn

Ruby: threads.map(&:join)
来源：http://yj.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vv.nicolike.cn

[O06] 使用进程池
来源：http://mk.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ek.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qp.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ys.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://ad.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://up.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qa.szsharing.cn

Ruby: // fork 块
来源：http://ot.bookmarksfly.cn

C#:   Parallel.For
来源：http://lt.colortex.cn

================================================================================
来源：http://lg.huanxung.cn

P. 常用工具函数
来源：http://jg.hnjuh.cn

================================================================================
来源：http://ao.newstarts.cn

[P01] 生成 UUID
来源：http://mv.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://ev.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uk.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://le.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://yj.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://pl.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://tc.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://zv.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://at.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://zs.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jh.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pq.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kt.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fr.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ly.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://al.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sj.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nu.lnxyls.cn

[P03] 生成短随机字符串
来源：http://rj.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iy.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dn.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ew.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://md.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nd.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sf.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fs.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tw.9csxet.cn

[P04] 求长度
来源：http://xy.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cc.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oj.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dv.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bf.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://jq.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://ay.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ya.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://no.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://bb.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lc.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qh.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://th.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rx.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rx.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ip.hnjuh.cn

Ruby: a == b
来源：http://mn.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://re.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kj.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rz.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://ci.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dj.huixiangedu.cn

TS:   if (x == null) {}
来源：http://uu.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rs.shxzukj.cn

Go:   if x == nil {}
来源：http://dm.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bv.lnxyls.cn

C#:   if (x is null) {}
来源：http://zh.jctech888.com.cn

[P07] 防抖与节流
来源：http://ps.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xt.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://xo.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kr.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yu.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ug.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fc.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zo.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sd.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://tl.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nk.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oo.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ng.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ut.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bt.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pi.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vj.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kr.haigaiapp.cn

================================================================================
来源：http://ys.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gv.haigaiapp.cn

================================================================================
来源：http://uc.521024.cn

[Q01] 创建表
来源：http://ee.nszjky.cn

CREATE TABLE users (
来源：http://fo.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ha.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://iu.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://bn.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kl.chemitech.net.cn

);
来源：http://hf.shxzukj.cn

[Q02] 创建带外键的表
来源：http://iz.hnjuh.cn

CREATE TABLE orders (
来源：http://qk.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://te.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://zq.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://uj.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lc.shxzukj.cn

);
来源：http://om.hnjuh.cn

[Q03] 增加列
来源：http://wc.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bh.gzmigu.cn

[Q04] 修改列类型
来源：http://tv.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nz.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ay.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dp.asd995.cn

[Q06] 删除列
来源：http://yz.9csxet.cn


<!-- 参考信息 -->