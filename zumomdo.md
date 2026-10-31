代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ao.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://th.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ly.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ed.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uu.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eu.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ve.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xv.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ae.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oc.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ph.asd995.cn

[L06] 解析响应为 JSON
来源：http://ut.huixinmuqiang.cn

Py:   resp.json()
来源：http://vv.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://ei.asd995.cn

JS:   await resp.json()
来源：http://cp.asd995.cn

TS:   await resp.json()
来源：http://ow.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zu.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://va.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://yt.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lu.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://nn.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ub.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ad.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://eh.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://pt.muxihuayi.cn

Java: resp.statusCode()
来源：http://dt.nszjky.cn

Go:   resp.StatusCode
来源：http://we.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://fa.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://pu.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://vl.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ke.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://zv.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fl.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lj.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://is.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ni.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://er.hnjuh.cn

================================================================================
来源：http://kv.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://cm.szxytkj.cn

================================================================================
来源：http://yf.szxytkj.cn

[M01] 读取命令行参数
来源：http://rk.lnxyls.cn

Py:   sys.argv[1:]
来源：http://bj.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://cj.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://vr.nicolike.cn

TS:   process.argv.slice(2)
来源：http://qe.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://xq.huanxung.cn

Go:   os.Args[1:]
来源：http://tn.newstarts.cn

Ruby: ARGV
来源：http://ny.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://yi.panjiajie.cn

[M02] 读取环境变量
来源：http://dz.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://ru.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sv.haigaiapp.cn

JS:   process.env.HOME
来源：http://qw.521024.cn

TS:   process.env.HOME
来源：http://tn.lnxyls.cn

Java: System.getenv("HOME")
来源：http://wm.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vs.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ek.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ap.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://xo.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hp.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mh.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qf.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tp.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fk.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bq.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jz.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://by.shxzukj.cn

[M04] 获取当前工作目录
来源：http://te.huanxung.cn

Py:   os.getcwd()
来源：http://jv.muxihuayi.cn

PHP:  getcwd();
来源：http://rc.huanxung.cn

JS:   process.cwd()
来源：http://hr.bjjhwx.cn

TS:   process.cwd()
来源：http://vz.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ky.521024.cn

Go:   os.Getwd()
来源：http://uy.szxytkj.cn

Ruby: Dir.pwd
来源：http://mu.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://so.chemitech.net.cn

[M05] 设置退出码
来源：http://tn.newstarts.cn

Py:   sys.exit(1)
来源：http://yb.asd995.cn

PHP:  exit(1);
来源：http://zn.huixiangedu.cn

JS:   process.exit(1)
来源：http://dz.bjjhwx.cn

TS:   process.exit(1)
来源：http://ku.shtwfgs.cn

Java: System.exit(1)
来源：http://eu.hnjuh.cn

Go:   os.Exit(1)
来源：http://nk.chemitech.net.cn

Ruby: exit 1
来源：http://tx.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ek.bjjhwx.cn

[M06] 向标准错误输出
来源：http://zw.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://pl.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wx.huixinmuqiang.cn

JS:   console.error("err")
来源：http://vv.yuexingan06.cn

TS:   console.error("err")
来源：http://bi.wgjwhj.cn

Java: System.err.println("err")
来源：http://it.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ws.hnjuh.cn

Ruby: warn "err"
来源：http://qp.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://pn.lnxyls.cn

[M07] 判断是否为主入口
来源：http://tk.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://zn.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bf.shtwfgs.cn

JS:   require.main === module
来源：http://rz.huanxung.cn

TS:   require.main === module
来源：http://mg.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://la.yuntaijiaju.cn

Go:   func main()
来源：http://im.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pp.9csxet.cn

C#:   static void Main(string[] args)
来源：http://ek.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://bk.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ff.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://pf.gzmigu.cn

JS:   process.platform;  process.version
来源：http://xr.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://dr.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dz.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yi.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eg.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ba.jianghongdianzi.cn

================================================================================
来源：http://oq.jianghongdianzi.cn

N. 数据结构与算法
来源：http://ye.asd995.cn

================================================================================
来源：http://pq.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://eg.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ce.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sr.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iv.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ki.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pr.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://va.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fx.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://an.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://kl.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wk.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ao.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ca.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://om.colortex.cn

Go:   slices.Sort(arr)
来源：http://kv.521024.cn

Ruby: arr.sort
来源：http://pi.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ir.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://qt.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qn.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://nz.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oq.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qk.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://io.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xp.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fu.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zk.shxzskj.cn

[N04] 斐波那契数列
来源：http://fv.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oe.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ex.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qz.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://te.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cp.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wz.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xa.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ln.shxzukj.cn

[N05] 最大公约数
来源：http://rk.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://sw.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fs.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vg.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fd.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dn.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://re.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://de.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pg.shtwfgs.cn

[N06] 判断回文字符串
来源：http://as.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ca.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://qv.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://rt.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://du.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lc.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ko.newstarts.cn

Ruby: s == s.reverse
来源：http://gb.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aw.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://qq.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jl.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cy.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yv.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://wz.shxzukj.cn

Java: // 手写 HashMap
来源：http://hh.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://wy.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://ms.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mz.nicolike.cn

[N08] 生成全排列
来源：http://bl.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://cf.huanxung.cn

PHP:  // 手写递归交换
来源：http://jz.shxzskj.cn

JS:   // 手写回溯递归
来源：http://wb.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://va.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://qn.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ku.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://rn.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://go.nszjky.cn

[N09] 栈与队列
来源：http://bc.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yf.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tg.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://af.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wq.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wt.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zn.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gq.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sz.colortex.cn

[N10] 链表节点定义
来源：http://is.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ek.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wk.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gs.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://at.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://hx.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iw.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gm.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lw.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://uv.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ty.szxytkj.cn

PHP:  // 手写递归函数
来源：http://wl.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rc.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xm.shxzskj.cn

Java: // 手写递归
来源：http://yj.chemitech.net.cn

Go:   // 手写递归
来源：http://zr.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eb.nicolike.cn

C#:   // 手写递归
来源：http://nh.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://my.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bq.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yq.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fl.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xo.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hw.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dc.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iq.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://az.huanxung.cn

================================================================================
来源：http://bl.shtwfgs.cn

O. 并发与异步
来源：http://du.yuntaijiaju.cn

================================================================================
来源：http://ox.haigaiapp.cn

[O01] 启动一个线程
来源：http://js.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qr.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vu.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bj.hnjuh.cn

TS:   // 同 JS
来源：http://kn.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://tn.haigaiapp.cn

Go:   go f()
来源：http://ke.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://hx.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://fe.asd995.cn

[O02] 使用线程池
来源：http://gl.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://af.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qq.newstarts.cn

JS:   // worker_threads 线程池
来源：http://mf.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://la.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zr.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xy.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://em.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ra.asd995.cn

[O03] 加锁保护共享数据
来源：http://cb.hnjuh.cn

Py:   with lock: shared += 1
来源：http://bm.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://yc.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://am.wgjwhj.cn

TS:   // 同 JS
来源：http://wr.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://do.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lb.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qn.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://uz.hahajie.cn

[O04] 定义异步函数并等待
来源：http://pa.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://pu.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://la.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://lu.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pl.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://df.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oh.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://el.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://bt.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://gb.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://nb.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xd.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://qo.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ao.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fa.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://to.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://dk.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kj.newstarts.cn

[O06] 使用进程池
来源：http://mk.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://is.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lp.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://yc.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://bs.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hn.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://id.bookmarksfly.cn

Ruby: // fork 块
来源：http://jx.asd995.cn

C#:   Parallel.For
来源：http://zk.huanxung.cn

================================================================================
来源：http://lo.nszjky.cn

P. 常用工具函数
来源：http://yx.huixiangedu.cn

================================================================================
来源：http://sj.bookmarksfly.cn

[P01] 生成 UUID
来源：http://bk.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://np.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ru.9csxet.cn

JS:   crypto.randomUUID()
来源：http://pg.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://yu.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://mh.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://bl.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://ya.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://aq.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://qu.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sm.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tc.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sy.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dd.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wf.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ss.yuexingan06.cn


<!-- 参考信息 -->