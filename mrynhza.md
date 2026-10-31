代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ad.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bl.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ge.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://na.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pv.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tz.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://fg.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ov.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vs.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lx.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fg.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nh.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xy.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pv.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ax.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://tk.muxihuayi.cn

Py:   resp.json()
来源：http://gt.szsharing.cn

PHP:  json_decode($body, true);
来源：http://xd.521024.cn

JS:   await resp.json()
来源：http://yp.muxihuayi.cn

TS:   await resp.json()
来源：http://lb.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bu.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pq.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://zp.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qp.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://rr.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bf.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ky.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ed.521024.cn

TS:   resp.ok;  resp.status
来源：http://zf.chemitech.net.cn

Java: resp.statusCode()
来源：http://af.9csxet.cn

Go:   resp.StatusCode
来源：http://sq.hnjuh.cn

Ruby: resp.code.to_i
来源：http://ti.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://pn.9csxet.cn

[L08] 并发请求多个地址
来源：http://fs.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zj.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://pu.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qp.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tf.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zx.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sd.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zw.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bb.newstarts.cn

================================================================================
来源：http://xd.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://to.bjjhwx.cn

================================================================================
来源：http://yi.asd995.cn

[M01] 读取命令行参数
来源：http://ej.shxzskj.cn

Py:   sys.argv[1:]
来源：http://vd.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://tc.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://lb.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://aj.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://uz.bjjhwx.cn

Go:   os.Args[1:]
来源：http://oo.yuntaijiaju.cn

Ruby: ARGV
来源：http://tj.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://zu.wgjwhj.cn

[M02] 读取环境变量
来源：http://uu.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://gy.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jb.haigaiapp.cn

JS:   process.env.HOME
来源：http://vg.bookmarksfly.cn

TS:   process.env.HOME
来源：http://bm.huanxung.cn

Java: System.getenv("HOME")
来源：http://mt.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xg.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://yo.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://he.haigaiapp.cn

[M03] 执行外部命令
来源：http://ge.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jx.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pq.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wy.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jg.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ed.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gr.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xf.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ez.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://nr.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://qc.lnxyls.cn

PHP:  getcwd();
来源：http://rs.gzmigu.cn

JS:   process.cwd()
来源：http://cw.lnxyls.cn

TS:   process.cwd()
来源：http://bo.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://kd.chemitech.net.cn

Go:   os.Getwd()
来源：http://dt.panjiajie.cn

Ruby: Dir.pwd
来源：http://dl.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lb.yuexingan06.cn

[M05] 设置退出码
来源：http://ik.yuexingan06.cn

Py:   sys.exit(1)
来源：http://gr.yuexingan06.cn

PHP:  exit(1);
来源：http://pk.asd995.cn

JS:   process.exit(1)
来源：http://xt.newstarts.cn

TS:   process.exit(1)
来源：http://zz.hahajie.cn

Java: System.exit(1)
来源：http://ch.521024.cn

Go:   os.Exit(1)
来源：http://af.jianghongdianzi.cn

Ruby: exit 1
来源：http://gk.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zx.shtwfgs.cn

[M06] 向标准错误输出
来源：http://vo.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://nd.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wm.wgjwhj.cn

JS:   console.error("err")
来源：http://eh.asd995.cn

TS:   console.error("err")
来源：http://xq.colortex.cn

Java: System.err.println("err")
来源：http://nz.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pt.huanxung.cn

Ruby: warn "err"
来源：http://qs.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://uy.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://mk.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://vg.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uk.huixinmuqiang.cn

JS:   require.main === module
来源：http://sy.colortex.cn

TS:   require.main === module
来源：http://uz.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://wk.yuexingan06.cn

Go:   func main()
来源：http://ue.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ge.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://oi.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://my.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://jh.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://nm.gzmigu.cn

JS:   process.platform;  process.version
来源：http://kg.szsharing.cn

TS:   process.platform;  process.version
来源：http://at.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bm.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aj.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hi.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zs.chemitech.net.cn

================================================================================
来源：http://iy.yuexingan06.cn

N. 数据结构与算法
来源：http://rp.colortex.cn

================================================================================
来源：http://ef.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://cg.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xh.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gr.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bu.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oe.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zq.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://oq.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gp.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iu.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://ps.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://fh.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://af.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yx.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zl.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ng.jctech888.com.cn

Ruby: arr.sort
来源：http://hn.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://co.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://vs.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eh.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://sm.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ce.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ud.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wu.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wj.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nk.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bf.szxytkj.cn

[N04] 斐波那契数列
来源：http://wx.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nt.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kh.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kz.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rw.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dk.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wm.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sg.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pd.szsharing.cn

[N05] 最大公约数
来源：http://qa.nszjky.cn

Py:   math.gcd(a, b)
来源：http://io.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ky.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wu.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://de.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dv.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hs.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://fk.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ql.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://eo.szxytkj.cn

Py:   s == s[::-1]
来源：http://xd.521024.cn

PHP:  $s === strrev($s);
来源：http://dc.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://on.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://in.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yp.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ka.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ss.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cm.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://tq.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ln.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ip.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xo.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://sm.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ln.nicolike.cn

Go:   // 手写 map[int]int
来源：http://nv.nszjky.cn

Ruby: // 手写 Hash
来源：http://pr.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://de.szxytkj.cn

[N08] 生成全排列
来源：http://xw.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://bi.521024.cn

PHP:  // 手写递归交换
来源：http://uh.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://tt.szsharing.cn

TS:   // 手写回溯递归
来源：http://sx.haigaiapp.cn

Java: // 手写回溯递归
来源：http://oj.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://gw.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://tn.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://fo.gzmigu.cn

[N09] 栈与队列
来源：http://oy.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ph.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kw.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://es.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qg.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lm.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ae.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://on.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hf.gzmigu.cn

[N10] 链表节点定义
来源：http://jb.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xb.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kd.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://en.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://we.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://dl.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dk.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fw.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pl.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://ot.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iy.9csxet.cn

PHP:  // 手写递归函数
来源：http://jq.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hu.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vc.jctech888.com.cn

Java: // 手写递归
来源：http://fq.huixinmuqiang.cn

Go:   // 手写递归
来源：http://gs.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bc.gzmigu.cn

C#:   // 手写递归
来源：http://em.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cl.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dc.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ai.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yc.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://md.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hh.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tu.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cy.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cm.jctech888.com.cn

================================================================================
来源：http://jv.gzmigu.cn

O. 并发与异步
来源：http://yw.lnxyls.cn

================================================================================
来源：http://ns.521024.cn

[O01] 启动一个线程
来源：http://mo.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://si.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://to.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yh.szxytkj.cn

TS:   // 同 JS
来源：http://xb.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://dg.9csxet.cn

Go:   go f()
来源：http://du.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://gn.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://zy.bookmarksfly.cn

[O02] 使用线程池
来源：http://th.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mg.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pj.huanxung.cn

JS:   // worker_threads 线程池
来源：http://ud.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://bx.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gs.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vp.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ec.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fe.521024.cn

[O03] 加锁保护共享数据
来源：http://nv.shxzskj.cn

Py:   with lock: shared += 1
来源：http://el.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ur.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cc.lnxyls.cn

TS:   // 同 JS
来源：http://xo.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://ed.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hf.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iz.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://va.newstarts.cn

[O04] 定义异步函数并等待
来源：http://zc.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://xb.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xe.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://je.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vm.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hn.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jn.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lx.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://zg.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://jv.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://ct.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pp.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://ex.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://fp.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mh.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ao.nszjky.cn

Ruby: threads.map(&:join)
来源：http://vx.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iw.nszjky.cn

[O06] 使用进程池
来源：http://ib.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uw.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ri.colortex.cn

JS:   // child_process / cluster 模块
来源：http://jl.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://qa.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tk.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yx.shtwfgs.cn

Ruby: // fork 块
来源：http://nd.hnjuh.cn

C#:   Parallel.For
来源：http://kd.panjiajie.cn

================================================================================
来源：http://if.muxihuayi.cn

P. 常用工具函数
来源：http://lw.521024.cn

================================================================================
来源：http://dn.yuexingan06.cn

[P01] 生成 UUID
来源：http://tc.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://ob.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fq.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://ao.huanxung.cn

TS:   crypto.randomUUID()
来源：http://ej.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://fi.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://bh.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ex.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://jk.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://fg.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nr.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ib.lnxyls.cn


<!-- 参考信息 -->