代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ps.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://oi.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://kr.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fb.nszjky.cn

Go:   encoding/gob
来源：http://qp.521024.cn

Ruby: Marshal.dump(obj)
来源：http://wm.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://da.wgjwhj.cn

================================================================================
来源：http://or.haigaiapp.cn

L. 网络请求
来源：http://xf.hnjuh.cn

================================================================================
来源：http://fe.shxzukj.cn

[L01] 发送 GET 请求
来源：http://sz.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://js.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://in.hnjuh.cn

JS:   await fetch(url)
来源：http://bn.gzmigu.cn

TS:   await fetch(url)
来源：http://gy.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hb.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://br.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pr.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rw.nicolike.cn

[L02] 发送 POST JSON
来源：http://xz.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nn.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fe.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ax.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wd.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gm.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bx.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rz.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ka.nicolike.cn

[L03] 设置自定义请求头
来源：http://hm.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://au.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gw.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vs.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://te.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xw.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wz.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gc.521024.cn

[L04] 设置超时
来源：http://qa.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://hj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rt.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qb.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lm.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://op.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ul.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ce.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wg.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://qn.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ng.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tk.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xs.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nz.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://of.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iw.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://js.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ys.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://dx.shxzskj.cn

Py:   resp.json()
来源：http://xk.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ja.muxihuayi.cn

JS:   await resp.json()
来源：http://hu.chemitech.net.cn

TS:   await resp.json()
来源：http://bl.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uj.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pq.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://nk.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ta.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://bi.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://md.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lo.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://vs.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ew.muxihuayi.cn

Java: resp.statusCode()
来源：http://yg.yuexingan06.cn

Go:   resp.StatusCode
来源：http://xt.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://to.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://ub.lnxyls.cn

[L08] 并发请求多个地址
来源：http://oe.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cs.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ux.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vo.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gf.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sn.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zz.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xm.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://js.bjjhwx.cn

================================================================================
来源：http://pn.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://tj.chemitech.net.cn

================================================================================
来源：http://ee.jctech888.com.cn

[M01] 读取命令行参数
来源：http://xw.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://lk.newstarts.cn

PHP:  $argv;  $argc;
来源：http://zv.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://po.nszjky.cn

TS:   process.argv.slice(2)
来源：http://wb.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://ap.jctech888.com.cn

Go:   os.Args[1:]
来源：http://hh.huanxung.cn

Ruby: ARGV
来源：http://vb.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ky.colortex.cn

[M02] 读取环境变量
来源：http://tg.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://uj.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uk.haigaiapp.cn

JS:   process.env.HOME
来源：http://bz.wgjwhj.cn

TS:   process.env.HOME
来源：http://gl.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://op.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dj.asd995.cn

Ruby: ENV["HOME"]
来源：http://be.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://so.colortex.cn

[M03] 执行外部命令
来源：http://mt.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zf.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nl.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mt.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rl.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fv.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cg.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bz.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://wf.hnjuh.cn

[M04] 获取当前工作目录
来源：http://zm.wgjwhj.cn

Py:   os.getcwd()
来源：http://ve.hnjuh.cn

PHP:  getcwd();
来源：http://xv.haigaiapp.cn

JS:   process.cwd()
来源：http://rh.yuntaijiaju.cn

TS:   process.cwd()
来源：http://xg.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://aw.521024.cn

Go:   os.Getwd()
来源：http://tj.shxzukj.cn

Ruby: Dir.pwd
来源：http://gt.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vj.panjiajie.cn

[M05] 设置退出码
来源：http://co.panjiajie.cn

Py:   sys.exit(1)
来源：http://jn.newstarts.cn

PHP:  exit(1);
来源：http://km.lnxyls.cn

JS:   process.exit(1)
来源：http://go.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://sl.huixiangedu.cn

Java: System.exit(1)
来源：http://ep.shtwfgs.cn

Go:   os.Exit(1)
来源：http://rx.newstarts.cn

Ruby: exit 1
来源：http://hu.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bz.nicolike.cn

[M06] 向标准错误输出
来源：http://bx.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://pi.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dx.szxytkj.cn

JS:   console.error("err")
来源：http://sz.bookmarksfly.cn

TS:   console.error("err")
来源：http://za.nicolike.cn

Java: System.err.println("err")
来源：http://hh.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tf.panjiajie.cn

Ruby: warn "err"
来源：http://vm.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://kt.colortex.cn

[M07] 判断是否为主入口
来源：http://ru.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://nj.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rq.panjiajie.cn

JS:   require.main === module
来源：http://aj.bookmarksfly.cn

TS:   require.main === module
来源：http://pg.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://aj.yuntaijiaju.cn

Go:   func main()
来源：http://ms.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bl.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://me.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://lu.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ow.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://cs.asd995.cn

JS:   process.platform;  process.version
来源：http://zm.shxzskj.cn

TS:   process.platform;  process.version
来源：http://kc.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eo.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oa.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fa.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eh.huixiangedu.cn

================================================================================
来源：http://mw.szsharing.cn

N. 数据结构与算法
来源：http://kt.nszjky.cn

================================================================================
来源：http://iz.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://on.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://li.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wi.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xs.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vb.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://be.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fp.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ph.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ut.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ww.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hf.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ab.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tc.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://br.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://xz.bookmarksfly.cn

Ruby: arr.sort
来源：http://lv.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wo.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://gi.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://br.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://yw.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pu.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lb.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oa.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zo.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cg.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cn.huixiangedu.cn

[N04] 斐波那契数列
来源：http://gp.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hy.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ls.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://km.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jr.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ci.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wl.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wc.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vw.yuntaijiaju.cn

[N05] 最大公约数
来源：http://pf.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://yr.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://me.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ml.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tu.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lh.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://ub.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zb.newstarts.cn

[N06] 判断回文字符串
来源：http://mu.chemitech.net.cn

Py:   s == s[::-1]
来源：http://uo.szsharing.cn

PHP:  $s === strrev($s);
来源：http://rm.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://fo.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://dp.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fi.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://gw.panjiajie.cn

Ruby: s == s.reverse
来源：http://zx.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lr.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://ww.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fm.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pr.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xd.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://pc.shxzskj.cn

Java: // 手写 HashMap
来源：http://gk.nicolike.cn

Go:   // 手写 map[int]int
来源：http://tv.shxzukj.cn

Ruby: // 手写 Hash
来源：http://rk.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eb.yuexingan06.cn

[N08] 生成全排列
来源：http://tq.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://qo.9csxet.cn

PHP:  // 手写递归交换
来源：http://dh.521024.cn

JS:   // 手写回溯递归
来源：http://mj.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://jh.huixiangedu.cn

Java: // 手写回溯递归
来源：http://cr.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://qr.521024.cn

Ruby: arr.permutation.to_a
来源：http://fm.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://pr.jctech888.com.cn

[N09] 栈与队列
来源：http://xi.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mi.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nb.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ov.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ke.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ml.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uv.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://di.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://es.shxzukj.cn

[N10] 链表节点定义
来源：http://gd.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xs.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pi.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ai.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oo.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://si.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aq.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oo.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aj.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://hu.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zu.9csxet.cn

PHP:  // 手写递归函数
来源：http://ib.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qv.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ts.yuexingan06.cn

Java: // 手写递归
来源：http://gs.colortex.cn

Go:   // 手写递归
来源：http://nc.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gl.lnxyls.cn

C#:   // 手写递归
来源：http://dg.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cx.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fm.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ae.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gj.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cs.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wn.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hb.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nr.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gr.huixiangedu.cn

================================================================================
来源：http://fd.szxytkj.cn

O. 并发与异步
来源：http://ih.jianghongdianzi.cn

================================================================================
来源：http://yb.hahajie.cn

[O01] 启动一个线程
来源：http://wh.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lb.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xi.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ol.nicolike.cn

TS:   // 同 JS
来源：http://pj.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://gu.hahajie.cn

Go:   go f()
来源：http://ez.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://mt.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://nw.muxihuayi.cn

[O02] 使用线程池
来源：http://zt.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qh.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kn.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://sq.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://ah.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://au.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tj.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xj.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://da.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://xn.shxzukj.cn

Py:   with lock: shared += 1
来源：http://to.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://se.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dj.panjiajie.cn

TS:   // 同 JS
来源：http://vx.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://zd.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://br.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fs.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://ka.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://cu.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://yr.hnjuh.cn


<!-- 参考信息 -->