代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vd.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ue.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uj.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ch.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fo.chemitech.net.cn

[L04] 设置超时
来源：http://yx.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://aw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nf.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rb.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mp.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qs.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hx.nicolike.cn

[L05] 上传文件（multipart）
来源：http://ao.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ka.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hw.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bp.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rc.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pv.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mi.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ds.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ci.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://sm.yuntaijiaju.cn

Py:   resp.json()
来源：http://bn.hahajie.cn

PHP:  json_decode($body, true);
来源：http://nq.newstarts.cn

JS:   await resp.json()
来源：http://xl.521024.cn

TS:   await resp.json()
来源：http://jb.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ic.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nu.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://cj.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://at.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://jz.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wg.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ys.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://dx.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://ri.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://wy.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://ay.colortex.cn

Ruby: resp.code.to_i
来源：http://rm.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ms.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://lz.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gt.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://ke.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ab.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ox.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pc.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xv.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tj.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ma.panjiajie.cn

================================================================================
来源：http://ah.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://wz.shxzukj.cn

================================================================================
来源：http://ah.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://ji.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ab.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://xn.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://zr.huanxung.cn

TS:   process.argv.slice(2)
来源：http://cm.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://cn.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ex.gzmigu.cn

Ruby: ARGV
来源：http://wu.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://si.bjjhwx.cn

[M02] 读取环境变量
来源：http://jh.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://kt.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ah.bjjhwx.cn

JS:   process.env.HOME
来源：http://ol.shtwfgs.cn

TS:   process.env.HOME
来源：http://pd.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://mm.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jr.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ix.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zv.chemitech.net.cn

[M03] 执行外部命令
来源：http://en.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zd.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oz.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lm.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sl.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uh.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mj.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wn.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://cb.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://nx.nszjky.cn

Py:   os.getcwd()
来源：http://wm.shtwfgs.cn

PHP:  getcwd();
来源：http://xo.shxzukj.cn

JS:   process.cwd()
来源：http://nf.shtwfgs.cn

TS:   process.cwd()
来源：http://ds.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://bg.szxytkj.cn

Go:   os.Getwd()
来源：http://zu.chemitech.net.cn

Ruby: Dir.pwd
来源：http://tl.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gr.huixiangedu.cn

[M05] 设置退出码
来源：http://xl.shxzukj.cn

Py:   sys.exit(1)
来源：http://vw.haigaiapp.cn

PHP:  exit(1);
来源：http://nk.colortex.cn

JS:   process.exit(1)
来源：http://yc.jctech888.com.cn

TS:   process.exit(1)
来源：http://uw.gzmigu.cn

Java: System.exit(1)
来源：http://qd.hnjuh.cn

Go:   os.Exit(1)
来源：http://ik.jianghongdianzi.cn

Ruby: exit 1
来源：http://zs.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ea.yuexingan06.cn

[M06] 向标准错误输出
来源：http://gw.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://pc.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tm.newstarts.cn

JS:   console.error("err")
来源：http://an.huixinmuqiang.cn

TS:   console.error("err")
来源：http://qa.huixiangedu.cn

Java: System.err.println("err")
来源：http://ow.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://di.nszjky.cn

Ruby: warn "err"
来源：http://tk.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://hn.gzmigu.cn

[M07] 判断是否为主入口
来源：http://cl.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://fu.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ck.shxzskj.cn

JS:   require.main === module
来源：http://ng.huixiangedu.cn

TS:   require.main === module
来源：http://un.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://qx.newstarts.cn

Go:   func main()
来源：http://lg.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xi.521024.cn

C#:   static void Main(string[] args)
来源：http://pi.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://nh.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://xt.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://si.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://js.asd995.cn

TS:   process.platform;  process.version
来源：http://ww.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://op.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vx.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hp.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kv.muxihuayi.cn

================================================================================
来源：http://oi.huanxung.cn

N. 数据结构与算法
来源：http://gy.9csxet.cn

================================================================================
来源：http://rp.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://ws.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zl.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eh.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oa.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iv.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wf.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://lk.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cr.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vr.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://id.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://mt.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uc.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mj.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dy.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ew.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://kg.shtwfgs.cn

Ruby: arr.sort
来源：http://mp.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ml.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://qu.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mc.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://us.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vj.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://il.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uc.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qr.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lj.shtwfgs.cn

[N04] 斐波那契数列
来源：http://mu.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nv.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dz.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://es.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bx.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oe.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ei.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://le.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qi.nszjky.cn

[N05] 最大公约数
来源：http://qk.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://jb.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tr.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ac.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fn.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fa.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bw.huanxung.cn

Ruby: a.gcd(b)
来源：http://dc.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zp.asd995.cn

[N06] 判断回文字符串
来源：http://sd.yuexingan06.cn

Py:   s == s[::-1]
来源：http://rb.asd995.cn

PHP:  $s === strrev($s);
来源：http://fr.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://xt.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ih.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mh.hahajie.cn

Go:   // 双指针从两端比较
来源：http://wt.yuexingan06.cn

Ruby: s == s.reverse
来源：http://tb.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vu.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://wg.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vo.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wy.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iv.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://gq.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://qp.nicolike.cn

Go:   // 手写 map[int]int
来源：http://vf.9csxet.cn

Ruby: // 手写 Hash
来源：http://lr.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ee.nicolike.cn

[N08] 生成全排列
来源：http://yc.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://rr.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://gh.huanxung.cn

JS:   // 手写回溯递归
来源：http://sl.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://hf.muxihuayi.cn

Java: // 手写回溯递归
来源：http://fp.huanxung.cn

Go:   // 手写回溯递归
来源：http://xk.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://qc.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://hf.shxzukj.cn

[N09] 栈与队列
来源：http://tb.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tb.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sw.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dr.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pf.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dn.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fs.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bu.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gg.asd995.cn

[N10] 链表节点定义
来源：http://jc.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qh.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fx.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sg.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rn.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://md.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jm.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://aq.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pb.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ss.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yz.huanxung.cn

PHP:  // 手写递归函数
来源：http://jk.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qg.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fa.szxytkj.cn

Java: // 手写递归
来源：http://yb.yuexingan06.cn

Go:   // 手写递归
来源：http://ci.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ux.huixinmuqiang.cn

C#:   // 手写递归
来源：http://yi.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zd.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mg.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zs.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xl.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zy.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://te.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tw.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zv.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fq.yuexingan06.cn

================================================================================
来源：http://rw.lnxyls.cn

O. 并发与异步
来源：http://vb.huixiangedu.cn

================================================================================
来源：http://jg.jctech888.com.cn

[O01] 启动一个线程
来源：http://jo.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tl.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://us.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uu.nicolike.cn

TS:   // 同 JS
来源：http://ot.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://gh.nicolike.cn

Go:   go f()
来源：http://dj.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://wi.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://li.hahajie.cn

[O02] 使用线程池
来源：http://qv.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://co.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://je.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://tt.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://jn.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bg.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://az.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ua.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ig.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://ha.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://jl.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://xb.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://df.huanxung.cn

TS:   // 同 JS
来源：http://uq.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://lz.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pc.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mb.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://yb.nicolike.cn

[O04] 定义异步函数并等待
来源：http://ef.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://lc.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oy.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://ph.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://js.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fh.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://us.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fy.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://vk.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://el.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://go.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://li.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://cf.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://qj.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nq.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xb.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ie.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bl.colortex.cn

[O06] 使用进程池
来源：http://gv.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sb.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qj.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://ss.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://az.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vn.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ur.shxzukj.cn

Ruby: // fork 块
来源：http://dg.huanxung.cn

C#:   Parallel.For
来源：http://iq.huanxung.cn

================================================================================
来源：http://hz.jctech888.com.cn

P. 常用工具函数
来源：http://pl.asd995.cn

================================================================================
来源：http://sc.newstarts.cn

[P01] 生成 UUID
来源：http://be.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://oo.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://or.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://dh.jianghongdianzi.cn


<!-- 参考信息 -->