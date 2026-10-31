代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oc.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xw.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://yh.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lh.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://yc.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mj.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nm.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://jl.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://ze.shxzukj.cn

Java: resp.statusCode()
来源：http://ga.shtwfgs.cn

Go:   resp.StatusCode
来源：http://tm.9csxet.cn

Ruby: resp.code.to_i
来源：http://wv.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://nz.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://vx.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bf.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://tu.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ge.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yj.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bh.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fy.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cv.muxihuayi.cn

================================================================================
来源：http://sb.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://to.huanxung.cn

================================================================================
来源：http://dt.bjjhwx.cn

[M01] 读取命令行参数
来源：http://so.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://fb.521024.cn

PHP:  $argv;  $argc;
来源：http://zo.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://ns.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://tl.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://zp.521024.cn

Go:   os.Args[1:]
来源：http://io.lnxyls.cn

Ruby: ARGV
来源：http://dz.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://gx.nicolike.cn

[M02] 读取环境变量
来源：http://zr.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://hl.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jv.szsharing.cn

JS:   process.env.HOME
来源：http://oj.muxihuayi.cn

TS:   process.env.HOME
来源：http://vr.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://pt.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bv.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://mu.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yr.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://jw.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pv.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jz.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gc.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hr.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bh.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yv.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ua.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://mn.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://bq.muxihuayi.cn

Py:   os.getcwd()
来源：http://wh.panjiajie.cn

PHP:  getcwd();
来源：http://td.yuexingan06.cn

JS:   process.cwd()
来源：http://kk.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ya.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://tq.panjiajie.cn

Go:   os.Getwd()
来源：http://bk.szsharing.cn

Ruby: Dir.pwd
来源：http://xg.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://go.gzmigu.cn

[M05] 设置退出码
来源：http://jt.muxihuayi.cn

Py:   sys.exit(1)
来源：http://dd.szsharing.cn

PHP:  exit(1);
来源：http://km.shtwfgs.cn

JS:   process.exit(1)
来源：http://od.colortex.cn

TS:   process.exit(1)
来源：http://jz.521024.cn

Java: System.exit(1)
来源：http://nk.huanxung.cn

Go:   os.Exit(1)
来源：http://pi.nszjky.cn

Ruby: exit 1
来源：http://tt.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fg.shtwfgs.cn

[M06] 向标准错误输出
来源：http://vr.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://nb.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zz.haigaiapp.cn

JS:   console.error("err")
来源：http://hb.hahajie.cn

TS:   console.error("err")
来源：http://ze.bookmarksfly.cn

Java: System.err.println("err")
来源：http://on.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bv.yuntaijiaju.cn

Ruby: warn "err"
来源：http://mg.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://bu.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://xg.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://wo.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dm.yuntaijiaju.cn

JS:   require.main === module
来源：http://ag.szsharing.cn

TS:   require.main === module
来源：http://mn.nszjky.cn

Java: public static void main(String[] args)
来源：http://bb.szsharing.cn

Go:   func main()
来源：http://wu.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bv.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://dc.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://po.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://dk.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ux.hahajie.cn

JS:   process.platform;  process.version
来源：http://du.lnxyls.cn

TS:   process.platform;  process.version
来源：http://lu.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wd.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://np.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kc.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ef.haigaiapp.cn

================================================================================
来源：http://nn.bookmarksfly.cn

N. 数据结构与算法
来源：http://rr.gzmigu.cn

================================================================================
来源：http://iv.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://ml.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fx.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tq.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sn.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://op.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ln.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://pe.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yi.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hs.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ar.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://yt.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cj.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ej.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pc.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ou.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://gz.bjjhwx.cn

Ruby: arr.sort
来源：http://rq.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rw.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://wb.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wu.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://uf.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sc.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ii.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://we.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rh.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://my.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yi.szxytkj.cn

[N04] 斐波那契数列
来源：http://uv.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fm.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://if.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sq.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jp.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kb.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xw.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uf.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://so.yuexingan06.cn

[N05] 最大公约数
来源：http://rv.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://zh.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kt.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sw.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://op.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yh.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://la.newstarts.cn

Ruby: a.gcd(b)
来源：http://qp.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xy.nszjky.cn

[N06] 判断回文字符串
来源：http://ij.panjiajie.cn

Py:   s == s[::-1]
来源：http://lf.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://cu.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://ci.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://an.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jw.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://dl.szsharing.cn

Ruby: s == s.reverse
来源：http://og.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ku.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://rr.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ig.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dd.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ky.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://sy.huixiangedu.cn

Java: // 手写 HashMap
来源：http://fk.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://rd.lnxyls.cn

Ruby: // 手写 Hash
来源：http://sd.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kh.bookmarksfly.cn

[N08] 生成全排列
来源：http://ke.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://rb.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ln.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://gk.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://kc.yuexingan06.cn

Java: // 手写回溯递归
来源：http://il.gzmigu.cn

Go:   // 手写回溯递归
来源：http://ty.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://ro.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://cg.muxihuayi.cn

[N09] 栈与队列
来源：http://fo.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bv.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sx.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zx.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nb.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jb.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ig.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vw.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xv.colortex.cn

[N10] 链表节点定义
来源：http://pt.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dg.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://th.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pd.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uc.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://mi.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mb.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pk.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ym.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://yn.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fb.szsharing.cn

PHP:  // 手写递归函数
来源：http://wq.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mc.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ui.jctech888.com.cn

Java: // 手写递归
来源：http://fk.newstarts.cn

Go:   // 手写递归
来源：http://cz.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://en.panjiajie.cn

C#:   // 手写递归
来源：http://sz.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zh.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tq.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pv.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://at.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jm.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qw.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jc.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rz.wgjwhj.cn

================================================================================
来源：http://yp.haigaiapp.cn

O. 并发与异步
来源：http://vg.asd995.cn

================================================================================
来源：http://nb.hnjuh.cn

[O01] 启动一个线程
来源：http://lo.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cu.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yk.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lf.newstarts.cn

TS:   // 同 JS
来源：http://xd.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://bj.haigaiapp.cn

Go:   go f()
来源：http://eh.nicolike.cn

Ruby: Thread.new { f }
来源：http://rw.521024.cn

C#:   Task.Run(() => F());
来源：http://an.colortex.cn

[O02] 使用线程池
来源：http://hs.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zc.szsharing.cn

JS:   // worker_threads 线程池
来源：http://fm.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://zw.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xa.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ob.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wd.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xq.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://cx.521024.cn

Py:   with lock: shared += 1
来源：http://tj.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://vx.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ex.muxihuayi.cn

TS:   // 同 JS
来源：http://dx.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://mo.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://en.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yi.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://wv.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://jt.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://qs.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nw.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://ne.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wt.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kb.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ak.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ur.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://xd.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://ur.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://ce.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://if.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://cl.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://jx.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ao.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uz.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://pg.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hf.jianghongdianzi.cn

[O06] 使用进程池
来源：http://ug.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ey.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ou.521024.cn

JS:   // child_process / cluster 模块
来源：http://kx.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://uc.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://du.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wm.huanxung.cn

Ruby: // fork 块
来源：http://ey.colortex.cn

C#:   Parallel.For
来源：http://ps.hnjuh.cn

================================================================================
来源：http://zr.jctech888.com.cn

P. 常用工具函数
来源：http://yh.shxzukj.cn

================================================================================
来源：http://zk.521024.cn

[P01] 生成 UUID
来源：http://ma.521024.cn

Py:   str(uuid.uuid4())
来源：http://op.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yh.newstarts.cn

JS:   crypto.randomUUID()
来源：http://rk.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ju.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://dm.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://hd.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://nl.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://fi.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://vh.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dn.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ih.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gu.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dy.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ol.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://su.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oe.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fr.szsharing.cn

[P03] 生成短随机字符串
来源：http://ou.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ud.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qo.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xj.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bl.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ab.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://st.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lz.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pz.asd995.cn

[P04] 求长度
来源：http://gg.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://av.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://de.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ma.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hp.nicolike.cn


<!-- 参考信息 -->