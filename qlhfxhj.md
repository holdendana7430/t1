代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hp.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://pi.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://fn.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rc.haigaiapp.cn

Go:   encoding/gob
来源：http://tr.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://wi.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zy.shxzukj.cn

================================================================================
来源：http://bs.hnjuh.cn

L. 网络请求
来源：http://hk.lnxyls.cn

================================================================================
来源：http://mp.huanxung.cn

[L01] 发送 GET 请求
来源：http://jz.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vg.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vi.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://li.wgjwhj.cn

TS:   await fetch(url)
来源：http://sz.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dl.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://ha.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gq.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oj.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://kb.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ng.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yr.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tc.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xg.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bn.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ww.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aj.9csxet.cn

[L03] 设置自定义请求头
来源：http://wl.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://df.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://it.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nv.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pi.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vx.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ff.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mb.jctech888.com.cn

[L04] 设置超时
来源：http://gs.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://vc.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xl.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ur.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pb.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eb.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ob.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zw.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zw.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ym.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ub.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fh.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dj.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mz.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iv.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qi.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://he.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vs.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://sy.bjjhwx.cn

Py:   resp.json()
来源：http://it.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://yq.muxihuayi.cn

JS:   await resp.json()
来源：http://yk.jctech888.com.cn

TS:   await resp.json()
来源：http://gk.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zp.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kh.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ww.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ne.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://wt.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wj.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rm.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://wd.asd995.cn

TS:   resp.ok;  resp.status
来源：http://br.shxzskj.cn

Java: resp.statusCode()
来源：http://yu.panjiajie.cn

Go:   resp.StatusCode
来源：http://vi.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://eg.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://er.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://te.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kb.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://ed.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wz.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rc.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ql.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dv.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://em.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yq.hahajie.cn

================================================================================
来源：http://zi.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://hs.hnjuh.cn

================================================================================
来源：http://ip.gzmigu.cn

[M01] 读取命令行参数
来源：http://vl.9csxet.cn

Py:   sys.argv[1:]
来源：http://pu.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://jr.hahajie.cn

JS:   process.argv.slice(2)
来源：http://qj.huanxung.cn

TS:   process.argv.slice(2)
来源：http://fa.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://wy.521024.cn

Go:   os.Args[1:]
来源：http://mc.panjiajie.cn

Ruby: ARGV
来源：http://ye.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://nf.chemitech.net.cn

[M02] 读取环境变量
来源：http://ey.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ci.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zt.hnjuh.cn

JS:   process.env.HOME
来源：http://vf.nicolike.cn

TS:   process.env.HOME
来源：http://bl.newstarts.cn

Java: System.getenv("HOME")
来源：http://gq.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wc.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://ci.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vl.gzmigu.cn

[M03] 执行外部命令
来源：http://pn.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cq.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gb.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tm.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zo.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pc.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xz.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nr.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://uf.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://tj.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://fo.huixiangedu.cn

PHP:  getcwd();
来源：http://wi.jianghongdianzi.cn

JS:   process.cwd()
来源：http://vt.newstarts.cn

TS:   process.cwd()
来源：http://tr.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ui.9csxet.cn

Go:   os.Getwd()
来源：http://sy.shxzukj.cn

Ruby: Dir.pwd
来源：http://kz.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://za.bookmarksfly.cn

[M05] 设置退出码
来源：http://vt.yuexingan06.cn

Py:   sys.exit(1)
来源：http://as.chemitech.net.cn

PHP:  exit(1);
来源：http://zv.bookmarksfly.cn

JS:   process.exit(1)
来源：http://vs.lnxyls.cn

TS:   process.exit(1)
来源：http://mf.521024.cn

Java: System.exit(1)
来源：http://is.lnxyls.cn

Go:   os.Exit(1)
来源：http://cf.szsharing.cn

Ruby: exit 1
来源：http://mw.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jt.nszjky.cn

[M06] 向标准错误输出
来源：http://sb.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://lr.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vu.huanxung.cn

JS:   console.error("err")
来源：http://uj.hnjuh.cn

TS:   console.error("err")
来源：http://zm.muxihuayi.cn

Java: System.err.println("err")
来源：http://ad.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ev.yuntaijiaju.cn

Ruby: warn "err"
来源：http://ra.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://wa.hnjuh.cn

[M07] 判断是否为主入口
来源：http://ch.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://mn.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tw.muxihuayi.cn

JS:   require.main === module
来源：http://rn.szsharing.cn

TS:   require.main === module
来源：http://wn.newstarts.cn

Java: public static void main(String[] args)
来源：http://vc.shxzskj.cn

Go:   func main()
来源：http://gg.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qe.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://gl.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://sh.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://xl.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://yf.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://is.shxzskj.cn

TS:   process.platform;  process.version
来源：http://xl.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rx.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yr.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uf.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zq.muxihuayi.cn

================================================================================
来源：http://da.szsharing.cn

N. 数据结构与算法
来源：http://ix.shxzskj.cn

================================================================================
来源：http://rx.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://xv.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cw.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fq.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gn.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sb.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tg.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://rj.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hw.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qg.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://my.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qo.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hu.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uy.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xe.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zv.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://mu.muxihuayi.cn

Ruby: arr.sort
来源：http://tg.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pa.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://xn.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fv.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://ck.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://so.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://av.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://im.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nz.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ad.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://es.shxzukj.cn

[N04] 斐波那契数列
来源：http://gx.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tj.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oh.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wb.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nj.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rt.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zu.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://of.huixinmuqiang.cn

[N05] 最大公约数
来源：http://yu.szsharing.cn

Py:   math.gcd(a, b)
来源：http://wb.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://we.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jq.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://io.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tk.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tp.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://hy.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gz.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ir.lnxyls.cn

Py:   s == s[::-1]
来源：http://nd.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://bx.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://df.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://xn.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ch.szsharing.cn

Go:   // 双指针从两端比较
来源：http://sg.huixiangedu.cn

Ruby: s == s.reverse
来源：http://mw.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mt.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://yb.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://li.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://me.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ib.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://at.hahajie.cn

Java: // 手写 HashMap
来源：http://rb.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://uz.nszjky.cn

Ruby: // 手写 Hash
来源：http://cv.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yc.szxytkj.cn

[N08] 生成全排列
来源：http://de.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://no.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://og.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://rx.colortex.cn

TS:   // 手写回溯递归
来源：http://zx.colortex.cn

Java: // 手写回溯递归
来源：http://px.colortex.cn

Go:   // 手写回溯递归
来源：http://ws.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://pm.nszjky.cn

C#:   // 手写回溯递归
来源：http://fw.yuntaijiaju.cn

[N09] 栈与队列
来源：http://ql.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tq.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jt.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vf.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wb.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gp.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kh.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cu.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eh.shtwfgs.cn

[N10] 链表节点定义
来源：http://wx.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bc.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zz.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dj.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dt.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://bw.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ln.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://et.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://af.newstarts.cn

[N11] 二叉树中序遍历
来源：http://ca.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jg.panjiajie.cn

PHP:  // 手写递归函数
来源：http://sq.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fb.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xf.521024.cn

Java: // 手写递归
来源：http://yh.szsharing.cn

Go:   // 手写递归
来源：http://jy.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ko.9csxet.cn

C#:   // 手写递归
来源：http://go.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mm.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fg.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://um.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yc.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ii.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ma.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zk.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uz.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yb.521024.cn

================================================================================
来源：http://uk.521024.cn

O. 并发与异步
来源：http://oo.bookmarksfly.cn

================================================================================
来源：http://bc.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://ri.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bp.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hq.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ww.szsharing.cn

TS:   // 同 JS
来源：http://cc.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://se.lnxyls.cn

Go:   go f()
来源：http://oq.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://bm.newstarts.cn

C#:   Task.Run(() => F());
来源：http://rs.bjjhwx.cn

[O02] 使用线程池
来源：http://ri.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fm.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vj.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://ee.nicolike.cn

TS:   // worker_threads 线程池
来源：http://ji.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fy.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yt.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://so.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lw.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://td.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://qs.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://yi.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gv.yuexingan06.cn

TS:   // 同 JS
来源：http://ac.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://fo.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oz.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wt.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://cz.newstarts.cn

[O04] 定义异步函数并等待
来源：http://lc.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://gh.asd995.cn


<!-- 参考信息 -->