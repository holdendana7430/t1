代发 wailian999

JS:   process.argv.slice(2)
来源：http://ra.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://hn.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://cs.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://bs.huixiangedu.cn

Ruby: ARGV
来源：http://yz.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://md.shxzskj.cn

[M02] 读取环境变量
来源：http://vu.colortex.cn

Py:   os.environ.get("HOME")
来源：http://ks.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zq.nszjky.cn

JS:   process.env.HOME
来源：http://fe.shxzukj.cn

TS:   process.env.HOME
来源：http://zn.gzmigu.cn

Java: System.getenv("HOME")
来源：http://vs.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gj.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://jb.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oa.shtwfgs.cn

[M03] 执行外部命令
来源：http://co.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mn.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rf.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wx.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tx.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://go.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jk.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bo.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://be.szxytkj.cn

[M04] 获取当前工作目录
来源：http://gv.huanxung.cn

Py:   os.getcwd()
来源：http://iq.szxytkj.cn

PHP:  getcwd();
来源：http://ie.521024.cn

JS:   process.cwd()
来源：http://ee.shxzskj.cn

TS:   process.cwd()
来源：http://bd.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://qj.panjiajie.cn

Go:   os.Getwd()
来源：http://jd.521024.cn

Ruby: Dir.pwd
来源：http://gl.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gw.shxzskj.cn

[M05] 设置退出码
来源：http://nc.shxzukj.cn

Py:   sys.exit(1)
来源：http://rg.lnxyls.cn

PHP:  exit(1);
来源：http://lo.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://hc.521024.cn

TS:   process.exit(1)
来源：http://xz.521024.cn

Java: System.exit(1)
来源：http://pj.asd995.cn

Go:   os.Exit(1)
来源：http://zx.haigaiapp.cn

Ruby: exit 1
来源：http://yt.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pd.521024.cn

[M06] 向标准错误输出
来源：http://bh.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://oi.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qw.panjiajie.cn

JS:   console.error("err")
来源：http://kb.huixinmuqiang.cn

TS:   console.error("err")
来源：http://od.shtwfgs.cn

Java: System.err.println("err")
来源：http://gg.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mk.huanxung.cn

Ruby: warn "err"
来源：http://ev.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://eq.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://sx.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://du.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://er.asd995.cn

JS:   require.main === module
来源：http://di.asd995.cn

TS:   require.main === module
来源：http://nj.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ge.nicolike.cn

Go:   func main()
来源：http://ov.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rk.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://zp.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://tc.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://kk.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://qj.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://vt.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://ze.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vc.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ur.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ex.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yk.hnjuh.cn

================================================================================
来源：http://bc.jianghongdianzi.cn

N. 数据结构与算法
来源：http://nw.wgjwhj.cn

================================================================================
来源：http://sk.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://ph.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fg.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yv.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lg.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nz.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pp.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://ab.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bi.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ln.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ig.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://bt.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://is.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ix.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rc.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ob.9csxet.cn

Go:   slices.Sort(arr)
来源：http://gu.huanxung.cn

Ruby: arr.sort
来源：http://ac.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ac.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ct.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bs.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://br.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wz.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hs.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ec.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tu.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dd.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fq.szxytkj.cn

[N04] 斐波那契数列
来源：http://xa.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://py.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mz.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://to.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pk.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zq.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zl.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kd.shtwfgs.cn

[N05] 最大公约数
来源：http://dl.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://ja.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ar.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jh.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iq.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hx.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pw.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://hg.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iv.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://hb.newstarts.cn

Py:   s == s[::-1]
来源：http://qx.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://za.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://lc.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://zu.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fz.newstarts.cn

Go:   // 双指针从两端比较
来源：http://sk.521024.cn

Ruby: s == s.reverse
来源：http://xv.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wf.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://da.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fd.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wr.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ci.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://ff.9csxet.cn

Java: // 手写 HashMap
来源：http://uz.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ip.shxzukj.cn

Ruby: // 手写 Hash
来源：http://ex.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qg.asd995.cn

[N08] 生成全排列
来源：http://yt.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://kq.asd995.cn

PHP:  // 手写递归交换
来源：http://xa.hnjuh.cn

JS:   // 手写回溯递归
来源：http://cr.521024.cn

TS:   // 手写回溯递归
来源：http://js.huixiangedu.cn

Java: // 手写回溯递归
来源：http://dm.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ij.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://ne.panjiajie.cn

C#:   // 手写回溯递归
来源：http://nl.bookmarksfly.cn

[N09] 栈与队列
来源：http://gx.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mo.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yc.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tl.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mt.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://is.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zt.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tt.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eh.9csxet.cn

[N10] 链表节点定义
来源：http://ts.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ac.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://og.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://av.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ex.521024.cn

Java: class Node { int v; Node next; }
来源：http://kp.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yx.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mz.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oj.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://iw.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://td.szsharing.cn

PHP:  // 手写递归函数
来源：http://gp.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lc.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ma.shtwfgs.cn

Java: // 手写递归
来源：http://ar.yuntaijiaju.cn

Go:   // 手写递归
来源：http://ul.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gf.huanxung.cn

C#:   // 手写递归
来源：http://yw.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oj.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vj.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oo.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xa.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ym.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bu.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ya.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rl.hnjuh.cn

================================================================================
来源：http://sc.huixinmuqiang.cn

O. 并发与异步
来源：http://ny.bookmarksfly.cn

================================================================================
来源：http://dn.yuexingan06.cn

[O01] 启动一个线程
来源：http://cx.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ja.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zj.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pt.huixinmuqiang.cn

TS:   // 同 JS
来源：http://xv.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://iq.shxzukj.cn

Go:   go f()
来源：http://vs.9csxet.cn

Ruby: Thread.new { f }
来源：http://bx.szsharing.cn

C#:   Task.Run(() => F());
来源：http://zs.shxzukj.cn

[O02] 使用线程池
来源：http://gu.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yv.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yg.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://gp.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://ni.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ig.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tk.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cz.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nv.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://py.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://ql.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://fe.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://um.jctech888.com.cn

TS:   // 同 JS
来源：http://xw.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ef.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://km.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fa.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://do.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://kp.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://bm.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qv.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://zb.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yv.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uo.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ti.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tu.colortex.cn

C#:   async Task F() { await G(); }
来源：http://wc.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://ie.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://qy.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yj.521024.cn

JS:   await Promise.all(tasks)
来源：http://wj.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://mq.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xb.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ig.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://qp.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ml.bookmarksfly.cn

[O06] 使用进程池
来源：http://ab.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ak.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ge.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://hd.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://iy.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yo.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eh.hahajie.cn

Ruby: // fork 块
来源：http://kt.nicolike.cn

C#:   Parallel.For
来源：http://xz.bjjhwx.cn

================================================================================
来源：http://xo.hnjuh.cn

P. 常用工具函数
来源：http://lg.colortex.cn

================================================================================
来源：http://gy.colortex.cn

[P01] 生成 UUID
来源：http://sa.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://jw.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xq.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://yw.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://jg.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://vj.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://in.521024.cn

Ruby: SecureRandom.uuid
来源：http://jb.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://xn.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://jd.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://af.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bl.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ne.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ze.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fo.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fa.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uo.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zx.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://me.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ix.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://es.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yr.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://on.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hb.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ug.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://we.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ux.jianghongdianzi.cn

[P04] 求长度
来源：http://pd.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ow.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://um.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ey.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rb.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://pl.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://qx.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://yv.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ev.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://xn.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ur.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ab.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pl.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bh.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rf.muxihuayi.cn

Ruby: a == b
来源：http://bd.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fc.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ip.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jv.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://fg.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://px.szxytkj.cn

TS:   if (x == null) {}
来源：http://kt.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bz.gzmigu.cn

Go:   if x == nil {}
来源：http://ye.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ze.huixiangedu.cn

C#:   if (x is null) {}
来源：http://mj.bjjhwx.cn

[P07] 防抖与节流
来源：http://th.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tq.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://qh.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kq.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mq.chemitech.net.cn


<!-- 参考信息 -->