代发 wailian999

Ruby: ARGV
来源：http://mp.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://nm.colortex.cn

[M02] 读取环境变量
来源：http://vf.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://rx.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ww.yuexingan06.cn

JS:   process.env.HOME
来源：http://qo.shtwfgs.cn

TS:   process.env.HOME
来源：http://tu.521024.cn

Java: System.getenv("HOME")
来源：http://mb.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vp.szsharing.cn

Ruby: ENV["HOME"]
来源：http://xl.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rg.nszjky.cn

[M03] 执行外部命令
来源：http://bp.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mk.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ce.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qg.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ml.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vx.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bs.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://po.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://ui.gzmigu.cn

[M04] 获取当前工作目录
来源：http://wc.nszjky.cn

Py:   os.getcwd()
来源：http://xd.jianghongdianzi.cn

PHP:  getcwd();
来源：http://cz.hnjuh.cn

JS:   process.cwd()
来源：http://ue.hahajie.cn

TS:   process.cwd()
来源：http://sv.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://qs.bookmarksfly.cn

Go:   os.Getwd()
来源：http://co.shtwfgs.cn

Ruby: Dir.pwd
来源：http://am.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qz.shxzskj.cn

[M05] 设置退出码
来源：http://wc.panjiajie.cn

Py:   sys.exit(1)
来源：http://nf.newstarts.cn

PHP:  exit(1);
来源：http://qp.nszjky.cn

JS:   process.exit(1)
来源：http://lo.huixiangedu.cn

TS:   process.exit(1)
来源：http://nh.asd995.cn

Java: System.exit(1)
来源：http://uc.haigaiapp.cn

Go:   os.Exit(1)
来源：http://lr.9csxet.cn

Ruby: exit 1
来源：http://xd.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yw.gzmigu.cn

[M06] 向标准错误输出
来源：http://kg.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://kd.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ma.jctech888.com.cn

JS:   console.error("err")
来源：http://lm.chemitech.net.cn

TS:   console.error("err")
来源：http://fr.bookmarksfly.cn

Java: System.err.println("err")
来源：http://oy.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kr.yuexingan06.cn

Ruby: warn "err"
来源：http://xb.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://sn.nszjky.cn

[M07] 判断是否为主入口
来源：http://oj.asd995.cn

Py:   if __name__ == "__main__":
来源：http://ln.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ka.huanxung.cn

JS:   require.main === module
来源：http://su.gzmigu.cn

TS:   require.main === module
来源：http://jd.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://wh.asd995.cn

Go:   func main()
来源：http://gd.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vs.521024.cn

C#:   static void Main(string[] args)
来源：http://gh.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://hf.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://zj.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://uz.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ax.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ni.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pn.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qb.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oi.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fh.haigaiapp.cn

================================================================================
来源：http://ey.huixiangedu.cn

N. 数据结构与算法
来源：http://bq.hahajie.cn

================================================================================
来源：http://bt.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://pg.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xr.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://no.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qj.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pr.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://ah.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://db.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pp.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://wu.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kp.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ho.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qn.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mf.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qw.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://tk.shxzukj.cn

Ruby: arr.sort
来源：http://jq.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pu.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://ri.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ky.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://vj.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cw.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pp.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ov.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pd.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oh.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qy.hnjuh.cn

[N04] 斐波那契数列
来源：http://fv.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ys.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iw.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yk.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xp.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ns.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nt.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://je.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://co.haigaiapp.cn

[N05] 最大公约数
来源：http://ph.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://ih.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fe.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xi.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cx.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cw.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vo.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://hh.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ng.asd995.cn

[N06] 判断回文字符串
来源：http://vu.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ak.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://ub.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ix.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://xh.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://il.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://jz.lnxyls.cn

Ruby: s == s.reverse
来源：http://ws.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wj.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://bv.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zr.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yr.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ye.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://gm.chemitech.net.cn

Java: // 手写 HashMap
来源：http://oc.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://vh.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://cc.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yn.huixiangedu.cn

[N08] 生成全排列
来源：http://it.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://vq.huanxung.cn

PHP:  // 手写递归交换
来源：http://tz.hnjuh.cn

JS:   // 手写回溯递归
来源：http://gg.hnjuh.cn

TS:   // 手写回溯递归
来源：http://fs.wgjwhj.cn

Java: // 手写回溯递归
来源：http://mv.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://dp.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://ho.hnjuh.cn

C#:   // 手写回溯递归
来源：http://gu.yuntaijiaju.cn

[N09] 栈与队列
来源：http://kg.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ep.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dg.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jw.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sz.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://af.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fu.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://us.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://br.hnjuh.cn

[N10] 链表节点定义
来源：http://mn.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lx.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ne.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nq.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sj.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://ot.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ae.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://is.colortex.cn

[N11] 二叉树中序遍历
来源：http://ty.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cu.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://kr.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fv.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xb.shxzskj.cn

Java: // 手写递归
来源：http://mb.shxzukj.cn

Go:   // 手写递归
来源：http://hj.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ru.huanxung.cn

C#:   // 手写递归
来源：http://hg.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zt.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kv.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eh.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mf.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jp.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mg.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aq.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dj.hnjuh.cn

================================================================================
来源：http://qt.bookmarksfly.cn

O. 并发与异步
来源：http://tv.gzmigu.cn

================================================================================
来源：http://wh.9csxet.cn

[O01] 启动一个线程
来源：http://dj.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tn.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://od.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dy.lnxyls.cn

TS:   // 同 JS
来源：http://jp.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://tn.panjiajie.cn

Go:   go f()
来源：http://es.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://xl.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://lh.shxzukj.cn

[O02] 使用线程池
来源：http://nx.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jh.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fm.nszjky.cn

JS:   // worker_threads 线程池
来源：http://ry.521024.cn

TS:   // worker_threads 线程池
来源：http://ls.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ce.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://by.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nc.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ls.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://xn.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://jz.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://iw.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aq.huanxung.cn

TS:   // 同 JS
来源：http://ry.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://jq.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qq.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ce.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://er.nicolike.cn

[O04] 定义异步函数并等待
来源：http://ae.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://qi.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zo.hahajie.cn

JS:   async function f() { await g(); }
来源：http://uf.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tg.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jx.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lj.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bw.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://rt.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://wg.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ff.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yg.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://dr.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://ud.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zt.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mt.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://kx.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tl.shtwfgs.cn

[O06] 使用进程池
来源：http://nu.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ao.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ds.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://ue.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://wu.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://js.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jk.newstarts.cn

Ruby: // fork 块
来源：http://id.yuntaijiaju.cn

C#:   Parallel.For
来源：http://ew.huixinmuqiang.cn

================================================================================
来源：http://rx.huixiangedu.cn

P. 常用工具函数
来源：http://gw.nicolike.cn

================================================================================
来源：http://rq.shxzskj.cn

[P01] 生成 UUID
来源：http://fs.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://in.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zi.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://tc.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://yo.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://pm.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://hs.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://cx.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://rl.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://ek.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ga.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mp.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qn.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ko.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sm.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qh.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xo.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tj.colortex.cn

[P03] 生成短随机字符串
来源：http://hq.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hj.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xk.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sm.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fs.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dm.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mp.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nb.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rr.bookmarksfly.cn

[P04] 求长度
来源：http://yd.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ex.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rl.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bg.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ky.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://bz.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://lv.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://fk.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vu.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ip.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://te.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mk.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ts.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zq.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kx.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vh.huixiangedu.cn

Ruby: a == b
来源：http://kg.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vd.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oa.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kj.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://fb.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qb.chemitech.net.cn

TS:   if (x == null) {}
来源：http://bt.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gq.nszjky.cn

Go:   if x == nil {}
来源：http://sg.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jh.shxzskj.cn

C#:   if (x is null) {}
来源：http://yx.9csxet.cn

[P07] 防抖与节流
来源：http://bj.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gc.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://qs.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gr.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://so.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ew.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vk.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ef.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://in.9csxet.cn

[P08] 处理浮点精度问题
来源：http://zs.huixinmuqiang.cn


<!-- 参考信息 -->