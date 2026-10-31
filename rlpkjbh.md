代发 wailian999

L. 网络请求
来源：http://cz.lnxyls.cn

================================================================================
来源：http://rv.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://oh.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ps.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gh.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://im.huanxung.cn

TS:   await fetch(url)
来源：http://sl.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fl.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://gf.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cb.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rn.hahajie.cn

[L02] 发送 POST JSON
来源：http://ws.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dr.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://be.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fk.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xa.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kv.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wn.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://me.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://ss.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://os.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gp.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pt.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ur.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hg.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qa.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hi.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://os.nszjky.cn

[L04] 设置超时
来源：http://vc.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://ra.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ue.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dn.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qn.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wx.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cq.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ey.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://px.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://jd.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qh.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uk.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fj.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zx.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yf.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uh.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jm.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sx.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://xi.521024.cn

Py:   resp.json()
来源：http://ej.newstarts.cn

PHP:  json_decode($body, true);
来源：http://yf.yuexingan06.cn

JS:   await resp.json()
来源：http://kt.huixinmuqiang.cn

TS:   await resp.json()
来源：http://mz.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dm.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://br.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://ee.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rh.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://wr.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://li.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ym.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://uv.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://oy.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://bj.hahajie.cn

Go:   resp.StatusCode
来源：http://ua.shxzukj.cn

Ruby: resp.code.to_i
来源：http://hy.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://vz.newstarts.cn

[L08] 并发请求多个地址
来源：http://yl.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dv.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://kx.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://md.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eu.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://un.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oj.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://um.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zf.bjjhwx.cn

================================================================================
来源：http://az.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://nb.szxytkj.cn

================================================================================
来源：http://op.shtwfgs.cn

[M01] 读取命令行参数
来源：http://nu.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://ye.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ji.huanxung.cn

JS:   process.argv.slice(2)
来源：http://kw.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://la.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yp.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://lv.hahajie.cn

Ruby: ARGV
来源：http://rb.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://dv.jctech888.com.cn

[M02] 读取环境变量
来源：http://hi.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://tn.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gs.9csxet.cn

JS:   process.env.HOME
来源：http://ln.gzmigu.cn

TS:   process.env.HOME
来源：http://bx.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://hh.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://um.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://te.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dz.haigaiapp.cn

[M03] 执行外部命令
来源：http://ih.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rx.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ox.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mw.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ic.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uv.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mc.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tj.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://pk.nicolike.cn

[M04] 获取当前工作目录
来源：http://ya.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://tm.nszjky.cn

PHP:  getcwd();
来源：http://me.bjjhwx.cn

JS:   process.cwd()
来源：http://ha.bookmarksfly.cn

TS:   process.cwd()
来源：http://yx.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://up.muxihuayi.cn

Go:   os.Getwd()
来源：http://yb.chemitech.net.cn

Ruby: Dir.pwd
来源：http://gd.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ff.hnjuh.cn

[M05] 设置退出码
来源：http://qz.muxihuayi.cn

Py:   sys.exit(1)
来源：http://qx.521024.cn

PHP:  exit(1);
来源：http://ep.gzmigu.cn

JS:   process.exit(1)
来源：http://tn.521024.cn

TS:   process.exit(1)
来源：http://zt.colortex.cn

Java: System.exit(1)
来源：http://hv.jctech888.com.cn

Go:   os.Exit(1)
来源：http://sw.shxzukj.cn

Ruby: exit 1
来源：http://dk.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zv.huixiangedu.cn

[M06] 向标准错误输出
来源：http://sr.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://xy.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dj.lnxyls.cn

JS:   console.error("err")
来源：http://ut.shxzukj.cn

TS:   console.error("err")
来源：http://xz.newstarts.cn

Java: System.err.println("err")
来源：http://yk.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qg.bjjhwx.cn

Ruby: warn "err"
来源：http://fh.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://nd.szxytkj.cn

[M07] 判断是否为主入口
来源：http://os.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://pl.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gu.shtwfgs.cn

JS:   require.main === module
来源：http://hi.newstarts.cn

TS:   require.main === module
来源：http://go.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://pc.yuexingan06.cn

Go:   func main()
来源：http://kn.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qi.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://yd.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://bv.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://vh.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://hh.huanxung.cn

JS:   process.platform;  process.version
来源：http://kh.hnjuh.cn

TS:   process.platform;  process.version
来源：http://wo.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kq.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ys.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uh.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mu.shxzukj.cn

================================================================================
来源：http://tf.huanxung.cn

N. 数据结构与算法
来源：http://ps.colortex.cn

================================================================================
来源：http://kh.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://ol.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cn.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nb.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dl.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vg.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://et.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ve.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xg.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://gb.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://cn.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://or.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sh.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ku.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wz.newstarts.cn

Go:   slices.Sort(arr)
来源：http://ks.shxzskj.cn

Ruby: arr.sort
来源：http://im.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://we.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://th.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wi.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://oz.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yi.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yr.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://og.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kq.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yt.yuexingan06.cn

[N04] 斐波那契数列
来源：http://wr.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ag.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://if.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ux.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kw.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ln.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tx.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://da.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yp.asd995.cn

[N05] 最大公约数
来源：http://zi.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://vj.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fp.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lt.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eb.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vp.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://xz.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kc.szsharing.cn

[N06] 判断回文字符串
来源：http://wu.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://yc.521024.cn

PHP:  $s === strrev($s);
来源：http://yc.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://uo.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://xc.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pz.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ta.hnjuh.cn

Ruby: s == s.reverse
来源：http://bt.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mv.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://ut.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oo.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://da.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pe.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://dk.gzmigu.cn

Java: // 手写 HashMap
来源：http://yv.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://nq.hahajie.cn

Ruby: // 手写 Hash
来源：http://wl.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tw.hnjuh.cn

[N08] 生成全排列
来源：http://sh.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://qs.asd995.cn

PHP:  // 手写递归交换
来源：http://eg.hahajie.cn

JS:   // 手写回溯递归
来源：http://fi.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://in.yuexingan06.cn

Java: // 手写回溯递归
来源：http://hj.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://mn.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://og.gzmigu.cn

C#:   // 手写回溯递归
来源：http://pb.huixinmuqiang.cn

[N09] 栈与队列
来源：http://vh.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mm.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kc.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iz.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wt.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dq.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fo.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ek.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oa.lnxyls.cn

[N10] 链表节点定义
来源：http://st.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qp.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rd.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sb.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xh.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://wd.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oz.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wx.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zt.9csxet.cn

[N11] 二叉树中序遍历
来源：http://mk.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gn.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://yj.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xh.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ed.521024.cn

Java: // 手写递归
来源：http://sv.lnxyls.cn

Go:   // 手写递归
来源：http://ki.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wy.szxytkj.cn

C#:   // 手写递归
来源：http://ta.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ae.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://la.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://us.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tm.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ay.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ke.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dy.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://md.szsharing.cn

================================================================================
来源：http://fr.huanxung.cn

O. 并发与异步
来源：http://hb.bjjhwx.cn

================================================================================
来源：http://ki.huixiangedu.cn

[O01] 启动一个线程
来源：http://de.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ev.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nx.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://da.bookmarksfly.cn

TS:   // 同 JS
来源：http://hq.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://tq.jianghongdianzi.cn

Go:   go f()
来源：http://kl.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://ob.huanxung.cn

C#:   Task.Run(() => F());
来源：http://ti.newstarts.cn

[O02] 使用线程池
来源：http://wh.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zl.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ty.szsharing.cn

JS:   // worker_threads 线程池
来源：http://xk.szsharing.cn

TS:   // worker_threads 线程池
来源：http://lw.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nt.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tb.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ss.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://xg.nicolike.cn

Py:   with lock: shared += 1
来源：http://tb.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://zy.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rk.huanxung.cn

TS:   // 同 JS
来源：http://sf.521024.cn

Java: synchronized (this) { shared++; }
来源：http://cr.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wz.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vv.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://vd.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://nz.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://kh.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://je.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://wq.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gu.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wr.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uw.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eg.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://rb.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://cf.newstarts.cn


<!-- 参考信息 -->