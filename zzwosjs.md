代发 wailian999

[M04] 获取当前工作目录
来源：http://hc.hahajie.cn

Py:   os.getcwd()
来源：http://my.shxzukj.cn

PHP:  getcwd();
来源：http://rf.panjiajie.cn

JS:   process.cwd()
来源：http://ft.nszjky.cn

TS:   process.cwd()
来源：http://ht.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://vh.wgjwhj.cn

Go:   os.Getwd()
来源：http://lg.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ib.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uc.lnxyls.cn

[M05] 设置退出码
来源：http://yt.panjiajie.cn

Py:   sys.exit(1)
来源：http://xe.huixinmuqiang.cn

PHP:  exit(1);
来源：http://qm.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://jv.hahajie.cn

TS:   process.exit(1)
来源：http://mv.gzmigu.cn

Java: System.exit(1)
来源：http://mk.shxzukj.cn

Go:   os.Exit(1)
来源：http://kr.shxzukj.cn

Ruby: exit 1
来源：http://sa.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xa.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ja.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ng.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ea.bjjhwx.cn

JS:   console.error("err")
来源：http://gq.newstarts.cn

TS:   console.error("err")
来源：http://ol.shtwfgs.cn

Java: System.err.println("err")
来源：http://rg.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jl.chemitech.net.cn

Ruby: warn "err"
来源：http://os.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://mr.nicolike.cn

[M07] 判断是否为主入口
来源：http://xj.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://wg.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.haigaiapp.cn

JS:   require.main === module
来源：http://we.bookmarksfly.cn

TS:   require.main === module
来源：http://te.hnjuh.cn

Java: public static void main(String[] args)
来源：http://eg.huixiangedu.cn

Go:   func main()
来源：http://ub.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://py.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://cx.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://mp.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://an.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://he.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://zu.asd995.cn

TS:   process.platform;  process.version
来源：http://ax.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rd.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ka.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sf.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nk.bjjhwx.cn

================================================================================
来源：http://da.jianghongdianzi.cn

N. 数据结构与算法
来源：http://js.haigaiapp.cn

================================================================================
来源：http://fg.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://io.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pm.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sy.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://re.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://px.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tk.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://wv.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ij.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ze.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://rv.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://zh.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://me.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pb.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lq.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ki.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://im.wgjwhj.cn

Ruby: arr.sort
来源：http://dt.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ov.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://vw.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nc.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ty.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oy.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fx.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ao.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mv.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://il.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kt.wgjwhj.cn

[N04] 斐波那契数列
来源：http://xs.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lp.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dn.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zi.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mk.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ei.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iq.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hv.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rf.shxzskj.cn

[N05] 最大公约数
来源：http://xl.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://vh.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gh.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bd.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qs.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://py.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cw.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://jy.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rb.lnxyls.cn

[N06] 判断回文字符串
来源：http://rj.haigaiapp.cn

Py:   s == s[::-1]
来源：http://es.colortex.cn

PHP:  $s === strrev($s);
来源：http://se.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://xj.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://rp.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ps.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://vo.panjiajie.cn

Ruby: s == s.reverse
来源：http://hg.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dc.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://lo.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wa.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zf.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jv.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://il.szxytkj.cn

Java: // 手写 HashMap
来源：http://nx.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ry.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://uc.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nd.szxytkj.cn

[N08] 生成全排列
来源：http://gb.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://jh.nszjky.cn

PHP:  // 手写递归交换
来源：http://md.panjiajie.cn

JS:   // 手写回溯递归
来源：http://ph.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://wp.wgjwhj.cn

Java: // 手写回溯递归
来源：http://mb.huanxung.cn

Go:   // 手写回溯递归
来源：http://bg.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://hp.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://tw.yuexingan06.cn

[N09] 栈与队列
来源：http://ty.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bq.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ba.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bh.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wd.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ug.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xq.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zs.yuexingan06.cn

[N10] 链表节点定义
来源：http://rc.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xn.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pl.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uc.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tm.521024.cn

Java: class Node { int v; Node next; }
来源：http://aq.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ya.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lh.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xr.9csxet.cn

[N11] 二叉树中序遍历
来源：http://fu.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vk.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ju.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sm.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.gzmigu.cn

Java: // 手写递归
来源：http://aj.9csxet.cn

Go:   // 手写递归
来源：http://id.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lo.muxihuayi.cn

C#:   // 手写递归
来源：http://qz.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rn.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://si.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qa.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rj.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ug.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tx.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oq.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mp.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lm.hnjuh.cn

================================================================================
来源：http://vf.yuexingan06.cn

O. 并发与异步
来源：http://tu.shxzskj.cn

================================================================================
来源：http://uj.gzmigu.cn

[O01] 启动一个线程
来源：http://ue.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jc.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://in.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zo.chemitech.net.cn

TS:   // 同 JS
来源：http://mv.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://qt.hnjuh.cn

Go:   go f()
来源：http://pm.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://uj.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://er.shxzskj.cn

[O02] 使用线程池
来源：http://lr.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lx.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://de.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://sn.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ky.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mt.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sh.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://un.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://re.newstarts.cn

[O03] 加锁保护共享数据
来源：http://ou.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://pg.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://nf.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hn.nicolike.cn

TS:   // 同 JS
来源：http://ya.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://tz.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ex.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fc.521024.cn

C#:   lock (gate) { shared++; }
来源：http://zf.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://zc.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://et.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bw.newstarts.cn

JS:   async function f() { await g(); }
来源：http://sv.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ff.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://on.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uo.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lp.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://yc.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ho.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ai.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ce.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://sx.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://qb.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eb.nicolike.cn

Ruby: threads.map(&:join)
来源：http://yb.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fr.bookmarksfly.cn

[O06] 使用进程池
来源：http://ii.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nw.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vh.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://sv.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://it.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pq.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zh.jctech888.com.cn

Ruby: // fork 块
来源：http://nm.521024.cn

C#:   Parallel.For
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://xb.gzmigu.cn

P. 常用工具函数
来源：http://ri.szsharing.cn

================================================================================
来源：http://fm.chemitech.net.cn

[P01] 生成 UUID
来源：http://wp.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://ny.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://me.szsharing.cn

JS:   crypto.randomUUID()
来源：http://dr.colortex.cn

TS:   crypto.randomUUID()
来源：http://pp.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://fb.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://jt.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://jc.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ui.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://hg.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bg.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wx.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hp.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ze.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://by.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://es.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jx.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ih.gzmigu.cn

[P03] 生成短随机字符串
来源：http://cg.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gz.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jc.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://no.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rp.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tp.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ck.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ly.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ip.hahajie.cn

[P04] 求长度
来源：http://jr.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gx.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://am.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wx.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://jd.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://no.9csxet.cn

Ruby: x.length;  x.size
来源：http://mr.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jx.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://qo.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rl.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jc.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tn.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ah.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nr.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://md.9csxet.cn

Ruby: a == b
来源：http://ag.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vn.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://al.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nq.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://ni.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jw.lnxyls.cn

TS:   if (x == null) {}
来源：http://br.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gk.jctech888.com.cn

Go:   if x == nil {}
来源：http://at.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yg.jctech888.com.cn

C#:   if (x is null) {}
来源：http://bx.hahajie.cn

[P07] 防抖与节流
来源：http://va.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zb.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://sk.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dm.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uc.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qf.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yu.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sm.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mu.newstarts.cn

[P08] 处理浮点精度问题
来源：http://wl.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ch.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://br.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rt.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ju.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vp.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pu.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wu.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lq.nszjky.cn

================================================================================
来源：http://uf.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vh.jctech888.com.cn

================================================================================
来源：http://nz.lnxyls.cn

[Q01] 创建表
来源：http://ti.jctech888.com.cn

CREATE TABLE users (
来源：http://rg.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hb.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://rf.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://lm.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ou.asd995.cn

);
来源：http://gk.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://rh.haigaiapp.cn

CREATE TABLE orders (
来源：http://jt.panjiajie.cn


<!-- 参考信息 -->