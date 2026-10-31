代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sg.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gf.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://iq.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hd.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://op.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tb.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://su.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://hn.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://vd.bookmarksfly.cn

Java: resp.statusCode()
来源：http://tc.wgjwhj.cn

Go:   resp.StatusCode
来源：http://ac.panjiajie.cn

Ruby: resp.code.to_i
来源：http://cj.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://hs.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://ct.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wj.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://tv.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hr.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ez.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cm.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eb.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pf.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vb.bookmarksfly.cn

================================================================================
来源：http://du.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://sz.nicolike.cn

================================================================================
来源：http://cn.hahajie.cn

[M01] 读取命令行参数
来源：http://pb.asd995.cn

Py:   sys.argv[1:]
来源：http://xs.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ip.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://jb.huanxung.cn

TS:   process.argv.slice(2)
来源：http://to.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://id.wgjwhj.cn

Go:   os.Args[1:]
来源：http://jr.9csxet.cn

Ruby: ARGV
来源：http://dz.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://zk.lnxyls.cn

[M02] 读取环境变量
来源：http://ra.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://qn.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qq.newstarts.cn

JS:   process.env.HOME
来源：http://nd.bjjhwx.cn

TS:   process.env.HOME
来源：http://af.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://qp.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kd.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://pw.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yp.haigaiapp.cn

[M03] 执行外部命令
来源：http://cd.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ii.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wm.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cw.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lg.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://by.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fn.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lg.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://hw.nicolike.cn

[M04] 获取当前工作目录
来源：http://ia.yuexingan06.cn

Py:   os.getcwd()
来源：http://eb.bookmarksfly.cn

PHP:  getcwd();
来源：http://rq.haigaiapp.cn

JS:   process.cwd()
来源：http://ln.yuexingan06.cn

TS:   process.cwd()
来源：http://rg.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://ik.shxzskj.cn

Go:   os.Getwd()
来源：http://xe.yuexingan06.cn

Ruby: Dir.pwd
来源：http://zy.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tf.hnjuh.cn

[M05] 设置退出码
来源：http://rp.huanxung.cn

Py:   sys.exit(1)
来源：http://mj.asd995.cn

PHP:  exit(1);
来源：http://ks.hnjuh.cn

JS:   process.exit(1)
来源：http://uk.panjiajie.cn

TS:   process.exit(1)
来源：http://ri.shtwfgs.cn

Java: System.exit(1)
来源：http://mn.shtwfgs.cn

Go:   os.Exit(1)
来源：http://kg.asd995.cn

Ruby: exit 1
来源：http://ob.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kb.szsharing.cn

[M06] 向标准错误输出
来源：http://kz.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ra.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gq.hahajie.cn

JS:   console.error("err")
来源：http://rb.huanxung.cn

TS:   console.error("err")
来源：http://mz.nszjky.cn

Java: System.err.println("err")
来源：http://im.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://co.shtwfgs.cn

Ruby: warn "err"
来源：http://bx.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://pt.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://rc.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ak.szxytkj.cn

JS:   require.main === module
来源：http://ee.9csxet.cn

TS:   require.main === module
来源：http://mx.9csxet.cn

Java: public static void main(String[] args)
来源：http://yo.lnxyls.cn

Go:   func main()
来源：http://br.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ie.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://eu.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://wc.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://ri.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ui.szxytkj.cn

TS:   process.platform;  process.version
来源：http://za.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fi.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mh.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vg.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sh.shtwfgs.cn

================================================================================
来源：http://xw.yuntaijiaju.cn

N. 数据结构与算法
来源：http://jz.lnxyls.cn

================================================================================
来源：http://aa.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://yy.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yh.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gc.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ai.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bf.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jz.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://fg.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lj.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wp.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://pw.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kw.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://un.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fy.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hl.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://xo.nszjky.cn

Ruby: arr.sort
来源：http://iw.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yi.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://xb.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pq.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://vq.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://su.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lr.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fp.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wj.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sg.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rx.muxihuayi.cn

[N04] 斐波那契数列
来源：http://uf.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ui.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gp.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xh.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wh.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cp.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qw.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ct.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://av.hnjuh.cn

[N05] 最大公约数
来源：http://vi.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://gg.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yf.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tn.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gj.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ii.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://up.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://ga.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kk.shtwfgs.cn

[N06] 判断回文字符串
来源：http://uu.hahajie.cn

Py:   s == s[::-1]
来源：http://jv.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://my.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://bx.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://kz.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://za.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://zl.newstarts.cn

Ruby: s == s.reverse
来源：http://ks.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fh.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://fm.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ng.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fi.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yo.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://tz.nicolike.cn

Java: // 手写 HashMap
来源：http://qt.huanxung.cn

Go:   // 手写 map[int]int
来源：http://pe.nszjky.cn

Ruby: // 手写 Hash
来源：http://ld.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zw.asd995.cn

[N08] 生成全排列
来源：http://km.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://zx.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ng.gzmigu.cn

JS:   // 手写回溯递归
来源：http://gh.gzmigu.cn

TS:   // 手写回溯递归
来源：http://zv.9csxet.cn

Java: // 手写回溯递归
来源：http://gf.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://bo.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ba.nicolike.cn

C#:   // 手写回溯递归
来源：http://jw.haigaiapp.cn

[N09] 栈与队列
来源：http://au.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ys.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wv.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tx.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cc.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://br.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://id.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ku.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rq.colortex.cn

[N10] 链表节点定义
来源：http://cj.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lh.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hf.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sw.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dw.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://ra.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ta.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tz.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fj.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://zs.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rc.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://qr.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://md.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eh.asd995.cn

Java: // 手写递归
来源：http://tu.shxzukj.cn

Go:   // 手写递归
来源：http://hn.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xu.huanxung.cn

C#:   // 手写递归
来源：http://hd.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sn.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rk.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kw.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xe.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eg.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yh.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fj.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eu.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hr.521024.cn

================================================================================
来源：http://wg.huixinmuqiang.cn

O. 并发与异步
来源：http://fo.huanxung.cn

================================================================================
来源：http://po.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ui.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://at.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tj.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eb.wgjwhj.cn

TS:   // 同 JS
来源：http://ms.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://pv.wgjwhj.cn

Go:   go f()
来源：http://ym.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://mf.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://jj.shtwfgs.cn

[O02] 使用线程池
来源：http://wt.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ho.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iz.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://aw.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://xt.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ie.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xp.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kk.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://it.szsharing.cn

[O03] 加锁保护共享数据
来源：http://th.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://ii.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qa.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gu.bjjhwx.cn

TS:   // 同 JS
来源：http://mq.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ke.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jw.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ct.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://qn.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://ri.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://ws.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nt.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://ba.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fj.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ws.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zj.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qn.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://kr.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://ee.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://dk.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cm.asd995.cn

JS:   await Promise.all(tasks)
来源：http://kw.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://re.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ru.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://io.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://ze.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xx.huixiangedu.cn

[O06] 使用进程池
来源：http://gv.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ls.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ee.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://lx.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://kj.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mg.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cr.chemitech.net.cn

Ruby: // fork 块
来源：http://dt.newstarts.cn

C#:   Parallel.For
来源：http://ka.yuexingan06.cn

================================================================================
来源：http://xp.shtwfgs.cn

P. 常用工具函数
来源：http://ve.hnjuh.cn

================================================================================
来源：http://yn.yuexingan06.cn

[P01] 生成 UUID
来源：http://tu.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://go.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jq.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://lc.colortex.cn

TS:   crypto.randomUUID()
来源：http://jy.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://fs.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://rw.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://lc.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://yj.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://er.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kx.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tk.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://et.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cr.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rl.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fi.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lz.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://or.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ca.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://id.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pn.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lo.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fv.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qd.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://za.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://et.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pn.gzmigu.cn

[P04] 求长度
来源：http://kc.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://li.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ac.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fk.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xm.521024.cn


<!-- 参考信息 -->