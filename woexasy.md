代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ap.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://sb.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://uy.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://if.haigaiapp.cn

Go:   encoding/gob
来源：http://nb.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://dw.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ai.asd995.cn

================================================================================
来源：http://hn.shtwfgs.cn

L. 网络请求
来源：http://ad.jianghongdianzi.cn

================================================================================
来源：http://ag.shxzukj.cn

[L01] 发送 GET 请求
来源：http://nk.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xa.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uq.shxzskj.cn

JS:   await fetch(url)
来源：http://cd.asd995.cn

TS:   await fetch(url)
来源：http://aa.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ag.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://wi.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sr.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tq.9csxet.cn

[L02] 发送 POST JSON
来源：http://yw.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wh.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vt.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yq.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ru.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://go.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ln.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cv.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mc.nszjky.cn

[L03] 设置自定义请求头
来源：http://is.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sh.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pu.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wl.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gu.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tg.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vp.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qc.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://we.szxytkj.cn

[L04] 设置超时
来源：http://qx.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://xk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pk.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uc.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dc.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ut.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hc.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wv.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://el.hahajie.cn

[L05] 上传文件（multipart）
来源：http://ou.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ll.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bl.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uc.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ju.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jl.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ac.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hb.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wl.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://du.9csxet.cn

Py:   resp.json()
来源：http://hk.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://sl.asd995.cn

JS:   await resp.json()
来源：http://ta.9csxet.cn

TS:   await resp.json()
来源：http://vv.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ht.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lw.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://gd.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qp.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://qn.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wg.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kp.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://eb.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://pe.muxihuayi.cn

Java: resp.statusCode()
来源：http://jj.hnjuh.cn

Go:   resp.StatusCode
来源：http://cd.colortex.cn

Ruby: resp.code.to_i
来源：http://nh.521024.cn

C#:   (int)resp.StatusCode
来源：http://wg.9csxet.cn

[L08] 并发请求多个地址
来源：http://kr.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ow.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://fi.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yh.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pd.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mn.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zc.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://et.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kn.jctech888.com.cn

================================================================================
来源：http://os.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://xa.bjjhwx.cn

================================================================================
来源：http://lq.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://aa.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://bb.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://in.newstarts.cn

JS:   process.argv.slice(2)
来源：http://tv.huanxung.cn

TS:   process.argv.slice(2)
来源：http://vs.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://hx.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://nz.shxzskj.cn

Ruby: ARGV
来源：http://sc.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://cd.hahajie.cn

[M02] 读取环境变量
来源：http://xy.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://mh.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lu.hnjuh.cn

JS:   process.env.HOME
来源：http://vp.9csxet.cn

TS:   process.env.HOME
来源：http://ee.hnjuh.cn

Java: System.getenv("HOME")
来源：http://op.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://su.huanxung.cn

Ruby: ENV["HOME"]
来源：http://bl.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pd.yuexingan06.cn

[M03] 执行外部命令
来源：http://qm.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mo.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yo.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hx.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://te.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ru.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ks.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tw.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://hz.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://rn.gzmigu.cn

Py:   os.getcwd()
来源：http://ft.gzmigu.cn

PHP:  getcwd();
来源：http://sr.szsharing.cn

JS:   process.cwd()
来源：http://sq.lnxyls.cn

TS:   process.cwd()
来源：http://vu.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://qh.gzmigu.cn

Go:   os.Getwd()
来源：http://gw.newstarts.cn

Ruby: Dir.pwd
来源：http://jt.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zb.szsharing.cn

[M05] 设置退出码
来源：http://ai.shxzskj.cn

Py:   sys.exit(1)
来源：http://yq.shxzukj.cn

PHP:  exit(1);
来源：http://qx.gzmigu.cn

JS:   process.exit(1)
来源：http://ub.huanxung.cn

TS:   process.exit(1)
来源：http://rl.521024.cn

Java: System.exit(1)
来源：http://im.jctech888.com.cn

Go:   os.Exit(1)
来源：http://no.szsharing.cn

Ruby: exit 1
来源：http://st.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nf.nszjky.cn

[M06] 向标准错误输出
来源：http://uf.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://xe.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zj.hnjuh.cn

JS:   console.error("err")
来源：http://wn.yuntaijiaju.cn

TS:   console.error("err")
来源：http://wu.szsharing.cn

Java: System.err.println("err")
来源：http://wg.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qk.huixinmuqiang.cn

Ruby: warn "err"
来源：http://wo.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://zt.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://wb.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://mn.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tj.wgjwhj.cn

JS:   require.main === module
来源：http://kf.haigaiapp.cn

TS:   require.main === module
来源：http://ce.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ij.chemitech.net.cn

Go:   func main()
来源：http://ch.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hr.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://lt.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://cn.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://ll.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://bb.colortex.cn

JS:   process.platform;  process.version
来源：http://zb.colortex.cn

TS:   process.platform;  process.version
来源：http://tf.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fc.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nb.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tn.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rf.shxzukj.cn

================================================================================
来源：http://iu.bookmarksfly.cn

N. 数据结构与算法
来源：http://gl.nicolike.cn

================================================================================
来源：http://af.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://ez.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vt.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zg.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vi.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bh.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bk.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://jl.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ye.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jh.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://xa.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ne.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lf.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hx.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lk.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dy.colortex.cn

Go:   slices.Sort(arr)
来源：http://wr.shxzskj.cn

Ruby: arr.sort
来源：http://jq.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://in.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://qw.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ah.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://kt.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uk.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://da.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fp.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zp.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ya.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://il.jctech888.com.cn

[N04] 斐波那契数列
来源：http://lj.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xd.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tn.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xo.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jt.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://at.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aj.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qo.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yb.haigaiapp.cn

[N05] 最大公约数
来源：http://ic.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://hq.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ix.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yq.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bi.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hn.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qn.shxzskj.cn

Ruby: a.gcd(b)
来源：http://dg.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ns.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://fo.9csxet.cn

Py:   s == s[::-1]
来源：http://tb.asd995.cn

PHP:  $s === strrev($s);
来源：http://dq.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://zk.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://nk.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lz.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://dl.gzmigu.cn

Ruby: s == s.reverse
来源：http://mh.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://do.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://sx.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kk.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gd.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dd.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://ld.lnxyls.cn

Java: // 手写 HashMap
来源：http://lf.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://nr.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://xm.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wq.gzmigu.cn

[N08] 生成全排列
来源：http://wz.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://bb.asd995.cn

PHP:  // 手写递归交换
来源：http://ms.hahajie.cn

JS:   // 手写回溯递归
来源：http://ry.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://ae.hnjuh.cn

Java: // 手写回溯递归
来源：http://sy.hahajie.cn

Go:   // 手写回溯递归
来源：http://io.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://sh.gzmigu.cn

C#:   // 手写回溯递归
来源：http://lu.huixiangedu.cn

[N09] 栈与队列
来源：http://mo.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tk.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rf.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://di.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zo.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xo.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sq.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tu.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ny.521024.cn

[N10] 链表节点定义
来源：http://ym.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yb.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tz.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zp.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://os.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://jx.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tg.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ie.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gu.asd995.cn

[N11] 二叉树中序遍历
来源：http://mz.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pi.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://bo.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ou.huixinmuqiang.cn

Java: // 手写递归
来源：http://pd.yuntaijiaju.cn

Go:   // 手写递归
来源：http://lw.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nt.jianghongdianzi.cn

C#:   // 手写递归
来源：http://gt.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ym.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ui.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cd.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ps.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qz.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kd.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jg.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fy.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gm.bjjhwx.cn

================================================================================
来源：http://xm.yuexingan06.cn

O. 并发与异步
来源：http://pi.haigaiapp.cn

================================================================================
来源：http://ai.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ja.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://at.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yh.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hn.hahajie.cn

TS:   // 同 JS
来源：http://ll.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://pu.yuntaijiaju.cn

Go:   go f()
来源：http://dy.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://ky.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ma.huixiangedu.cn

[O02] 使用线程池
来源：http://ui.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ah.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pr.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://gy.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://qc.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sl.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bx.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yu.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dk.hahajie.cn

[O03] 加锁保护共享数据
来源：http://iz.szsharing.cn

Py:   with lock: shared += 1
来源：http://ja.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://sp.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dg.jctech888.com.cn

TS:   // 同 JS
来源：http://pi.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://iu.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zy.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qt.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://yh.9csxet.cn

[O04] 定义异步函数并等待
来源：http://vm.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ff.lnxyls.cn


<!-- 参考信息 -->