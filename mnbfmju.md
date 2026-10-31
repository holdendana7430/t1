代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fg.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ix.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yc.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qj.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://js.szxytkj.cn

[K07] 进制转换
来源：http://xk.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ev.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qv.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yu.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ev.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bi.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vb.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ra.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://si.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://xr.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yx.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://hq.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://fp.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nq.bookmarksfly.cn

Go:   encoding/gob
来源：http://qr.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://zb.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uc.huanxung.cn

================================================================================
来源：http://tk.haigaiapp.cn

L. 网络请求
来源：http://fy.colortex.cn

================================================================================
来源：http://vk.asd995.cn

[L01] 发送 GET 请求
来源：http://at.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hk.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oa.hahajie.cn

JS:   await fetch(url)
来源：http://mg.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://sq.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xu.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://dg.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sz.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tv.hahajie.cn

[L02] 发送 POST JSON
来源：http://fq.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zm.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vh.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wm.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://um.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ph.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vl.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://us.nszjky.cn

[L03] 设置自定义请求头
来源：http://rt.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nx.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bj.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tg.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lx.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zu.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ky.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jd.yuexingan06.cn

[L04] 设置超时
来源：http://pe.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://px.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lm.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sy.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fi.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gn.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ts.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fv.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bl.asd995.cn

[L05] 上传文件（multipart）
来源：http://em.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ik.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://op.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yu.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yj.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zr.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xf.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ap.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://za.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://ea.muxihuayi.cn

Py:   resp.json()
来源：http://hk.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://bu.hahajie.cn

JS:   await resp.json()
来源：http://jg.newstarts.cn

TS:   await resp.json()
来源：http://pi.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ow.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uj.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://kp.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mv.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ga.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wr.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bz.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://io.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://mw.nszjky.cn

Java: resp.statusCode()
来源：http://oh.muxihuayi.cn

Go:   resp.StatusCode
来源：http://rb.gzmigu.cn

Ruby: resp.code.to_i
来源：http://zq.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://bk.nszjky.cn

[L08] 并发请求多个地址
来源：http://ho.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dg.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://jm.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ky.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tj.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jw.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xm.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yf.jctech888.com.cn

================================================================================
来源：http://bg.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://eo.nszjky.cn

================================================================================
来源：http://mo.huanxung.cn

[M01] 读取命令行参数
来源：http://mj.colortex.cn

Py:   sys.argv[1:]
来源：http://ql.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://rd.asd995.cn

JS:   process.argv.slice(2)
来源：http://xu.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://sy.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://zj.szxytkj.cn

Go:   os.Args[1:]
来源：http://wi.chemitech.net.cn

Ruby: ARGV
来源：http://sy.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://mw.hahajie.cn

[M02] 读取环境变量
来源：http://nf.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://wa.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fo.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://ol.wgjwhj.cn

TS:   process.env.HOME
来源：http://xu.hnjuh.cn

Java: System.getenv("HOME")
来源：http://tx.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nv.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://cv.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://br.jctech888.com.cn

[M03] 执行外部命令
来源：http://cf.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mp.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bi.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dt.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://md.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cd.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tr.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ct.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://tt.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://cn.chemitech.net.cn

Py:   os.getcwd()
来源：http://sn.shxzukj.cn

PHP:  getcwd();
来源：http://wc.huixiangedu.cn

JS:   process.cwd()
来源：http://ow.hnjuh.cn

TS:   process.cwd()
来源：http://zb.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://qi.9csxet.cn

Go:   os.Getwd()
来源：http://iq.wgjwhj.cn

Ruby: Dir.pwd
来源：http://oh.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rh.gzmigu.cn

[M05] 设置退出码
来源：http://ec.asd995.cn

Py:   sys.exit(1)
来源：http://jf.9csxet.cn

PHP:  exit(1);
来源：http://vk.asd995.cn

JS:   process.exit(1)
来源：http://ap.yuexingan06.cn

TS:   process.exit(1)
来源：http://bo.jctech888.com.cn

Java: System.exit(1)
来源：http://aa.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://rc.huixinmuqiang.cn

Ruby: exit 1
来源：http://qg.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vw.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ri.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://xc.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dz.lnxyls.cn

JS:   console.error("err")
来源：http://zv.shxzskj.cn

TS:   console.error("err")
来源：http://jh.bjjhwx.cn

Java: System.err.println("err")
来源：http://qx.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pe.panjiajie.cn

Ruby: warn "err"
来源：http://ac.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://pb.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://bx.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://yv.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://um.szsharing.cn

JS:   require.main === module
来源：http://gn.jctech888.com.cn

TS:   require.main === module
来源：http://dw.szxytkj.cn

Java: public static void main(String[] args)
来源：http://rf.yuexingan06.cn

Go:   func main()
来源：http://sn.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gb.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://jg.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ir.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://yi.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://jt.hahajie.cn

JS:   process.platform;  process.version
来源：http://yw.521024.cn

TS:   process.platform;  process.version
来源：http://it.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tr.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bj.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wd.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gz.shxzukj.cn

================================================================================
来源：http://ma.521024.cn

N. 数据结构与算法
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://sl.521024.cn

[N01] 二分查找（有序数组）
来源：http://wq.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sa.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ks.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fi.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://px.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://po.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iw.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wh.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ww.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://tx.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mi.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ql.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uw.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ft.huanxung.cn

Go:   slices.Sort(arr)
来源：http://xc.521024.cn

Ruby: arr.sort
来源：http://sf.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ja.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://pj.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oe.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://ea.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://va.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://si.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aj.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ld.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vi.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ao.wgjwhj.cn

[N04] 斐波那契数列
来源：http://yl.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ld.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://on.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xl.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gm.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rx.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zz.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uw.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tc.colortex.cn

[N05] 最大公约数
来源：http://se.hahajie.cn

Py:   math.gcd(a, b)
来源：http://gk.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mp.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ix.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vi.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vo.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://as.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://ht.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qp.9csxet.cn

[N06] 判断回文字符串
来源：http://le.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://rh.asd995.cn

PHP:  $s === strrev($s);
来源：http://jm.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://cq.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://qs.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kc.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://ix.asd995.cn

Ruby: s == s.reverse
来源：http://gl.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mb.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://ao.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yt.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fj.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ts.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://wv.nicolike.cn

Java: // 手写 HashMap
来源：http://ms.521024.cn

Go:   // 手写 map[int]int
来源：http://bw.nicolike.cn

Ruby: // 手写 Hash
来源：http://jq.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bs.bookmarksfly.cn

[N08] 生成全排列
来源：http://zu.521024.cn

Py:   itertools.permutations(arr)
来源：http://au.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://we.nicolike.cn

JS:   // 手写回溯递归
来源：http://ss.panjiajie.cn

TS:   // 手写回溯递归
来源：http://ao.chemitech.net.cn

Java: // 手写回溯递归
来源：http://hc.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://rp.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ov.huanxung.cn

C#:   // 手写回溯递归
来源：http://jo.hnjuh.cn

[N09] 栈与队列
来源：http://pt.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ti.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qe.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ae.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bf.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qh.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wq.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zt.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zt.shtwfgs.cn

[N10] 链表节点定义
来源：http://bi.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fn.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nx.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gb.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ih.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://ht.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://du.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sd.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tf.colortex.cn

[N11] 二叉树中序遍历
来源：http://qf.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hc.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://po.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rx.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wj.yuntaijiaju.cn

Java: // 手写递归
来源：http://cb.shxzukj.cn

Go:   // 手写递归
来源：http://bb.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ll.shxzskj.cn

C#:   // 手写递归
来源：http://hp.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ai.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wi.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oj.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ij.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eh.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ke.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pz.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ky.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://co.jianghongdianzi.cn

================================================================================
来源：http://fe.jianghongdianzi.cn

O. 并发与异步
来源：http://qk.muxihuayi.cn

================================================================================
来源：http://ld.szsharing.cn

[O01] 启动一个线程
来源：http://eq.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ls.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://re.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mb.wgjwhj.cn

TS:   // 同 JS
来源：http://ry.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://uu.haigaiapp.cn

Go:   go f()
来源：http://xo.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://dn.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://kj.chemitech.net.cn

[O02] 使用线程池
来源：http://qo.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ao.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://px.asd995.cn

JS:   // worker_threads 线程池
来源：http://mg.panjiajie.cn


<!-- 参考信息 -->