代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oh.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lb.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://au.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qb.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xe.gzmigu.cn

[L04] 设置超时
来源：http://sp.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://mr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rr.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bl.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pk.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uk.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uj.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ba.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://go.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://mf.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uq.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qw.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://af.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://of.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vq.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bt.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sr.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://uf.yuexingan06.cn

Py:   resp.json()
来源：http://wa.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ba.muxihuayi.cn

JS:   await resp.json()
来源：http://xn.gzmigu.cn

TS:   await resp.json()
来源：http://gj.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://du.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ws.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ia.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qv.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://qw.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gi.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pe.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ld.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://kh.gzmigu.cn

Java: resp.statusCode()
来源：http://jc.hnjuh.cn

Go:   resp.StatusCode
来源：http://di.shxzskj.cn

Ruby: resp.code.to_i
来源：http://pv.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://mv.lnxyls.cn

[L08] 并发请求多个地址
来源：http://bw.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uo.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://rj.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bo.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cl.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jf.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wx.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ji.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tr.huanxung.cn

================================================================================
来源：http://zt.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://su.muxihuayi.cn

================================================================================
来源：http://bl.shtwfgs.cn

[M01] 读取命令行参数
来源：http://vv.lnxyls.cn

Py:   sys.argv[1:]
来源：http://nf.521024.cn

PHP:  $argv;  $argc;
来源：http://ej.521024.cn

JS:   process.argv.slice(2)
来源：http://nt.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://zu.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://bh.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ug.shtwfgs.cn

Ruby: ARGV
来源：http://af.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://bn.huixiangedu.cn

[M02] 读取环境变量
来源：http://ub.521024.cn

Py:   os.environ.get("HOME")
来源：http://bx.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jx.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://oe.nszjky.cn

TS:   process.env.HOME
来源：http://ag.shxzukj.cn

Java: System.getenv("HOME")
来源：http://gy.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://py.9csxet.cn

Ruby: ENV["HOME"]
来源：http://vv.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oc.panjiajie.cn

[M03] 执行外部命令
来源：http://tf.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hl.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zu.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jz.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://un.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bg.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qt.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ph.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://jv.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://yh.asd995.cn

Py:   os.getcwd()
来源：http://zl.nicolike.cn

PHP:  getcwd();
来源：http://fm.nicolike.cn

JS:   process.cwd()
来源：http://zi.hahajie.cn

TS:   process.cwd()
来源：http://wb.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://cz.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://lu.huixiangedu.cn

Ruby: Dir.pwd
来源：http://mq.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aq.hahajie.cn

[M05] 设置退出码
来源：http://tb.szxytkj.cn

Py:   sys.exit(1)
来源：http://wb.szsharing.cn

PHP:  exit(1);
来源：http://wz.asd995.cn

JS:   process.exit(1)
来源：http://yt.colortex.cn

TS:   process.exit(1)
来源：http://do.szsharing.cn

Java: System.exit(1)
来源：http://qn.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://fj.shxzukj.cn

Ruby: exit 1
来源：http://nz.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ku.haigaiapp.cn

[M06] 向标准错误输出
来源：http://uw.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://md.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dh.yuntaijiaju.cn

JS:   console.error("err")
来源：http://wc.jctech888.com.cn

TS:   console.error("err")
来源：http://ca.yuexingan06.cn

Java: System.err.println("err")
来源：http://ot.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ln.shxzskj.cn

Ruby: warn "err"
来源：http://kk.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.newstarts.cn

[M07] 判断是否为主入口
来源：http://si.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://rt.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bm.szsharing.cn

JS:   require.main === module
来源：http://ov.nicolike.cn

TS:   require.main === module
来源：http://mg.nszjky.cn

Java: public static void main(String[] args)
来源：http://mc.9csxet.cn

Go:   func main()
来源：http://ic.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fk.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://cq.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://dx.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://mb.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://zq.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://rg.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://iw.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://em.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ix.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yu.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://or.9csxet.cn

================================================================================
来源：http://km.shxzskj.cn

N. 数据结构与算法
来源：http://ki.jianghongdianzi.cn

================================================================================
来源：http://tk.colortex.cn

[N01] 二分查找（有序数组）
来源：http://yk.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zw.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hb.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uo.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vo.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jn.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://gl.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lg.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ee.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://vi.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zg.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fh.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jm.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gc.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ij.asd995.cn

Go:   slices.Sort(arr)
来源：http://nf.muxihuayi.cn

Ruby: arr.sort
来源：http://sr.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hr.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://eo.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qv.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://sg.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dz.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ox.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yq.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yn.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dm.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ey.panjiajie.cn

[N04] 斐波那契数列
来源：http://cm.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ob.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oy.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ry.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bu.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://to.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ws.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vb.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ry.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ds.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://fj.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lc.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ju.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ic.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cd.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://he.colortex.cn

Ruby: a.gcd(b)
来源：http://cv.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yc.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://ke.chemitech.net.cn

Py:   s == s[::-1]
来源：http://kj.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://if.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://mp.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://by.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cd.hahajie.cn

Go:   // 双指针从两端比较
来源：http://ae.shxzskj.cn

Ruby: s == s.reverse
来源：http://lc.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tk.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://yd.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sz.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qk.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nh.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://wc.panjiajie.cn

Java: // 手写 HashMap
来源：http://yx.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://ct.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://wk.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jv.bjjhwx.cn

[N08] 生成全排列
来源：http://nj.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://oo.asd995.cn

PHP:  // 手写递归交换
来源：http://po.szsharing.cn

JS:   // 手写回溯递归
来源：http://er.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://ah.shxzskj.cn

Java: // 手写回溯递归
来源：http://om.asd995.cn

Go:   // 手写回溯递归
来源：http://sk.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://ep.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://ft.521024.cn

[N09] 栈与队列
来源：http://ao.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ik.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kd.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dx.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zo.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qc.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mo.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jd.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sa.huixiangedu.cn

[N10] 链表节点定义
来源：http://xt.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lv.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ei.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qy.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zk.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://nn.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jv.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ai.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dg.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://xo.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rh.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://lg.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ue.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ms.gzmigu.cn

Java: // 手写递归
来源：http://gx.yuexingan06.cn

Go:   // 手写递归
来源：http://bf.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pl.muxihuayi.cn

C#:   // 手写递归
来源：http://jk.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fl.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://at.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://co.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ps.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zi.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tj.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cb.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nz.shtwfgs.cn

================================================================================
来源：http://vi.jianghongdianzi.cn

O. 并发与异步
来源：http://se.bookmarksfly.cn

================================================================================
来源：http://br.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://vi.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qo.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fv.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zv.bjjhwx.cn

TS:   // 同 JS
来源：http://rg.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://ue.colortex.cn

Go:   go f()
来源：http://rb.shxzskj.cn

Ruby: Thread.new { f }
来源：http://si.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ue.szsharing.cn

[O02] 使用线程池
来源：http://sl.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ft.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://un.nicolike.cn

JS:   // worker_threads 线程池
来源：http://jx.szsharing.cn

TS:   // worker_threads 线程池
来源：http://in.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qe.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lh.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zs.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ek.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://zt.szsharing.cn

Py:   with lock: shared += 1
来源：http://ov.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://cn.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ix.bookmarksfly.cn

TS:   // 同 JS
来源：http://cw.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://wb.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ot.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wl.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://pf.521024.cn

[O04] 定义异步函数并等待
来源：http://ak.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://vz.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lo.asd995.cn

JS:   async function f() { await g(); }
来源：http://sm.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fe.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fy.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jm.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gz.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://vf.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://mc.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://nq.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aq.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://fm.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://ho.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rp.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ly.521024.cn

Ruby: threads.map(&:join)
来源：http://ol.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ly.shxzukj.cn

[O06] 使用进程池
来源：http://zs.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://au.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rc.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://oo.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://ig.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dk.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nw.hnjuh.cn

Ruby: // fork 块
来源：http://ct.newstarts.cn

C#:   Parallel.For
来源：http://vx.huanxung.cn

================================================================================
来源：http://sa.9csxet.cn

P. 常用工具函数
来源：http://sd.asd995.cn

================================================================================
来源：http://ie.lnxyls.cn

[P01] 生成 UUID
来源：http://eo.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://hu.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tw.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://qq.huixiangedu.cn


<!-- 参考信息 -->