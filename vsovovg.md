代发 wailian999

Go:   encoding/gob
来源：http://dx.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://as.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ni.huixinmuqiang.cn

================================================================================
来源：http://gp.521024.cn

L. 网络请求
来源：http://cx.shtwfgs.cn

================================================================================
来源：http://ib.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ff.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tp.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://st.szxytkj.cn

JS:   await fetch(url)
来源：http://xh.9csxet.cn

TS:   await fetch(url)
来源：http://zk.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ts.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://sz.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aa.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ke.panjiajie.cn

[L02] 发送 POST JSON
来源：http://aj.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vq.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ba.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rm.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rh.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jo.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qa.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ce.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ut.huanxung.cn

[L03] 设置自定义请求头
来源：http://wy.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kl.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xx.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cb.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wf.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nd.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://no.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ke.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ng.hahajie.cn

[L04] 设置超时
来源：http://ci.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://lf.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zk.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ey.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aa.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hy.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iz.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ym.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ih.521024.cn

[L05] 上传文件（multipart）
来源：http://kb.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vo.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mt.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://if.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iw.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kh.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wl.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lg.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ro.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://ts.muxihuayi.cn

Py:   resp.json()
来源：http://om.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ek.hnjuh.cn

JS:   await resp.json()
来源：http://xh.521024.cn

TS:   await resp.json()
来源：http://fr.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sv.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mm.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://sz.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ti.521024.cn

[L07] 处理 HTTP 状态码
来源：http://pv.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cc.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pw.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://ua.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://sv.9csxet.cn

Java: resp.statusCode()
来源：http://hg.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://cs.huanxung.cn

Ruby: resp.code.to_i
来源：http://gc.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://bo.hnjuh.cn

[L08] 并发请求多个地址
来源：http://oa.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nu.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://mf.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kw.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ea.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ro.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zb.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ja.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gg.panjiajie.cn

================================================================================
来源：http://tb.521024.cn

M. 命令行 / 进程 / 环境
来源：http://aa.nicolike.cn

================================================================================
来源：http://tp.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://xh.shxzukj.cn

Py:   sys.argv[1:]
来源：http://fx.szsharing.cn

PHP:  $argv;  $argc;
来源：http://cm.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://ec.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://mv.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yv.shtwfgs.cn

Go:   os.Args[1:]
来源：http://wb.shxzukj.cn

Ruby: ARGV
来源：http://xq.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://it.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://zc.asd995.cn

Py:   os.environ.get("HOME")
来源：http://tu.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lc.shxzukj.cn

JS:   process.env.HOME
来源：http://ru.panjiajie.cn

TS:   process.env.HOME
来源：http://pa.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ob.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://st.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://af.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://df.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://le.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gq.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vv.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xa.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gy.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://is.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://no.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://et.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://cm.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://cm.huixiangedu.cn

Py:   os.getcwd()
来源：http://gv.hnjuh.cn

PHP:  getcwd();
来源：http://nv.colortex.cn

JS:   process.cwd()
来源：http://qb.yuntaijiaju.cn

TS:   process.cwd()
来源：http://dn.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bf.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://ch.huixiangedu.cn

Ruby: Dir.pwd
来源：http://wg.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xr.9csxet.cn

[M05] 设置退出码
来源：http://qy.shtwfgs.cn

Py:   sys.exit(1)
来源：http://xs.bjjhwx.cn

PHP:  exit(1);
来源：http://qm.huanxung.cn

JS:   process.exit(1)
来源：http://ka.9csxet.cn

TS:   process.exit(1)
来源：http://lb.muxihuayi.cn

Java: System.exit(1)
来源：http://sh.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://so.panjiajie.cn

Ruby: exit 1
来源：http://cv.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ve.nszjky.cn

[M06] 向标准错误输出
来源：http://qr.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ml.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ud.shxzskj.cn

JS:   console.error("err")
来源：http://qa.chemitech.net.cn

TS:   console.error("err")
来源：http://rz.bookmarksfly.cn

Java: System.err.println("err")
来源：http://uu.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zi.chemitech.net.cn

Ruby: warn "err"
来源：http://oh.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://dq.gzmigu.cn

[M07] 判断是否为主入口
来源：http://gh.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://so.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://me.panjiajie.cn

JS:   require.main === module
来源：http://qf.jctech888.com.cn

TS:   require.main === module
来源：http://lx.shxzskj.cn

Java: public static void main(String[] args)
来源：http://jb.bjjhwx.cn

Go:   func main()
来源：http://ra.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bh.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ns.asd995.cn

[M08] 获取系统与运行时信息
来源：http://ya.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://wc.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://en.nicolike.cn

JS:   process.platform;  process.version
来源：http://pl.szsharing.cn

TS:   process.platform;  process.version
来源：http://of.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gb.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mz.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zr.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zt.jianghongdianzi.cn

================================================================================
来源：http://kg.shxzukj.cn

N. 数据结构与算法
来源：http://zt.yuexingan06.cn

================================================================================
来源：http://kn.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://pf.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ju.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rq.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zx.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ed.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xz.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ij.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ix.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tt.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://ci.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://oe.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vz.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wm.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tx.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hu.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://nf.huanxung.cn

Ruby: arr.sort
来源：http://pz.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ho.521024.cn

[N03] 快速排序（分治示例）
来源：http://ge.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uk.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://fl.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ij.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ov.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lx.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ry.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ey.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://be.chemitech.net.cn

[N04] 斐波那契数列
来源：http://pe.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gc.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qe.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ni.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jo.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xx.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hg.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bo.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tc.bookmarksfly.cn

[N05] 最大公约数
来源：http://ng.newstarts.cn

Py:   math.gcd(a, b)
来源：http://db.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zc.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ra.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qf.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://em.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rz.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://ns.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fl.asd995.cn

[N06] 判断回文字符串
来源：http://fs.hnjuh.cn

Py:   s == s[::-1]
来源：http://ch.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://nv.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://nw.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://vy.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jn.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://jq.gzmigu.cn

Ruby: s == s.reverse
来源：http://xl.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mn.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://va.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qe.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rg.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ih.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://st.wgjwhj.cn

Java: // 手写 HashMap
来源：http://ym.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://sv.9csxet.cn

Ruby: // 手写 Hash
来源：http://jg.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pn.huixinmuqiang.cn

[N08] 生成全排列
来源：http://da.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://ad.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://cc.lnxyls.cn

JS:   // 手写回溯递归
来源：http://yv.szxytkj.cn

TS:   // 手写回溯递归
来源：http://im.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://lr.szxytkj.cn

Go:   // 手写回溯递归
来源：http://vu.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://sl.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://cn.bjjhwx.cn

[N09] 栈与队列
来源：http://mg.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xy.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://em.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lu.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bg.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yl.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ey.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ap.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cf.chemitech.net.cn

[N10] 链表节点定义
来源：http://pb.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wm.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eg.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ao.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ej.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://hc.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://do.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://id.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tp.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://lo.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wv.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://ol.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rr.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rd.nicolike.cn

Java: // 手写递归
来源：http://af.szxytkj.cn

Go:   // 手写递归
来源：http://nl.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hq.szsharing.cn

C#:   // 手写递归
来源：http://me.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hh.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xe.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pi.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pj.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://al.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jt.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rj.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tj.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gg.haigaiapp.cn

================================================================================
来源：http://bu.muxihuayi.cn

O. 并发与异步
来源：http://ly.wgjwhj.cn

================================================================================
来源：http://eo.asd995.cn

[O01] 启动一个线程
来源：http://oa.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ns.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ig.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xh.wgjwhj.cn

TS:   // 同 JS
来源：http://bf.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://xy.huixinmuqiang.cn

Go:   go f()
来源：http://kb.9csxet.cn

Ruby: Thread.new { f }
来源：http://fa.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://ud.shxzukj.cn

[O02] 使用线程池
来源：http://vr.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bx.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gg.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://yz.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://kr.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://px.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pc.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lz.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ne.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://tq.colortex.cn

Py:   with lock: shared += 1
来源：http://rk.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://tv.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jc.chemitech.net.cn

TS:   // 同 JS
来源：http://it.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://qq.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gp.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bv.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ag.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://xd.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://hi.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lh.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://cq.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://td.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eo.bookmarksfly.cn


<!-- 参考信息 -->