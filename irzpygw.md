代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://pk.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wu.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ft.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kz.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bb.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kh.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hk.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rn.9csxet.cn

[L03] 设置自定义请求头
来源：http://nl.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jl.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://po.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pi.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://md.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ny.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ry.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qk.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qw.colortex.cn

[L04] 设置超时
来源：http://ua.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://fa.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dy.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kj.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mw.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hi.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xt.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dc.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://sd.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://db.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ja.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dn.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://to.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ou.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nu.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sb.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mr.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://na.shxzskj.cn

Py:   resp.json()
来源：http://vp.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://fq.nszjky.cn

JS:   await resp.json()
来源：http://nl.wgjwhj.cn

TS:   await resp.json()
来源：http://xs.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zh.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bm.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://me.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xf.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://ut.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rh.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cy.521024.cn

JS:   resp.ok;  resp.status
来源：http://qs.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ff.lnxyls.cn

Java: resp.statusCode()
来源：http://wt.szxytkj.cn

Go:   resp.StatusCode
来源：http://ix.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://qa.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ib.huanxung.cn

[L08] 并发请求多个地址
来源：http://qu.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dl.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://yv.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yo.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gj.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zd.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ky.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://je.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ge.newstarts.cn

================================================================================
来源：http://ax.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ae.9csxet.cn

================================================================================
来源：http://ac.nszjky.cn

[M01] 读取命令行参数
来源：http://gx.hahajie.cn

Py:   sys.argv[1:]
来源：http://tq.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://mt.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://hg.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://dz.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://yq.nszjky.cn

Go:   os.Args[1:]
来源：http://bu.szxytkj.cn

Ruby: ARGV
来源：http://ub.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://dd.haigaiapp.cn

[M02] 读取环境变量
来源：http://js.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://lj.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dj.hnjuh.cn

JS:   process.env.HOME
来源：http://ed.nicolike.cn

TS:   process.env.HOME
来源：http://pn.nszjky.cn

Java: System.getenv("HOME")
来源：http://tp.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://al.szsharing.cn

Ruby: ENV["HOME"]
来源：http://hp.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cq.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://jg.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://by.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bp.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aw.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vw.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rh.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ih.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sd.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://mq.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ye.szsharing.cn

Py:   os.getcwd()
来源：http://em.bjjhwx.cn

PHP:  getcwd();
来源：http://zz.huixinmuqiang.cn

JS:   process.cwd()
来源：http://pl.yuntaijiaju.cn

TS:   process.cwd()
来源：http://gz.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://gy.nicolike.cn

Go:   os.Getwd()
来源：http://bn.shtwfgs.cn

Ruby: Dir.pwd
来源：http://iq.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fx.asd995.cn

[M05] 设置退出码
来源：http://ca.panjiajie.cn

Py:   sys.exit(1)
来源：http://vz.szsharing.cn

PHP:  exit(1);
来源：http://ak.hnjuh.cn

JS:   process.exit(1)
来源：http://gt.521024.cn

TS:   process.exit(1)
来源：http://nb.yuexingan06.cn

Java: System.exit(1)
来源：http://wy.huanxung.cn

Go:   os.Exit(1)
来源：http://xf.jianghongdianzi.cn

Ruby: exit 1
来源：http://fo.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://en.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://sz.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://uj.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ay.nicolike.cn

JS:   console.error("err")
来源：http://pl.nicolike.cn

TS:   console.error("err")
来源：http://cn.wgjwhj.cn

Java: System.err.println("err")
来源：http://qs.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ob.shxzskj.cn

Ruby: warn "err"
来源：http://nh.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://gz.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://vv.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://dw.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.hnjuh.cn

JS:   require.main === module
来源：http://gc.hahajie.cn

TS:   require.main === module
来源：http://mw.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://hv.szxytkj.cn

Go:   func main()
来源：http://fq.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nb.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://th.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://le.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://zh.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://cf.colortex.cn

JS:   process.platform;  process.version
来源：http://hf.szxytkj.cn

TS:   process.platform;  process.version
来源：http://xx.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qt.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ic.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dz.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sm.chemitech.net.cn

================================================================================
来源：http://xb.panjiajie.cn

N. 数据结构与算法
来源：http://nx.lnxyls.cn

================================================================================
来源：http://uk.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://sf.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rp.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zk.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uz.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qu.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fv.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://qy.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rd.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kz.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://mt.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ac.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qv.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cy.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pd.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ma.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://vt.shxzukj.cn

Ruby: arr.sort
来源：http://tr.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oi.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://qi.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mm.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://zj.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jh.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mr.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gs.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qz.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wv.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ov.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://dv.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yb.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sv.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rw.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bb.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sl.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://il.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://do.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hf.muxihuayi.cn

[N05] 最大公约数
来源：http://bz.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://et.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://st.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://et.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kv.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ew.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zw.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://pi.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wd.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://wt.shxzskj.cn

Py:   s == s[::-1]
来源：http://is.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://oi.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://nk.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://tw.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://io.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ln.asd995.cn

Ruby: s == s.reverse
来源：http://df.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dv.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://nu.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uu.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cp.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ch.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://ev.chemitech.net.cn

Java: // 手写 HashMap
来源：http://fg.9csxet.cn

Go:   // 手写 map[int]int
来源：http://bp.shxzukj.cn

Ruby: // 手写 Hash
来源：http://zl.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zp.lnxyls.cn

[N08] 生成全排列
来源：http://nr.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ro.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ts.gzmigu.cn

JS:   // 手写回溯递归
来源：http://cq.szxytkj.cn

TS:   // 手写回溯递归
来源：http://pr.muxihuayi.cn

Java: // 手写回溯递归
来源：http://hi.hahajie.cn

Go:   // 手写回溯递归
来源：http://eg.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://md.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://pn.chemitech.net.cn

[N09] 栈与队列
来源：http://et.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://di.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lm.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yg.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://he.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zb.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yr.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yg.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zg.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://yu.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vd.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ee.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wl.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://to.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://dc.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fa.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pa.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ff.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ts.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pu.asd995.cn

PHP:  // 手写递归函数
来源：http://me.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://om.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lb.huixinmuqiang.cn

Java: // 手写递归
来源：http://ru.shxzukj.cn

Go:   // 手写递归
来源：http://ef.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qa.muxihuayi.cn

C#:   // 手写递归
来源：http://mf.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://or.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cl.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rg.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zt.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qh.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fy.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zb.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zm.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ti.haigaiapp.cn

================================================================================
来源：http://gj.hnjuh.cn

O. 并发与异步
来源：http://qj.panjiajie.cn

================================================================================
来源：http://li.newstarts.cn

[O01] 启动一个线程
来源：http://ex.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bo.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hh.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://av.muxihuayi.cn

TS:   // 同 JS
来源：http://ut.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://zt.lnxyls.cn

Go:   go f()
来源：http://be.9csxet.cn

Ruby: Thread.new { f }
来源：http://cy.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://pg.szxytkj.cn

[O02] 使用线程池
来源：http://ap.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wp.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ae.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://am.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://ot.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zw.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://as.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hq.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wv.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://jq.huanxung.cn

Py:   with lock: shared += 1
来源：http://fg.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://qf.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ww.hahajie.cn

TS:   // 同 JS
来源：http://gu.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://wj.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xe.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ab.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://tc.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://lm.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://bu.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qc.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://lf.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lb.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rh.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bv.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ff.colortex.cn

C#:   async Task F() { await G(); }
来源：http://nb.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://rc.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://mi.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ev.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://br.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://xx.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gp.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://if.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://up.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nq.lnxyls.cn

[O06] 使用进程池
来源：http://be.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://we.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wf.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://xo.shxzskj.cn


<!-- 参考信息 -->