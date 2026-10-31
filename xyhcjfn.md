代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ix.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://do.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nk.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://po.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zm.gzmigu.cn

[L04] 设置超时
来源：http://po.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://ka.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dt.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gb.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hf.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zh.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zo.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sa.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://pj.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bf.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zh.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vj.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bv.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ri.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sz.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lg.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cl.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://kb.lnxyls.cn

Py:   resp.json()
来源：http://yk.huanxung.cn

PHP:  json_decode($body, true);
来源：http://cr.huixiangedu.cn

JS:   await resp.json()
来源：http://ar.huanxung.cn

TS:   await resp.json()
来源：http://rp.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eq.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wg.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://kl.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gs.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://zt.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pt.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hw.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://vv.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://ql.wgjwhj.cn

Java: resp.statusCode()
来源：http://fy.huixiangedu.cn

Go:   resp.StatusCode
来源：http://hp.lnxyls.cn

Ruby: resp.code.to_i
来源：http://ky.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://wa.hahajie.cn

[L08] 并发请求多个地址
来源：http://yw.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ir.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ly.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jf.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://la.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lb.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ra.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vb.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hm.yuexingan06.cn

================================================================================
来源：http://xt.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://jn.huixinmuqiang.cn

================================================================================
来源：http://yk.huixiangedu.cn

[M01] 读取命令行参数
来源：http://kd.panjiajie.cn

Py:   sys.argv[1:]
来源：http://om.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://wh.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://ng.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://fr.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://gv.huanxung.cn

Go:   os.Args[1:]
来源：http://so.huixiangedu.cn

Ruby: ARGV
来源：http://ml.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://op.hahajie.cn

[M02] 读取环境变量
来源：http://vo.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://xl.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://km.shtwfgs.cn

JS:   process.env.HOME
来源：http://ms.muxihuayi.cn

TS:   process.env.HOME
来源：http://xk.hnjuh.cn

Java: System.getenv("HOME")
来源：http://to.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qv.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ta.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://by.gzmigu.cn

[M03] 执行外部命令
来源：http://nh.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ig.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://js.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fp.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jc.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ag.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gh.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rw.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://fh.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ln.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://uy.wgjwhj.cn

PHP:  getcwd();
来源：http://bk.nicolike.cn

JS:   process.cwd()
来源：http://iu.newstarts.cn

TS:   process.cwd()
来源：http://sv.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://qk.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://un.huixiangedu.cn

Ruby: Dir.pwd
来源：http://mh.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vu.lnxyls.cn

[M05] 设置退出码
来源：http://jh.hnjuh.cn

Py:   sys.exit(1)
来源：http://ku.jianghongdianzi.cn

PHP:  exit(1);
来源：http://fl.wgjwhj.cn

JS:   process.exit(1)
来源：http://nd.szsharing.cn

TS:   process.exit(1)
来源：http://hh.shxzukj.cn

Java: System.exit(1)
来源：http://gf.nszjky.cn

Go:   os.Exit(1)
来源：http://gt.muxihuayi.cn

Ruby: exit 1
来源：http://fb.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ym.huanxung.cn

[M06] 向标准错误输出
来源：http://qx.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://vz.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://je.szsharing.cn

JS:   console.error("err")
来源：http://jp.haigaiapp.cn

TS:   console.error("err")
来源：http://zy.szxytkj.cn

Java: System.err.println("err")
来源：http://hr.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ss.huanxung.cn

Ruby: warn "err"
来源：http://wb.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://so.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://be.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://ge.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ar.nicolike.cn

JS:   require.main === module
来源：http://sk.huanxung.cn

TS:   require.main === module
来源：http://fy.szsharing.cn

Java: public static void main(String[] args)
来源：http://wx.nicolike.cn

Go:   func main()
来源：http://qb.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jk.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://yf.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://bp.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ia.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://gt.huanxung.cn

JS:   process.platform;  process.version
来源：http://it.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://sz.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vp.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rz.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tz.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dm.shtwfgs.cn

================================================================================
来源：http://ld.yuexingan06.cn

N. 数据结构与算法
来源：http://ar.lnxyls.cn

================================================================================
来源：http://xl.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://zx.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qj.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ec.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ro.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pl.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cm.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://at.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dc.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jp.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gi.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://az.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pv.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ok.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aw.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ti.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://hv.colortex.cn

Ruby: arr.sort
来源：http://fm.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rn.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://bp.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rp.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://qu.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ee.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ol.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ff.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sw.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qd.huanxung.cn

[N04] 斐波那契数列
来源：http://fe.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ca.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wz.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dp.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ev.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wh.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fm.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yd.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jq.gzmigu.cn

[N05] 最大公约数
来源：http://fs.nszjky.cn

Py:   math.gcd(a, b)
来源：http://se.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fw.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rd.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fa.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eb.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tv.shxzukj.cn

Ruby: a.gcd(b)
来源：http://sy.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wm.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ck.huanxung.cn

Py:   s == s[::-1]
来源：http://je.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://yw.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://se.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://pl.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mm.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://xe.nicolike.cn

Ruby: s == s.reverse
来源：http://hp.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ea.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://hn.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rz.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yq.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lk.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://au.hnjuh.cn

Java: // 手写 HashMap
来源：http://fk.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://kg.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://te.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bl.nszjky.cn

[N08] 生成全排列
来源：http://uy.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://fi.szsharing.cn

PHP:  // 手写递归交换
来源：http://vu.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://qn.szxytkj.cn

TS:   // 手写回溯递归
来源：http://vr.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://ky.panjiajie.cn

Go:   // 手写回溯递归
来源：http://cj.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://iu.shxzskj.cn

C#:   // 手写回溯递归
来源：http://tp.jianghongdianzi.cn

[N09] 栈与队列
来源：http://th.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wp.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ra.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://en.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nh.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nc.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cw.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hc.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vh.shxzukj.cn

[N10] 链表节点定义
来源：http://qu.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jd.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aw.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jt.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://un.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://vn.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ky.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ef.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qz.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://zd.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://go.szxytkj.cn

PHP:  // 手写递归函数
来源：http://ti.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xx.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rc.shxzukj.cn

Java: // 手写递归
来源：http://am.9csxet.cn

Go:   // 手写递归
来源：http://vj.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tv.newstarts.cn

C#:   // 手写递归
来源：http://zt.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jz.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ma.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qo.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://am.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sh.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lt.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ai.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mn.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sq.huanxung.cn

================================================================================
来源：http://xn.huanxung.cn

O. 并发与异步
来源：http://qp.hnjuh.cn

================================================================================
来源：http://kj.bookmarksfly.cn

[O01] 启动一个线程
来源：http://ub.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ib.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ik.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bb.9csxet.cn

TS:   // 同 JS
来源：http://ss.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://uk.bjjhwx.cn

Go:   go f()
来源：http://rr.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://ag.nszjky.cn

C#:   Task.Run(() => F());
来源：http://xn.gzmigu.cn

[O02] 使用线程池
来源：http://kp.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gr.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://rb.asd995.cn

TS:   // worker_threads 线程池
来源：http://cl.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qo.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hl.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tb.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sc.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://jy.shxzskj.cn

Py:   with lock: shared += 1
来源：http://rv.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ui.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iv.hnjuh.cn

TS:   // 同 JS
来源：http://kg.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://mq.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qb.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pn.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ck.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://fz.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://bp.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://df.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://vj.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://or.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fz.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://il.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mh.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ao.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://gx.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://bw.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lu.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://kw.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://pw.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fq.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kk.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://qz.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nr.szxytkj.cn

[O06] 使用进程池
来源：http://oa.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vj.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fn.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://qx.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://bl.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nc.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zm.shxzukj.cn

Ruby: // fork 块
来源：http://zb.shxzukj.cn

C#:   Parallel.For
来源：http://af.huixinmuqiang.cn

================================================================================
来源：http://bm.yuntaijiaju.cn

P. 常用工具函数
来源：http://ad.bookmarksfly.cn

================================================================================
来源：http://ov.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://lw.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ss.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dc.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://wd.szxytkj.cn


<!-- 参考信息 -->