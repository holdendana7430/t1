代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ik.bjjhwx.cn

JS:   process.env.HOME
来源：http://iv.9csxet.cn

TS:   process.env.HOME
来源：http://yj.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://zf.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hb.521024.cn

Ruby: ENV["HOME"]
来源：http://tj.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kj.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://pa.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pl.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kn.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bu.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nq.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sf.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ds.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hi.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://gx.521024.cn

[M04] 获取当前工作目录
来源：http://ye.wgjwhj.cn

Py:   os.getcwd()
来源：http://vz.asd995.cn

PHP:  getcwd();
来源：http://tx.szxytkj.cn

JS:   process.cwd()
来源：http://ha.bookmarksfly.cn

TS:   process.cwd()
来源：http://vu.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://zz.szsharing.cn

Go:   os.Getwd()
来源：http://ub.gzmigu.cn

Ruby: Dir.pwd
来源：http://jd.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xr.huixiangedu.cn

[M05] 设置退出码
来源：http://rc.gzmigu.cn

Py:   sys.exit(1)
来源：http://jy.bjjhwx.cn

PHP:  exit(1);
来源：http://od.haigaiapp.cn

JS:   process.exit(1)
来源：http://ph.nszjky.cn

TS:   process.exit(1)
来源：http://ec.szsharing.cn

Java: System.exit(1)
来源：http://vv.newstarts.cn

Go:   os.Exit(1)
来源：http://ob.yuntaijiaju.cn

Ruby: exit 1
来源：http://fl.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qu.shtwfgs.cn

[M06] 向标准错误输出
来源：http://yx.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://wg.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bf.9csxet.cn

JS:   console.error("err")
来源：http://ow.9csxet.cn

TS:   console.error("err")
来源：http://jr.szsharing.cn

Java: System.err.println("err")
来源：http://qp.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hq.shtwfgs.cn

Ruby: warn "err"
来源：http://dh.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://do.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://sn.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://pd.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://de.jctech888.com.cn

JS:   require.main === module
来源：http://oo.wgjwhj.cn

TS:   require.main === module
来源：http://qy.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ax.huanxung.cn

Go:   func main()
来源：http://tu.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rx.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://pv.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://zm.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://vj.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://cg.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://zg.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://rn.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mt.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oi.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://je.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oh.panjiajie.cn

================================================================================
来源：http://mp.huixiangedu.cn

N. 数据结构与算法
来源：http://gu.bjjhwx.cn

================================================================================
来源：http://il.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://xy.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zw.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ak.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bb.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bn.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iz.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://qu.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://et.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ps.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://mi.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://va.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kl.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xf.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xb.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gb.asd995.cn

Go:   slices.Sort(arr)
来源：http://vg.panjiajie.cn

Ruby: arr.sort
来源：http://hc.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://as.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://rv.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://st.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://oa.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rn.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nx.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ku.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nj.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wd.szsharing.cn

[N04] 斐波那契数列
来源：http://ha.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ll.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eb.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jf.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zj.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qk.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vh.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zr.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fr.huixiangedu.cn

[N05] 最大公约数
来源：http://ip.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://xq.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bj.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sz.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ka.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zo.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lq.lnxyls.cn

Ruby: a.gcd(b)
来源：http://tk.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dn.panjiajie.cn

[N06] 判断回文字符串
来源：http://nv.yuexingan06.cn

Py:   s == s[::-1]
来源：http://qw.newstarts.cn

PHP:  $s === strrev($s);
来源：http://ky.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://zs.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://ud.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dy.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://qd.wgjwhj.cn

Ruby: s == s.reverse
来源：http://rc.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tg.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ef.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pb.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rn.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ar.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://zq.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ne.newstarts.cn

Go:   // 手写 map[int]int
来源：http://pk.asd995.cn

Ruby: // 手写 Hash
来源：http://cf.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rw.yuexingan06.cn

[N08] 生成全排列
来源：http://hn.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://ll.9csxet.cn

PHP:  // 手写递归交换
来源：http://oz.hnjuh.cn

JS:   // 手写回溯递归
来源：http://kq.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://pp.hahajie.cn

Java: // 手写回溯递归
来源：http://yb.panjiajie.cn

Go:   // 手写回溯递归
来源：http://cc.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://yx.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://as.muxihuayi.cn

[N09] 栈与队列
来源：http://yu.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qd.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jb.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://um.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ml.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pv.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ci.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nz.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yg.jctech888.com.cn

[N10] 链表节点定义
来源：http://og.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vo.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mn.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://po.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://du.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://bd.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wv.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://am.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hv.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://mi.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ca.shxzskj.cn

PHP:  // 手写递归函数
来源：http://de.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sb.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aw.shtwfgs.cn

Java: // 手写递归
来源：http://ll.hnjuh.cn

Go:   // 手写递归
来源：http://qw.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hj.shxzskj.cn

C#:   // 手写递归
来源：http://eg.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fa.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://up.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bl.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ai.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qt.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kr.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ht.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qa.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gw.wgjwhj.cn

================================================================================
来源：http://mv.gzmigu.cn

O. 并发与异步
来源：http://cb.huixinmuqiang.cn

================================================================================
来源：http://mv.nszjky.cn

[O01] 启动一个线程
来源：http://fy.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ij.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://up.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xb.chemitech.net.cn

TS:   // 同 JS
来源：http://zc.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://pp.chemitech.net.cn

Go:   go f()
来源：http://vm.colortex.cn

Ruby: Thread.new { f }
来源：http://lg.newstarts.cn

C#:   Task.Run(() => F());
来源：http://lo.asd995.cn

[O02] 使用线程池
来源：http://rg.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://re.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xp.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://tq.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://yy.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yl.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wp.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uc.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jb.szsharing.cn

[O03] 加锁保护共享数据
来源：http://kn.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://ga.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://mi.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ee.szxytkj.cn

TS:   // 同 JS
来源：http://yj.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://oz.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pc.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zi.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://cg.szsharing.cn

[O04] 定义异步函数并等待
来源：http://cw.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://cm.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yy.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://ex.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hq.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nt.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zm.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ml.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://it.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://qj.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://lu.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lk.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://yl.521024.cn

TS:   await Promise.all(tasks)
来源：http://vy.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ml.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ld.nszjky.cn

Ruby: threads.map(&:join)
来源：http://un.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wv.huanxung.cn

[O06] 使用进程池
来源：http://lp.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://du.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dk.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://pf.colortex.cn

TS:   // child_process / cluster 模块
来源：http://br.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://og.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ko.shxzukj.cn

Ruby: // fork 块
来源：http://ux.nszjky.cn

C#:   Parallel.For
来源：http://ga.huixiangedu.cn

================================================================================
来源：http://hc.jctech888.com.cn

P. 常用工具函数
来源：http://vi.shxzskj.cn

================================================================================
来源：http://ym.shxzukj.cn

[P01] 生成 UUID
来源：http://mg.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://at.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ly.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://ru.newstarts.cn

TS:   crypto.randomUUID()
来源：http://co.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ci.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://jy.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://gw.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://xm.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://qg.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bt.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nc.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dt.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ya.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cm.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vc.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zu.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ua.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://nv.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fc.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nq.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hx.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tm.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ty.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tn.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ye.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vo.chemitech.net.cn

[P04] 求长度
来源：http://em.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ss.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ll.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dn.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ef.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://pp.newstarts.cn

Go:   len(arr);  len(m)
来源：http://me.shxzukj.cn

Ruby: x.length;  x.size
来源：http://xm.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dy.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://hu.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qx.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sf.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uv.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iv.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qk.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hf.colortex.cn

Ruby: a == b
来源：http://yd.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oz.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eu.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qv.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://cc.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xa.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://ug.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hh.huanxung.cn

Go:   if x == nil {}
来源：http://yz.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rf.gzmigu.cn

C#:   if (x is null) {}
来源：http://cc.szsharing.cn

[P07] 防抖与节流
来源：http://az.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zm.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://tg.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sc.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sf.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://to.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lm.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cz.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cr.nszjky.cn

[P08] 处理浮点精度问题
来源：http://my.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://on.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://th.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jj.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qz.huixinmuqiang.cn


<!-- 参考信息 -->