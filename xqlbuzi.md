代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lb.huanxung.cn

JS:   process.env.HOME
来源：http://vg.shxzukj.cn

TS:   process.env.HOME
来源：http://lv.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ve.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wc.szsharing.cn

Ruby: ENV["HOME"]
来源：http://jw.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gz.haigaiapp.cn

[M03] 执行外部命令
来源：http://mn.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kd.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cg.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ok.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vm.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ht.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kb.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mx.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://hh.colortex.cn

[M04] 获取当前工作目录
来源：http://un.521024.cn

Py:   os.getcwd()
来源：http://kt.haigaiapp.cn

PHP:  getcwd();
来源：http://wy.newstarts.cn

JS:   process.cwd()
来源：http://qd.bjjhwx.cn

TS:   process.cwd()
来源：http://we.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qr.szsharing.cn

Go:   os.Getwd()
来源：http://el.panjiajie.cn

Ruby: Dir.pwd
来源：http://wl.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://os.jianghongdianzi.cn

[M05] 设置退出码
来源：http://sj.shtwfgs.cn

Py:   sys.exit(1)
来源：http://fj.colortex.cn

PHP:  exit(1);
来源：http://cf.nicolike.cn

JS:   process.exit(1)
来源：http://ko.nszjky.cn

TS:   process.exit(1)
来源：http://rl.yuexingan06.cn

Java: System.exit(1)
来源：http://kb.nicolike.cn

Go:   os.Exit(1)
来源：http://jn.muxihuayi.cn

Ruby: exit 1
来源：http://pc.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rx.newstarts.cn

[M06] 向标准错误输出
来源：http://wm.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://co.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kl.huixiangedu.cn

JS:   console.error("err")
来源：http://ju.wgjwhj.cn

TS:   console.error("err")
来源：http://xc.bjjhwx.cn

Java: System.err.println("err")
来源：http://sp.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ol.9csxet.cn

Ruby: warn "err"
来源：http://qg.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://eo.huanxung.cn

[M07] 判断是否为主入口
来源：http://tk.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://he.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oa.yuntaijiaju.cn

JS:   require.main === module
来源：http://mq.nszjky.cn

TS:   require.main === module
来源：http://kg.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://gk.9csxet.cn

Go:   func main()
来源：http://bd.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rk.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://hx.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://sg.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ba.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://tn.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://eu.hnjuh.cn

TS:   process.platform;  process.version
来源：http://ua.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ne.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ky.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sa.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uc.jianghongdianzi.cn

================================================================================
来源：http://zt.shxzukj.cn

N. 数据结构与算法
来源：http://js.shxzskj.cn

================================================================================
来源：http://xu.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://kj.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kp.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ha.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oc.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pe.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kq.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ef.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qi.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qv.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://uv.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://kh.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oz.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dj.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yy.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bo.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://jy.newstarts.cn

Ruby: arr.sort
来源：http://zn.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://to.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://cu.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://it.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ym.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://td.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oj.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yy.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xm.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ov.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ei.newstarts.cn

[N04] 斐波那契数列
来源：http://st.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qg.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nt.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lv.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tj.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ts.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dw.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gh.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hr.nicolike.cn

[N05] 最大公约数
来源：http://yi.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://xi.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yu.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lz.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ss.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mf.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cg.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://db.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ih.hnjuh.cn

[N06] 判断回文字符串
来源：http://ui.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://nv.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://nt.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://lb.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://la.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ja.521024.cn

Go:   // 双指针从两端比较
来源：http://ty.nicolike.cn

Ruby: s == s.reverse
来源：http://qt.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lp.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://xc.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xs.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ma.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nt.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://yo.hnjuh.cn

Java: // 手写 HashMap
来源：http://bb.szsharing.cn

Go:   // 手写 map[int]int
来源：http://ry.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://fe.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fl.huixinmuqiang.cn

[N08] 生成全排列
来源：http://li.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://ue.shxzskj.cn

PHP:  // 手写递归交换
来源：http://pa.9csxet.cn

JS:   // 手写回溯递归
来源：http://ku.nszjky.cn

TS:   // 手写回溯递归
来源：http://zu.colortex.cn

Java: // 手写回溯递归
来源：http://qc.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ou.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ig.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://lg.hahajie.cn

[N09] 栈与队列
来源：http://rx.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bq.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ik.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ox.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dl.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ha.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kv.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xr.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://va.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://zg.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ax.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://de.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lq.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jc.asd995.cn

Java: class Node { int v; Node next; }
来源：http://wb.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ec.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hj.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ah.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://xm.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rp.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://jf.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://of.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sy.huixinmuqiang.cn

Java: // 手写递归
来源：http://wa.bjjhwx.cn

Go:   // 手写递归
来源：http://ks.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xh.9csxet.cn

C#:   // 手写递归
来源：http://sr.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kc.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nx.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://px.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lx.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qf.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bs.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fe.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yo.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bd.521024.cn

================================================================================
来源：http://ho.bjjhwx.cn

O. 并发与异步
来源：http://dp.szsharing.cn

================================================================================
来源：http://md.bjjhwx.cn

[O01] 启动一个线程
来源：http://be.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zb.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mk.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fl.nszjky.cn

TS:   // 同 JS
来源：http://xg.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://yw.szsharing.cn

Go:   go f()
来源：http://px.nszjky.cn

Ruby: Thread.new { f }
来源：http://zt.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://wn.wgjwhj.cn

[O02] 使用线程池
来源：http://tt.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ye.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ah.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://gv.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://sl.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cc.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vn.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ka.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hi.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://qp.nicolike.cn

Py:   with lock: shared += 1
来源：http://yk.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://wn.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fn.bjjhwx.cn

TS:   // 同 JS
来源：http://uq.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://rc.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lr.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cb.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://yt.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://sg.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://vw.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fi.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://cw.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gr.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pm.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ik.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mp.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://ty.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://jh.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://og.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kq.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://mb.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://cp.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ek.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cc.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://ly.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tx.muxihuayi.cn

[O06] 使用进程池
来源：http://wu.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bp.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jw.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://le.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://tb.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ou.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nu.wgjwhj.cn

Ruby: // fork 块
来源：http://fg.wgjwhj.cn

C#:   Parallel.For
来源：http://tu.szsharing.cn

================================================================================
来源：http://fz.newstarts.cn

P. 常用工具函数
来源：http://lz.shtwfgs.cn

================================================================================
来源：http://vj.yuexingan06.cn

[P01] 生成 UUID
来源：http://wu.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://hj.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qc.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://pf.colortex.cn

TS:   crypto.randomUUID()
来源：http://bq.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://zh.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://zm.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://cg.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://vt.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://ru.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wd.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uc.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jw.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ps.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oy.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ay.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mq.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qo.shxzskj.cn

[P03] 生成短随机字符串
来源：http://gr.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ig.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dg.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vg.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xu.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zc.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bt.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qp.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pb.wgjwhj.cn

[P04] 求长度
来源：http://yx.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kh.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://px.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vb.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pp.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://hm.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://qa.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://uv.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://du.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://cg.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://az.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wv.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zb.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cc.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gz.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vh.shxzukj.cn

Ruby: a == b
来源：http://uy.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fz.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mr.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oh.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://hp.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fa.chemitech.net.cn

TS:   if (x == null) {}
来源：http://co.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gp.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://jt.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://za.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://je.haigaiapp.cn

[P07] 防抖与节流
来源：http://sl.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mq.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://ee.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jj.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oi.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ug.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ym.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jd.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ap.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://pq.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gz.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dn.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jg.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://io.haigaiapp.cn


<!-- 参考信息 -->