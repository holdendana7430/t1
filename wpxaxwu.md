代发 wailian999

L. 网络请求
来源：http://gm.jctech888.com.cn

================================================================================
来源：http://sz.szsharing.cn

[L01] 发送 GET 请求
来源：http://gy.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ce.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rj.521024.cn

JS:   await fetch(url)
来源：http://ty.gzmigu.cn

TS:   await fetch(url)
来源：http://vs.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pg.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://mw.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://im.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hx.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://it.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gj.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qv.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vs.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qa.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xg.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bl.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zh.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://oz.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nk.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yl.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uu.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lm.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://do.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yh.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ui.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nt.chemitech.net.cn

[L04] 设置超时
来源：http://fj.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://mt.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qn.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mr.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wl.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zk.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gm.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wm.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://in.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jj.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nt.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sk.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ka.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://da.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mn.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tx.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ix.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://bm.lnxyls.cn

Py:   resp.json()
来源：http://rf.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ss.szxytkj.cn

JS:   await resp.json()
来源：http://vk.hnjuh.cn

TS:   await resp.json()
来源：http://hx.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bc.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qm.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://tz.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cl.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://uo.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ev.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yp.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://yz.colortex.cn

TS:   resp.ok;  resp.status
来源：http://oh.gzmigu.cn

Java: resp.statusCode()
来源：http://tx.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://vo.nszjky.cn

Ruby: resp.code.to_i
来源：http://tt.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://ex.shxzukj.cn

[L08] 并发请求多个地址
来源：http://zp.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hc.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://dk.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ii.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zo.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ca.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sr.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qz.bjjhwx.cn

================================================================================
来源：http://qd.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://el.shtwfgs.cn

================================================================================
来源：http://rh.haigaiapp.cn

[M01] 读取命令行参数
来源：http://qt.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://qe.nicolike.cn

PHP:  $argv;  $argc;
来源：http://gi.newstarts.cn

JS:   process.argv.slice(2)
来源：http://rr.asd995.cn

TS:   process.argv.slice(2)
来源：http://qh.521024.cn

Java: args 数组（main 方法参数）
来源：http://zi.bjjhwx.cn

Go:   os.Args[1:]
来源：http://ky.nicolike.cn

Ruby: ARGV
来源：http://ie.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://yk.szsharing.cn

[M02] 读取环境变量
来源：http://br.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://be.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kf.shxzukj.cn

JS:   process.env.HOME
来源：http://nk.yuexingan06.cn

TS:   process.env.HOME
来源：http://ss.colortex.cn

Java: System.getenv("HOME")
来源：http://ml.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nv.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://vo.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ij.9csxet.cn

[M03] 执行外部命令
来源：http://du.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zz.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cc.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sk.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kj.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nm.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gb.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bx.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://or.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://wt.jctech888.com.cn

Py:   os.getcwd()
来源：http://wx.yuntaijiaju.cn

PHP:  getcwd();
来源：http://xt.jctech888.com.cn

JS:   process.cwd()
来源：http://ig.jianghongdianzi.cn

TS:   process.cwd()
来源：http://sp.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://sz.lnxyls.cn

Go:   os.Getwd()
来源：http://kj.9csxet.cn

Ruby: Dir.pwd
来源：http://mk.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://px.gzmigu.cn

[M05] 设置退出码
来源：http://yh.9csxet.cn

Py:   sys.exit(1)
来源：http://hf.colortex.cn

PHP:  exit(1);
来源：http://wg.panjiajie.cn

JS:   process.exit(1)
来源：http://gh.nszjky.cn

TS:   process.exit(1)
来源：http://cv.yuexingan06.cn

Java: System.exit(1)
来源：http://nq.hnjuh.cn

Go:   os.Exit(1)
来源：http://oi.bjjhwx.cn

Ruby: exit 1
来源：http://xs.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ya.9csxet.cn

[M06] 向标准错误输出
来源：http://uz.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://so.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bq.colortex.cn

JS:   console.error("err")
来源：http://br.newstarts.cn

TS:   console.error("err")
来源：http://pd.szxytkj.cn

Java: System.err.println("err")
来源：http://kr.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pu.szsharing.cn

Ruby: warn "err"
来源：http://ys.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://vk.shxzukj.cn

[M07] 判断是否为主入口
来源：http://vi.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://ca.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xu.hahajie.cn

JS:   require.main === module
来源：http://fb.shtwfgs.cn

TS:   require.main === module
来源：http://ip.hahajie.cn

Java: public static void main(String[] args)
来源：http://ig.gzmigu.cn

Go:   func main()
来源：http://xb.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ia.szsharing.cn

C#:   static void Main(string[] args)
来源：http://uq.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://zc.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://rc.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://tw.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://io.521024.cn

TS:   process.platform;  process.version
来源：http://pt.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wu.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uh.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aw.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ch.huixiangedu.cn

================================================================================
来源：http://ee.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ym.nszjky.cn

================================================================================
来源：http://us.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://id.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://na.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://af.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zu.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aj.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://dn.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ci.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qa.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://yz.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mc.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kp.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kc.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ib.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wc.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ny.521024.cn

Ruby: arr.sort
来源：http://gj.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pc.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://cg.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pm.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://on.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ja.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gf.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zd.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xj.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nz.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zk.shxzskj.cn

[N04] 斐波那契数列
来源：http://ca.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pt.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xh.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://my.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ej.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://be.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yb.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rm.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dk.shtwfgs.cn

[N05] 最大公约数
来源：http://au.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://es.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mh.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lg.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cu.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://js.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vw.colortex.cn

Ruby: a.gcd(b)
来源：http://sd.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ub.chemitech.net.cn

[N06] 判断回文字符串
来源：http://gu.szxytkj.cn

Py:   s == s[::-1]
来源：http://wa.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://bi.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://si.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://gz.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wu.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://wh.shxzskj.cn

Ruby: s == s.reverse
来源：http://vv.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ck.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://xg.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ya.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://va.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rk.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://ic.haigaiapp.cn

Java: // 手写 HashMap
来源：http://nh.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://nx.asd995.cn

Ruby: // 手写 Hash
来源：http://ei.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vw.colortex.cn

[N08] 生成全排列
来源：http://sy.asd995.cn

Py:   itertools.permutations(arr)
来源：http://cr.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://un.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://av.colortex.cn

TS:   // 手写回溯递归
来源：http://ts.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://lc.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://jd.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://nb.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://xs.yuntaijiaju.cn

[N09] 栈与队列
来源：http://hx.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bt.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qx.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dq.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wk.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fo.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://il.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xo.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sf.bookmarksfly.cn

[N10] 链表节点定义
来源：http://ln.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vk.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://um.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sb.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wp.521024.cn

Java: class Node { int v; Node next; }
来源：http://yn.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lb.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://it.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ct.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://rq.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qy.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://qc.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dl.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pz.nicolike.cn

Java: // 手写递归
来源：http://ko.shtwfgs.cn

Go:   // 手写递归
来源：http://yz.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cl.colortex.cn

C#:   // 手写递归
来源：http://wr.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kq.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yw.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rc.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nt.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xw.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dv.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hs.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dm.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ed.bjjhwx.cn

================================================================================
来源：http://lp.haigaiapp.cn

O. 并发与异步
来源：http://yo.panjiajie.cn

================================================================================
来源：http://ld.newstarts.cn

[O01] 启动一个线程
来源：http://vm.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yo.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eg.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dw.9csxet.cn

TS:   // 同 JS
来源：http://gb.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://vh.szxytkj.cn

Go:   go f()
来源：http://by.szsharing.cn

Ruby: Thread.new { f }
来源：http://qf.colortex.cn

C#:   Task.Run(() => F());
来源：http://sa.lnxyls.cn

[O02] 使用线程池
来源：http://ym.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zd.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://da.newstarts.cn

JS:   // worker_threads 线程池
来源：http://af.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://oy.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hw.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oo.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zu.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fb.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://bv.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://tj.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://sg.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zy.gzmigu.cn

TS:   // 同 JS
来源：http://hd.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://qv.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qn.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pq.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://jv.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ru.colortex.cn

Py:   async def f():⏎    await g()
来源：http://qh.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rh.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://tc.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ki.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dw.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nt.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tw.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://io.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ml.hnjuh.cn


<!-- 参考信息 -->