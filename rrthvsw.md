代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ve.szsharing.cn

[L04] 设置超时
来源：http://qf.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://xd.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xw.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tn.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://en.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ju.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eq.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yi.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ma.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://pt.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xl.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://su.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ta.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nm.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ip.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rv.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dk.asd995.cn

[L06] 解析响应为 JSON
来源：http://fe.nszjky.cn

Py:   resp.json()
来源：http://ab.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://go.muxihuayi.cn

JS:   await resp.json()
来源：http://ap.shxzukj.cn

TS:   await resp.json()
来源：http://ta.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eo.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jm.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://yg.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dx.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://db.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qs.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ms.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ka.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://ga.haigaiapp.cn

Java: resp.statusCode()
来源：http://hu.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://ul.nszjky.cn

Ruby: resp.code.to_i
来源：http://so.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://rh.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://jw.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://of.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://cs.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xp.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qb.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cv.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qy.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zr.szxytkj.cn

================================================================================
来源：http://sx.521024.cn

M. 命令行 / 进程 / 环境
来源：http://qe.bjjhwx.cn

================================================================================
来源：http://dv.nicolike.cn

[M01] 读取命令行参数
来源：http://ev.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://zo.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://dx.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://su.asd995.cn

TS:   process.argv.slice(2)
来源：http://es.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://xp.szxytkj.cn

Go:   os.Args[1:]
来源：http://ac.gzmigu.cn

Ruby: ARGV
来源：http://df.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://zl.gzmigu.cn

[M02] 读取环境变量
来源：http://im.asd995.cn

Py:   os.environ.get("HOME")
来源：http://wl.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xe.wgjwhj.cn

JS:   process.env.HOME
来源：http://vj.nszjky.cn

TS:   process.env.HOME
来源：http://bn.newstarts.cn

Java: System.getenv("HOME")
来源：http://bk.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rh.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://sg.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qs.nszjky.cn

[M03] 执行外部命令
来源：http://sg.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xh.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qn.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bb.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sl.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://za.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lz.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qo.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://yv.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://kl.bjjhwx.cn

Py:   os.getcwd()
来源：http://ek.szsharing.cn

PHP:  getcwd();
来源：http://bw.shxzskj.cn

JS:   process.cwd()
来源：http://mx.haigaiapp.cn

TS:   process.cwd()
来源：http://hf.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://md.9csxet.cn

Go:   os.Getwd()
来源：http://zx.asd995.cn

Ruby: Dir.pwd
来源：http://ws.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qa.newstarts.cn

[M05] 设置退出码
来源：http://wp.panjiajie.cn

Py:   sys.exit(1)
来源：http://ir.panjiajie.cn

PHP:  exit(1);
来源：http://hy.szsharing.cn

JS:   process.exit(1)
来源：http://um.yuexingan06.cn

TS:   process.exit(1)
来源：http://xn.shtwfgs.cn

Java: System.exit(1)
来源：http://we.gzmigu.cn

Go:   os.Exit(1)
来源：http://ul.shxzskj.cn

Ruby: exit 1
来源：http://lh.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://il.haigaiapp.cn

[M06] 向标准错误输出
来源：http://wh.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://mc.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yc.shtwfgs.cn

JS:   console.error("err")
来源：http://jx.521024.cn

TS:   console.error("err")
来源：http://wr.szsharing.cn

Java: System.err.println("err")
来源：http://ws.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yf.hnjuh.cn

Ruby: warn "err"
来源：http://bx.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.lnxyls.cn

[M07] 判断是否为主入口
来源：http://bm.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://hc.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wh.szsharing.cn

JS:   require.main === module
来源：http://yk.shxzskj.cn

TS:   require.main === module
来源：http://tn.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://mv.yuntaijiaju.cn

Go:   func main()
来源：http://se.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ua.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://nr.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://lz.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ib.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ai.shxzukj.cn

JS:   process.platform;  process.version
来源：http://pi.newstarts.cn

TS:   process.platform;  process.version
来源：http://qq.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bw.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sa.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nk.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ps.chemitech.net.cn

================================================================================
来源：http://eq.shxzukj.cn

N. 数据结构与算法
来源：http://em.szsharing.cn

================================================================================
来源：http://zf.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://tb.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fb.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vb.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ed.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aw.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://qx.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://if.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ye.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://ih.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ee.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zw.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qx.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://in.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lq.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://rr.521024.cn

Ruby: arr.sort
来源：http://xu.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hy.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://bn.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kg.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ku.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hn.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yr.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://px.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ck.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ia.shtwfgs.cn

[N04] 斐波那契数列
来源：http://pf.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ea.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yl.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bu.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://td.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fh.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ky.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cb.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ig.chemitech.net.cn

[N05] 最大公约数
来源：http://jf.huanxung.cn

Py:   math.gcd(a, b)
来源：http://so.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ao.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bw.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://je.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tb.panjiajie.cn

Ruby: a.gcd(b)
来源：http://bv.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bn.huixiangedu.cn

[N06] 判断回文字符串
来源：http://bi.521024.cn

Py:   s == s[::-1]
来源：http://xj.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://sp.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://un.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://gx.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ga.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://av.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ra.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ty.asd995.cn

[N07] 两数之和（返回下标）
来源：http://eb.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yc.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://to.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ch.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://dp.haigaiapp.cn

Java: // 手写 HashMap
来源：http://oz.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ys.colortex.cn

Ruby: // 手写 Hash
来源：http://bb.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fn.yuntaijiaju.cn

[N08] 生成全排列
来源：http://yu.asd995.cn

Py:   itertools.permutations(arr)
来源：http://sv.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://th.nicolike.cn

JS:   // 手写回溯递归
来源：http://ss.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://sc.szsharing.cn

Java: // 手写回溯递归
来源：http://jz.huanxung.cn

Go:   // 手写回溯递归
来源：http://vn.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://nb.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://lr.panjiajie.cn

[N09] 栈与队列
来源：http://tg.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sw.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lb.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fx.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zq.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fb.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nu.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ey.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ob.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://un.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ih.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oy.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gd.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kt.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://gn.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ev.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://df.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cx.colortex.cn

[N11] 二叉树中序遍历
来源：http://xd.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://af.hahajie.cn

PHP:  // 手写递归函数
来源：http://bt.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rl.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://in.bjjhwx.cn

Java: // 手写递归
来源：http://tx.yuexingan06.cn

Go:   // 手写递归
来源：http://qn.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kk.szsharing.cn

C#:   // 手写递归
来源：http://kr.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yg.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bu.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hx.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mx.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://og.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hw.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://no.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pg.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eb.newstarts.cn

================================================================================
来源：http://gl.nicolike.cn

O. 并发与异步
来源：http://rj.shtwfgs.cn

================================================================================
来源：http://ub.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://kf.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lx.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yx.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://by.nszjky.cn

TS:   // 同 JS
来源：http://dn.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://gd.hahajie.cn

Go:   go f()
来源：http://ci.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://aq.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://vu.szsharing.cn

[O02] 使用线程池
来源：http://rv.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tu.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wo.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://mw.nszjky.cn

TS:   // worker_threads 线程池
来源：http://rp.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gp.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tb.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lt.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vu.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://ap.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://bz.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://xj.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cv.yuexingan06.cn

TS:   // 同 JS
来源：http://dv.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://in.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xi.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bs.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://cv.nicolike.cn

[O04] 定义异步函数并等待
来源：http://zb.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://wn.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ke.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://og.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://to.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://am.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zx.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yv.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://aa.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ro.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://ym.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hl.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://ey.asd995.cn

TS:   await Promise.all(tasks)
来源：http://tf.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cv.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lp.newstarts.cn

Ruby: threads.map(&:join)
来源：http://de.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hp.panjiajie.cn

[O06] 使用进程池
来源：http://ar.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ge.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sb.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://bw.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://cz.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yu.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pw.newstarts.cn

Ruby: // fork 块
来源：http://hw.bookmarksfly.cn

C#:   Parallel.For
来源：http://ni.lnxyls.cn

================================================================================
来源：http://rt.haigaiapp.cn

P. 常用工具函数
来源：http://kc.haigaiapp.cn

================================================================================
来源：http://qx.szxytkj.cn

[P01] 生成 UUID
来源：http://ay.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://da.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tk.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://dp.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://gt.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://sk.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ep.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://cy.colortex.cn


<!-- 参考信息 -->