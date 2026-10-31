代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bp.gzmigu.cn

JS:   process.env.HOME
来源：http://sw.yuexingan06.cn

TS:   process.env.HOME
来源：http://ju.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://hk.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mm.newstarts.cn

Ruby: ENV["HOME"]
来源：http://ko.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fp.wgjwhj.cn

[M03] 执行外部命令
来源：http://xa.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kq.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mc.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gb.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pj.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gw.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cy.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xm.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://nv.nicolike.cn

[M04] 获取当前工作目录
来源：http://wu.haigaiapp.cn

Py:   os.getcwd()
来源：http://zh.jctech888.com.cn

PHP:  getcwd();
来源：http://vn.szsharing.cn

JS:   process.cwd()
来源：http://po.yuntaijiaju.cn

TS:   process.cwd()
来源：http://no.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yq.lnxyls.cn

Go:   os.Getwd()
来源：http://hc.521024.cn

Ruby: Dir.pwd
来源：http://bl.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cf.bookmarksfly.cn

[M05] 设置退出码
来源：http://lt.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://we.lnxyls.cn

PHP:  exit(1);
来源：http://ya.hnjuh.cn

JS:   process.exit(1)
来源：http://iu.nicolike.cn

TS:   process.exit(1)
来源：http://dc.nicolike.cn

Java: System.exit(1)
来源：http://al.gzmigu.cn

Go:   os.Exit(1)
来源：http://jo.yuntaijiaju.cn

Ruby: exit 1
来源：http://qi.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rx.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://yf.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://qq.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yh.lnxyls.cn

JS:   console.error("err")
来源：http://et.hahajie.cn

TS:   console.error("err")
来源：http://ib.newstarts.cn

Java: System.err.println("err")
来源：http://nv.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bt.9csxet.cn

Ruby: warn "err"
来源：http://uj.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://dr.colortex.cn

[M07] 判断是否为主入口
来源：http://dt.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://jw.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nl.521024.cn

JS:   require.main === module
来源：http://rs.panjiajie.cn

TS:   require.main === module
来源：http://wn.nicolike.cn

Java: public static void main(String[] args)
来源：http://qu.bjjhwx.cn

Go:   func main()
来源：http://ba.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vh.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://ly.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://xi.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://ca.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://xm.shxzskj.cn

JS:   process.platform;  process.version
来源：http://dk.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://kv.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ix.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pn.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ja.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mg.jianghongdianzi.cn

================================================================================
来源：http://sn.asd995.cn

N. 数据结构与算法
来源：http://vf.newstarts.cn

================================================================================
来源：http://db.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://iv.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sd.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://su.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gm.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fb.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yq.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://jb.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ev.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qk.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ut.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://dt.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iu.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sh.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ky.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://od.asd995.cn

Go:   slices.Sort(arr)
来源：http://mf.newstarts.cn

Ruby: arr.sort
来源：http://dn.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kt.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://lu.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sl.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://ue.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jf.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fd.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bj.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fy.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nh.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wi.wgjwhj.cn

[N04] 斐波那契数列
来源：http://da.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xc.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rt.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fa.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bm.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rq.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hs.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ch.hahajie.cn

[N05] 最大公约数
来源：http://bw.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://zd.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xm.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rh.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ip.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://np.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zy.9csxet.cn

Ruby: a.gcd(b)
来源：http://ow.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ti.panjiajie.cn

[N06] 判断回文字符串
来源：http://sb.huanxung.cn

Py:   s == s[::-1]
来源：http://rs.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://aq.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://cp.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://fz.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://me.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ya.szxytkj.cn

Ruby: s == s.reverse
来源：http://tt.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hb.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://oy.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nm.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ux.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ia.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://dn.nszjky.cn

Java: // 手写 HashMap
来源：http://dh.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://tk.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ne.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mq.shxzukj.cn

[N08] 生成全排列
来源：http://yw.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://mi.szsharing.cn

PHP:  // 手写递归交换
来源：http://zp.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://jl.hahajie.cn

TS:   // 手写回溯递归
来源：http://ik.szxytkj.cn

Java: // 手写回溯递归
来源：http://pw.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ai.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://vs.hnjuh.cn

C#:   // 手写回溯递归
来源：http://kg.nicolike.cn

[N09] 栈与队列
来源：http://nj.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cv.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lg.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zr.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sh.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ez.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ao.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mi.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fp.nicolike.cn

[N10] 链表节点定义
来源：http://lg.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dr.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eq.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fx.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nk.521024.cn

Java: class Node { int v; Node next; }
来源：http://zy.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pm.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rq.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wm.9csxet.cn

[N11] 二叉树中序遍历
来源：http://uu.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rl.521024.cn

PHP:  // 手写递归函数
来源：http://ok.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ju.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qm.szsharing.cn

Java: // 手写递归
来源：http://ui.shxzukj.cn

Go:   // 手写递归
来源：http://ou.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dc.bjjhwx.cn

C#:   // 手写递归
来源：http://ll.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yp.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fs.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bn.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cm.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tj.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hr.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://go.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ew.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hu.shxzukj.cn

================================================================================
来源：http://rn.jctech888.com.cn

O. 并发与异步
来源：http://bp.hahajie.cn

================================================================================
来源：http://yx.muxihuayi.cn

[O01] 启动一个线程
来源：http://wk.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ed.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eb.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://od.lnxyls.cn

TS:   // 同 JS
来源：http://sm.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ya.colortex.cn

Go:   go f()
来源：http://qo.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://ri.szsharing.cn

C#:   Task.Run(() => F());
来源：http://mo.bjjhwx.cn

[O02] 使用线程池
来源：http://us.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dr.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jr.hahajie.cn

JS:   // worker_threads 线程池
来源：http://jc.nicolike.cn

TS:   // worker_threads 线程池
来源：http://bt.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mc.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rf.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://um.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ze.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://fx.shxzukj.cn

Py:   with lock: shared += 1
来源：http://hp.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://sj.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sh.gzmigu.cn

TS:   // 同 JS
来源：http://id.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://hg.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://op.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vp.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://gy.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://dy.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://ym.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://se.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://wv.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jf.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ai.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ii.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fd.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://lb.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://ed.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://bp.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lv.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://tz.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://ql.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aa.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tt.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://bf.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pq.lnxyls.cn

[O06] 使用进程池
来源：http://at.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ry.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ek.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://vm.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://et.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uk.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qh.huanxung.cn

Ruby: // fork 块
来源：http://fo.shtwfgs.cn

C#:   Parallel.For
来源：http://sm.haigaiapp.cn

================================================================================
来源：http://ky.huixinmuqiang.cn

P. 常用工具函数
来源：http://hl.huanxung.cn

================================================================================
来源：http://wc.9csxet.cn

[P01] 生成 UUID
来源：http://al.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://cz.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rk.huanxung.cn

JS:   crypto.randomUUID()
来源：http://iy.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://yc.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://oz.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://dx.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://hs.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://zo.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://qb.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qp.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rh.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oj.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ih.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fi.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://st.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://to.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wd.newstarts.cn

[P03] 生成短随机字符串
来源：http://gk.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zq.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://br.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://td.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bn.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zo.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kq.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ke.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tf.haigaiapp.cn

[P04] 求长度
来源：http://zt.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lw.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qn.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nk.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rx.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://bo.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://fq.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://lq.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zf.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://tc.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fl.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://od.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rd.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ge.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://za.newstarts.cn

Ruby: a == b
来源：http://ik.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kn.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pj.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jb.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://ms.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cs.newstarts.cn

TS:   if (x == null) {}
来源：http://iv.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rp.hahajie.cn

Go:   if x == nil {}
来源：http://bg.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cu.lnxyls.cn

C#:   if (x is null) {}
来源：http://mv.chemitech.net.cn

[P07] 防抖与节流
来源：http://at.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ho.colortex.cn

PHP:  // 手写时间戳比较
来源：http://pk.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ol.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zx.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qq.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cr.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yo.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ie.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://fl.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://az.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sd.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tx.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pz.521024.cn


<!-- 参考信息 -->