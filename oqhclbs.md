代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://ir.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ln.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zw.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xl.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sq.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://or.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yl.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ve.shxzukj.cn

[L03] 设置自定义请求头
来源：http://uj.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://za.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yp.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eq.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://is.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kp.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gg.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bp.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oh.asd995.cn

[L04] 设置超时
来源：http://li.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://lr.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gz.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nb.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jw.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ko.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qh.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jg.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://mg.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lq.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hv.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nh.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wf.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bu.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yf.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tz.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://us.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://db.asd995.cn

Py:   resp.json()
来源：http://ov.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://dq.wgjwhj.cn

JS:   await resp.json()
来源：http://wg.asd995.cn

TS:   await resp.json()
来源：http://dg.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yi.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mo.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://hv.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tt.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://jq.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sp.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uf.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://ks.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://de.asd995.cn

Java: resp.statusCode()
来源：http://pd.huanxung.cn

Go:   resp.StatusCode
来源：http://wz.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://cx.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://dl.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://up.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ce.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://oc.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://np.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://no.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ww.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ux.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qh.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qd.9csxet.cn

================================================================================
来源：http://lo.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ti.nszjky.cn

================================================================================
来源：http://ap.haigaiapp.cn

[M01] 读取命令行参数
来源：http://uv.panjiajie.cn

Py:   sys.argv[1:]
来源：http://fz.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://px.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://fx.hahajie.cn

TS:   process.argv.slice(2)
来源：http://nu.colortex.cn

Java: args 数组（main 方法参数）
来源：http://ge.lnxyls.cn

Go:   os.Args[1:]
来源：http://qi.bookmarksfly.cn

Ruby: ARGV
来源：http://pt.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://pc.bookmarksfly.cn

[M02] 读取环境变量
来源：http://qp.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://fz.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://my.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://jv.chemitech.net.cn

TS:   process.env.HOME
来源：http://fi.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://vj.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rh.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://mt.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ca.chemitech.net.cn

[M03] 执行外部命令
来源：http://mp.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://io.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://so.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fw.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fn.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ja.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ix.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sf.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://zi.asd995.cn

[M04] 获取当前工作目录
来源：http://lq.lnxyls.cn

Py:   os.getcwd()
来源：http://hc.szxytkj.cn

PHP:  getcwd();
来源：http://mu.9csxet.cn

JS:   process.cwd()
来源：http://zm.jianghongdianzi.cn

TS:   process.cwd()
来源：http://la.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://yh.muxihuayi.cn

Go:   os.Getwd()
来源：http://bn.szxytkj.cn

Ruby: Dir.pwd
来源：http://sn.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tl.bookmarksfly.cn

[M05] 设置退出码
来源：http://kh.hnjuh.cn

Py:   sys.exit(1)
来源：http://ms.9csxet.cn

PHP:  exit(1);
来源：http://oe.shxzukj.cn

JS:   process.exit(1)
来源：http://ut.nszjky.cn

TS:   process.exit(1)
来源：http://px.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ld.shtwfgs.cn

Go:   os.Exit(1)
来源：http://qa.huixinmuqiang.cn

Ruby: exit 1
来源：http://aw.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xl.hnjuh.cn

[M06] 向标准错误输出
来源：http://az.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ya.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hq.jianghongdianzi.cn

JS:   console.error("err")
来源：http://pl.shxzskj.cn

TS:   console.error("err")
来源：http://up.huanxung.cn

Java: System.err.println("err")
来源：http://hn.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://st.szsharing.cn

Ruby: warn "err"
来源：http://ts.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://nc.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://wx.asd995.cn

Py:   if __name__ == "__main__":
来源：http://yf.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://so.hahajie.cn

JS:   require.main === module
来源：http://ho.lnxyls.cn

TS:   require.main === module
来源：http://zn.szsharing.cn

Java: public static void main(String[] args)
来源：http://gw.jianghongdianzi.cn

Go:   func main()
来源：http://nt.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vo.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://gz.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://gm.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://wx.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://kr.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://ia.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ju.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yw.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ku.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kv.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rg.haigaiapp.cn

================================================================================
来源：http://ph.nicolike.cn

N. 数据结构与算法
来源：http://ha.jctech888.com.cn

================================================================================
来源：http://ii.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://kc.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sx.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vq.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cy.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://du.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aj.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://pb.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://om.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://id.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gd.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ob.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sb.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zc.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jm.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://cy.yuexingan06.cn

Ruby: arr.sort
来源：http://in.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ul.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://na.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gq.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://ln.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oe.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wh.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ht.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qd.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rg.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ym.shxzukj.cn

[N04] 斐波那契数列
来源：http://ld.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ej.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://de.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yg.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xb.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ln.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pm.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rb.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rd.huixinmuqiang.cn

[N05] 最大公约数
来源：http://zm.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://dx.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wk.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wn.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sx.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fx.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gd.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://pl.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wd.chemitech.net.cn

[N06] 判断回文字符串
来源：http://py.huanxung.cn

Py:   s == s[::-1]
来源：http://zv.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://qk.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://qv.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://gf.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qv.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://rb.szsharing.cn

Ruby: s == s.reverse
来源：http://iv.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cq.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://zn.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ik.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dz.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kl.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://eo.hnjuh.cn

Java: // 手写 HashMap
来源：http://pn.hahajie.cn

Go:   // 手写 map[int]int
来源：http://bz.newstarts.cn

Ruby: // 手写 Hash
来源：http://ns.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gv.gzmigu.cn

[N08] 生成全排列
来源：http://pc.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://ak.panjiajie.cn

PHP:  // 手写递归交换
来源：http://uc.colortex.cn

JS:   // 手写回溯递归
来源：http://gv.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://zo.nszjky.cn

Java: // 手写回溯递归
来源：http://wk.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://af.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://xy.newstarts.cn

C#:   // 手写回溯递归
来源：http://de.yuexingan06.cn

[N09] 栈与队列
来源：http://of.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gv.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pr.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iu.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mv.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hy.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rr.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sd.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cx.muxihuayi.cn

[N10] 链表节点定义
来源：http://xb.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lz.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nf.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sa.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zd.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://by.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ag.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ih.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://af.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://cm.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qn.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://ty.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bd.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nr.hnjuh.cn

Java: // 手写递归
来源：http://vj.9csxet.cn

Go:   // 手写递归
来源：http://xn.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hd.yuexingan06.cn

C#:   // 手写递归
来源：http://oc.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cy.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pd.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://af.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rf.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oo.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sm.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pu.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dn.hnjuh.cn

================================================================================
来源：http://ck.yuntaijiaju.cn

O. 并发与异步
来源：http://by.9csxet.cn

================================================================================
来源：http://pp.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://yi.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nu.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cd.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://et.gzmigu.cn

TS:   // 同 JS
来源：http://cf.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://mk.panjiajie.cn

Go:   go f()
来源：http://fk.lnxyls.cn

Ruby: Thread.new { f }
来源：http://vs.colortex.cn

C#:   Task.Run(() => F());
来源：http://pq.shxzskj.cn

[O02] 使用线程池
来源：http://ol.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fe.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://gw.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://rw.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gl.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hq.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sm.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zp.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://ai.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://bs.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kg.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tj.szsharing.cn

TS:   // 同 JS
来源：http://fc.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://du.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ie.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gj.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ry.newstarts.cn

[O04] 定义异步函数并等待
来源：http://bx.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://kq.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://le.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://br.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sa.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://db.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://my.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ty.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ei.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://zn.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://ym.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cn.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://wr.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://ps.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ns.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://di.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://vs.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mj.newstarts.cn

[O06] 使用进程池
来源：http://ne.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nb.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ej.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://nb.panjiajie.cn


<!-- 参考信息 -->