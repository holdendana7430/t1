代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ci.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hd.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ny.hahajie.cn

[L06] 解析响应为 JSON
来源：http://td.colortex.cn

Py:   resp.json()
来源：http://xl.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://rp.yuexingan06.cn

JS:   await resp.json()
来源：http://eo.newstarts.cn

TS:   await resp.json()
来源：http://hs.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kd.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uc.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://fc.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fc.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://lg.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qi.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pw.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ns.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://hm.chemitech.net.cn

Java: resp.statusCode()
来源：http://ne.newstarts.cn

Go:   resp.StatusCode
来源：http://bu.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://em.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://mo.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://zx.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://br.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://ma.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mh.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qq.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vr.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yz.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wm.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nu.hnjuh.cn

================================================================================
来源：http://rp.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://jr.hahajie.cn

================================================================================
来源：http://dk.muxihuayi.cn

[M01] 读取命令行参数
来源：http://mi.gzmigu.cn

Py:   sys.argv[1:]
来源：http://ha.521024.cn

PHP:  $argv;  $argc;
来源：http://te.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://jo.521024.cn

TS:   process.argv.slice(2)
来源：http://sn.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://ly.huanxung.cn

Go:   os.Args[1:]
来源：http://zr.jctech888.com.cn

Ruby: ARGV
来源：http://gm.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ff.asd995.cn

[M02] 读取环境变量
来源：http://kk.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://ri.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hv.haigaiapp.cn

JS:   process.env.HOME
来源：http://wo.colortex.cn

TS:   process.env.HOME
来源：http://jr.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://dl.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zl.nszjky.cn

Ruby: ENV["HOME"]
来源：http://je.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jt.colortex.cn

[M03] 执行外部命令
来源：http://ph.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://go.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://de.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://te.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sj.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tg.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://do.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cv.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://eo.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://xq.szsharing.cn

Py:   os.getcwd()
来源：http://om.521024.cn

PHP:  getcwd();
来源：http://rp.haigaiapp.cn

JS:   process.cwd()
来源：http://zb.panjiajie.cn

TS:   process.cwd()
来源：http://wh.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://co.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://fk.huixiangedu.cn

Ruby: Dir.pwd
来源：http://vs.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yc.jctech888.com.cn

[M05] 设置退出码
来源：http://kc.haigaiapp.cn

Py:   sys.exit(1)
来源：http://fp.shtwfgs.cn

PHP:  exit(1);
来源：http://nn.huixiangedu.cn

JS:   process.exit(1)
来源：http://ae.wgjwhj.cn

TS:   process.exit(1)
来源：http://rk.chemitech.net.cn

Java: System.exit(1)
来源：http://fc.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://dg.wgjwhj.cn

Ruby: exit 1
来源：http://ru.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.huanxung.cn

[M06] 向标准错误输出
来源：http://zz.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://tc.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rj.huanxung.cn

JS:   console.error("err")
来源：http://xt.shxzukj.cn

TS:   console.error("err")
来源：http://uk.szsharing.cn

Java: System.err.println("err")
来源：http://qv.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tm.jianghongdianzi.cn

Ruby: warn "err"
来源：http://tq.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://yr.9csxet.cn

[M07] 判断是否为主入口
来源：http://mc.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://ia.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lo.newstarts.cn

JS:   require.main === module
来源：http://px.nicolike.cn

TS:   require.main === module
来源：http://pu.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://fq.shxzukj.cn

Go:   func main()
来源：http://hk.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oz.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://hm.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://it.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://yi.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://mj.shxzukj.cn

JS:   process.platform;  process.version
来源：http://ei.szsharing.cn

TS:   process.platform;  process.version
来源：http://sm.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ct.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qz.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tm.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ds.gzmigu.cn

================================================================================
来源：http://wb.bjjhwx.cn

N. 数据结构与算法
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://rh.521024.cn

[N01] 二分查找（有序数组）
来源：http://rb.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yo.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ol.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fd.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xk.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ar.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ff.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ku.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yr.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://dx.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hf.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aa.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://er.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jc.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://vq.huanxung.cn

Ruby: arr.sort
来源：http://wx.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rp.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://is.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eg.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://lp.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yu.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jn.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ji.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mi.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ej.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wx.nicolike.cn

[N04] 斐波那契数列
来源：http://hu.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uj.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wj.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ab.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://og.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wu.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pe.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bn.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nu.hnjuh.cn

[N05] 最大公约数
来源：http://wn.szsharing.cn

Py:   math.gcd(a, b)
来源：http://az.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yj.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://az.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fj.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://va.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yf.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://or.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://py.hnjuh.cn

[N06] 判断回文字符串
来源：http://qa.haigaiapp.cn

Py:   s == s[::-1]
来源：http://mo.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://lk.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://aj.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://nl.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mu.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://zm.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ci.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fq.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://fj.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xo.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oz.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iw.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://dh.shtwfgs.cn

Java: // 手写 HashMap
来源：http://iw.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://wt.nicolike.cn

Ruby: // 手写 Hash
来源：http://ff.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nz.wgjwhj.cn

[N08] 生成全排列
来源：http://kk.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ws.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://nq.521024.cn

JS:   // 手写回溯递归
来源：http://hl.newstarts.cn

TS:   // 手写回溯递归
来源：http://lg.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://pk.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://vp.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://hj.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://ca.yuexingan06.cn

[N09] 栈与队列
来源：http://nn.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://if.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hw.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ad.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pg.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oz.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pl.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tl.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kw.shxzukj.cn

[N10] 链表节点定义
来源：http://ei.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zb.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qw.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aa.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://os.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://na.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hl.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ye.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sn.asd995.cn

[N11] 二叉树中序遍历
来源：http://ak.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lw.521024.cn

PHP:  // 手写递归函数
来源：http://al.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dj.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ev.huixinmuqiang.cn

Java: // 手写递归
来源：http://uc.gzmigu.cn

Go:   // 手写递归
来源：http://wk.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://et.colortex.cn

C#:   // 手写递归
来源：http://fz.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lu.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nl.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mx.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xc.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kh.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wr.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rf.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hn.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gv.yuexingan06.cn

================================================================================
来源：http://lk.bjjhwx.cn

O. 并发与异步
来源：http://wz.hahajie.cn

================================================================================
来源：http://br.chemitech.net.cn

[O01] 启动一个线程
来源：http://aa.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bd.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oc.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ao.huixiangedu.cn

TS:   // 同 JS
来源：http://uo.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://fx.shtwfgs.cn

Go:   go f()
来源：http://wz.gzmigu.cn

Ruby: Thread.new { f }
来源：http://ko.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://ft.huixiangedu.cn

[O02] 使用线程池
来源：http://gs.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xw.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cv.szsharing.cn

JS:   // worker_threads 线程池
来源：http://hw.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://hq.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zf.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qy.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jp.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xj.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://aq.szsharing.cn

Py:   with lock: shared += 1
来源：http://ia.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://hg.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yw.panjiajie.cn

TS:   // 同 JS
来源：http://rw.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://cf.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nq.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://va.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://vb.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://cl.colortex.cn

Py:   async def f():⏎    await g()
来源：http://lw.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tu.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://zo.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gl.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iq.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wg.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://et.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://ri.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://jb.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://lw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://om.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://vn.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://gg.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ri.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bd.huanxung.cn

Ruby: threads.map(&:join)
来源：http://hg.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vs.521024.cn

[O06] 使用进程池
来源：http://tj.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://am.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rv.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://cs.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://li.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xu.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://os.shxzukj.cn

Ruby: // fork 块
来源：http://cs.nicolike.cn

C#:   Parallel.For
来源：http://ts.521024.cn

================================================================================
来源：http://hp.muxihuayi.cn

P. 常用工具函数
来源：http://gq.yuexingan06.cn

================================================================================
来源：http://aj.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://mq.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://mo.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ne.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://du.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://ms.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://rr.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://wm.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://nq.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://kq.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://xb.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ol.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tj.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://up.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lx.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fr.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zw.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://br.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ug.szxytkj.cn

[P03] 生成短随机字符串
来源：http://lr.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pm.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xa.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ar.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ya.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qa.yuntaijiaju.cn


<!-- 参考信息 -->