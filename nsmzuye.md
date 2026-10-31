代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://et.szsharing.cn

[L04] 设置超时
来源：http://cl.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://tl.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ly.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uf.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yj.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://au.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ds.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bb.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sm.szsharing.cn

[L05] 上传文件（multipart）
来源：http://xl.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gt.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fu.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zy.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jo.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ta.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qb.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ha.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ft.szsharing.cn

[L06] 解析响应为 JSON
来源：http://lh.bjjhwx.cn

Py:   resp.json()
来源：http://gz.521024.cn

PHP:  json_decode($body, true);
来源：http://xt.9csxet.cn

JS:   await resp.json()
来源：http://xg.gzmigu.cn

TS:   await resp.json()
来源：http://yx.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://an.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ji.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://wd.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nw.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://io.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sd.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sx.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://ix.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://km.9csxet.cn

Java: resp.statusCode()
来源：http://gz.lnxyls.cn

Go:   resp.StatusCode
来源：http://ni.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://jh.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://bp.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://uv.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fn.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://fl.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vi.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fe.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hw.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vw.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bi.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nl.jctech888.com.cn

================================================================================
来源：http://ar.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://kj.muxihuayi.cn

================================================================================
来源：http://mk.gzmigu.cn

[M01] 读取命令行参数
来源：http://qd.nicolike.cn

Py:   sys.argv[1:]
来源：http://kl.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://ki.nicolike.cn

JS:   process.argv.slice(2)
来源：http://kv.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://vx.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://dc.newstarts.cn

Go:   os.Args[1:]
来源：http://cc.hahajie.cn

Ruby: ARGV
来源：http://mb.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://zl.bookmarksfly.cn

[M02] 读取环境变量
来源：http://lu.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://co.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ef.bookmarksfly.cn

JS:   process.env.HOME
来源：http://kl.bjjhwx.cn

TS:   process.env.HOME
来源：http://js.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ka.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gr.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://fx.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yd.9csxet.cn

[M03] 执行外部命令
来源：http://oz.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sa.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qu.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wa.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tk.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jh.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ng.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wm.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://qx.gzmigu.cn

[M04] 获取当前工作目录
来源：http://wk.wgjwhj.cn

Py:   os.getcwd()
来源：http://yb.huixinmuqiang.cn

PHP:  getcwd();
来源：http://zl.huixinmuqiang.cn

JS:   process.cwd()
来源：http://te.shxzukj.cn

TS:   process.cwd()
来源：http://dc.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://wo.chemitech.net.cn

Go:   os.Getwd()
来源：http://py.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://xr.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://og.huanxung.cn

[M05] 设置退出码
来源：http://go.szxytkj.cn

Py:   sys.exit(1)
来源：http://ws.huixinmuqiang.cn

PHP:  exit(1);
来源：http://hn.huanxung.cn

JS:   process.exit(1)
来源：http://tn.gzmigu.cn

TS:   process.exit(1)
来源：http://hx.panjiajie.cn

Java: System.exit(1)
来源：http://ti.asd995.cn

Go:   os.Exit(1)
来源：http://vb.huixinmuqiang.cn

Ruby: exit 1
来源：http://tk.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fx.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ss.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://ip.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jp.shxzskj.cn

JS:   console.error("err")
来源：http://nd.shtwfgs.cn

TS:   console.error("err")
来源：http://ah.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://cj.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pv.521024.cn

Ruby: warn "err"
来源：http://sv.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://qp.shxzskj.cn

[M07] 判断是否为主入口
来源：http://jp.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://md.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hh.yuntaijiaju.cn

JS:   require.main === module
来源：http://zy.muxihuayi.cn

TS:   require.main === module
来源：http://lg.hahajie.cn

Java: public static void main(String[] args)
来源：http://na.yuntaijiaju.cn

Go:   func main()
来源：http://hj.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ph.521024.cn

C#:   static void Main(string[] args)
来源：http://fq.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://aq.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ac.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mc.panjiajie.cn

JS:   process.platform;  process.version
来源：http://py.newstarts.cn

TS:   process.platform;  process.version
来源：http://tl.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oy.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://em.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qc.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oh.szxytkj.cn

================================================================================
来源：http://au.colortex.cn

N. 数据结构与算法
来源：http://mk.huixiangedu.cn

================================================================================
来源：http://th.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://hp.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dg.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cj.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rp.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zm.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ei.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ny.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://of.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ab.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ar.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ta.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ch.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ba.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vb.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cx.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://lk.bookmarksfly.cn

Ruby: arr.sort
来源：http://ka.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ga.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://sj.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bp.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://su.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ix.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nw.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://su.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sa.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jx.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sb.chemitech.net.cn

[N04] 斐波那契数列
来源：http://gp.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fb.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qr.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zm.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xt.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yw.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xy.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://co.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yv.haigaiapp.cn

[N05] 最大公约数
来源：http://au.szsharing.cn

Py:   math.gcd(a, b)
来源：http://bl.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xo.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yz.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gv.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dy.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bv.lnxyls.cn

Ruby: a.gcd(b)
来源：http://my.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://td.haigaiapp.cn

[N06] 判断回文字符串
来源：http://zh.wgjwhj.cn

Py:   s == s[::-1]
来源：http://pv.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://fl.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://ym.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://zz.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tz.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://tq.asd995.cn

Ruby: s == s.reverse
来源：http://bf.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wp.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://nf.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ly.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dw.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gd.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://ps.asd995.cn

Java: // 手写 HashMap
来源：http://at.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://zv.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://uc.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kc.wgjwhj.cn

[N08] 生成全排列
来源：http://qr.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://rj.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://lu.hahajie.cn

JS:   // 手写回溯递归
来源：http://cg.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://kj.hahajie.cn

Java: // 手写回溯递归
来源：http://mp.hahajie.cn

Go:   // 手写回溯递归
来源：http://js.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://rz.newstarts.cn

C#:   // 手写回溯递归
来源：http://ra.huixinmuqiang.cn

[N09] 栈与队列
来源：http://fo.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rq.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pj.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ki.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hi.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bc.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vu.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lu.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xh.shtwfgs.cn

[N10] 链表节点定义
来源：http://ms.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mq.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fr.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://af.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hj.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://sy.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vp.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xv.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bu.szsharing.cn

[N11] 二叉树中序遍历
来源：http://je.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zv.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://yb.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ml.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://os.chemitech.net.cn

Java: // 手写递归
来源：http://io.newstarts.cn

Go:   // 手写递归
来源：http://yh.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gi.chemitech.net.cn

C#:   // 手写递归
来源：http://ab.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ck.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xa.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cb.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xx.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zm.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ls.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jv.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mn.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tk.muxihuayi.cn

================================================================================
来源：http://xy.jianghongdianzi.cn

O. 并发与异步
来源：http://xf.hahajie.cn

================================================================================
来源：http://mr.haigaiapp.cn

[O01] 启动一个线程
来源：http://gm.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://po.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fg.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hg.yuntaijiaju.cn

TS:   // 同 JS
来源：http://sb.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://ki.yuexingan06.cn

Go:   go f()
来源：http://mp.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://mu.szsharing.cn

C#:   Task.Run(() => F());
来源：http://ut.panjiajie.cn

[O02] 使用线程池
来源：http://us.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://be.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wj.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ju.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://uc.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ue.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gz.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ey.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nl.nicolike.cn

[O03] 加锁保护共享数据
来源：http://tp.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://fj.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://ui.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qh.szsharing.cn

TS:   // 同 JS
来源：http://mm.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://op.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lg.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gg.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ym.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://gw.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ai.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aq.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://jf.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bb.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yo.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vz.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sl.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://gm.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://ry.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ap.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gn.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://vc.521024.cn

TS:   await Promise.all(tasks)
来源：http://ru.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ah.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://av.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://il.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zl.haigaiapp.cn

[O06] 使用进程池
来源：http://ub.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qg.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qu.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://mh.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://ga.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ud.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ls.jianghongdianzi.cn

Ruby: // fork 块
来源：http://wa.jianghongdianzi.cn

C#:   Parallel.For
来源：http://yo.newstarts.cn

================================================================================
来源：http://ps.huixinmuqiang.cn

P. 常用工具函数
来源：http://hl.yuntaijiaju.cn

================================================================================
来源：http://fy.9csxet.cn

[P01] 生成 UUID
来源：http://sf.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://qn.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mn.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ze.newstarts.cn

TS:   crypto.randomUUID()
来源：http://pk.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://tp.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://uf.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://fq.jctech888.com.cn


<!-- 参考信息 -->