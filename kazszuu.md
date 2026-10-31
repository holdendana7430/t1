代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hh.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wk.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yf.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jj.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://xn.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cl.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://on.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://up.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iz.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gt.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://je.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gd.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pk.bookmarksfly.cn

[K07] 进制转换
来源：http://mw.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hw.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ia.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://px.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tw.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zf.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pc.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qp.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zu.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://hf.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://ny.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uv.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://vj.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://nu.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lx.muxihuayi.cn

Go:   encoding/gob
来源：http://xj.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://iw.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pt.panjiajie.cn

================================================================================
来源：http://ve.muxihuayi.cn

L. 网络请求
来源：http://yh.huanxung.cn

================================================================================
来源：http://ux.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://bp.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uf.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kv.asd995.cn

JS:   await fetch(url)
来源：http://bc.muxihuayi.cn

TS:   await fetch(url)
来源：http://hh.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yp.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://gg.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lk.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gc.hnjuh.cn

[L02] 发送 POST JSON
来源：http://ay.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jm.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oo.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oh.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mw.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pk.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ia.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zi.hahajie.cn

[L03] 设置自定义请求头
来源：http://ef.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nk.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hm.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kn.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qs.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bo.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ky.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ey.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hw.colortex.cn

[L04] 设置超时
来源：http://gn.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://vp.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jd.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yg.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bm.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xv.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rq.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yl.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mc.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://dq.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fo.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ko.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kx.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xg.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mx.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yn.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oi.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ch.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://nc.jianghongdianzi.cn

Py:   resp.json()
来源：http://vh.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ic.yuexingan06.cn

JS:   await resp.json()
来源：http://cg.bjjhwx.cn

TS:   await resp.json()
来源：http://nf.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hu.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rw.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://df.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mz.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://de.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xa.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wm.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://wv.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://uh.shtwfgs.cn

Java: resp.statusCode()
来源：http://gu.nszjky.cn

Go:   resp.StatusCode
来源：http://so.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://fg.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://bz.9csxet.cn

[L08] 并发请求多个地址
来源：http://fs.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sf.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://om.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cs.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ik.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tm.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://co.szsharing.cn

================================================================================
来源：http://kk.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://wx.jianghongdianzi.cn

================================================================================
来源：http://pb.chemitech.net.cn

[M01] 读取命令行参数
来源：http://nv.szsharing.cn

Py:   sys.argv[1:]
来源：http://un.nszjky.cn

PHP:  $argv;  $argc;
来源：http://lg.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://do.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://tu.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://gn.panjiajie.cn

Go:   os.Args[1:]
来源：http://nx.wgjwhj.cn

Ruby: ARGV
来源：http://wj.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://dg.wgjwhj.cn

[M02] 读取环境变量
来源：http://sc.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://rj.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://no.nicolike.cn

JS:   process.env.HOME
来源：http://yx.bookmarksfly.cn

TS:   process.env.HOME
来源：http://va.gzmigu.cn

Java: System.getenv("HOME")
来源：http://uv.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mv.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://wq.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hr.huanxung.cn

[M03] 执行外部命令
来源：http://ro.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hw.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://va.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zp.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yl.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ee.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tg.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vj.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://hb.521024.cn

[M04] 获取当前工作目录
来源：http://pp.haigaiapp.cn

Py:   os.getcwd()
来源：http://zw.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ou.chemitech.net.cn

JS:   process.cwd()
来源：http://jm.gzmigu.cn

TS:   process.cwd()
来源：http://rl.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://oz.muxihuayi.cn

Go:   os.Getwd()
来源：http://ld.gzmigu.cn

Ruby: Dir.pwd
来源：http://ld.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ku.nszjky.cn

[M05] 设置退出码
来源：http://rb.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ne.huanxung.cn

PHP:  exit(1);
来源：http://iy.bjjhwx.cn

JS:   process.exit(1)
来源：http://rj.shtwfgs.cn

TS:   process.exit(1)
来源：http://ys.yuexingan06.cn

Java: System.exit(1)
来源：http://hc.hahajie.cn

Go:   os.Exit(1)
来源：http://rm.shxzukj.cn

Ruby: exit 1
来源：http://aw.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ky.huixiangedu.cn

[M06] 向标准错误输出
来源：http://he.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://nj.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wr.wgjwhj.cn

JS:   console.error("err")
来源：http://wl.huanxung.cn

TS:   console.error("err")
来源：http://da.9csxet.cn

Java: System.err.println("err")
来源：http://xx.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jz.chemitech.net.cn

Ruby: warn "err"
来源：http://fl.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ce.hahajie.cn

[M07] 判断是否为主入口
来源：http://rr.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://fa.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bf.nszjky.cn

JS:   require.main === module
来源：http://bw.newstarts.cn

TS:   require.main === module
来源：http://ng.szsharing.cn

Java: public static void main(String[] args)
来源：http://au.gzmigu.cn

Go:   func main()
来源：http://mi.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wl.521024.cn

C#:   static void Main(string[] args)
来源：http://uj.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://py.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://sg.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gy.panjiajie.cn

JS:   process.platform;  process.version
来源：http://kn.9csxet.cn

TS:   process.platform;  process.version
来源：http://pl.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mh.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hk.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://as.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wq.shxzukj.cn

================================================================================
来源：http://fm.muxihuayi.cn

N. 数据结构与算法
来源：http://gt.colortex.cn

================================================================================
来源：http://jn.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://sw.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ie.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dm.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://re.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tr.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fs.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://xk.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uu.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ft.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://lz.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://en.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yf.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pc.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wy.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cu.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://wu.huanxung.cn

Ruby: arr.sort
来源：http://yv.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tx.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ps.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xo.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://pv.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://is.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ao.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mb.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ag.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xl.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ep.hahajie.cn

[N04] 斐波那契数列
来源：http://iy.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ru.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oe.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://re.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ri.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yh.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kk.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bz.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wd.huixiangedu.cn

[N05] 最大公约数
来源：http://zn.huanxung.cn

Py:   math.gcd(a, b)
来源：http://oy.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ac.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ei.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wi.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sk.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oy.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://sh.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kv.asd995.cn

[N06] 判断回文字符串
来源：http://dg.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ke.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://md.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://cs.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://uq.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kk.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://ct.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://ng.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bo.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://ei.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ha.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sw.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qn.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://ma.asd995.cn

Java: // 手写 HashMap
来源：http://ok.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://pc.szsharing.cn

Ruby: // 手写 Hash
来源：http://bq.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hn.yuexingan06.cn

[N08] 生成全排列
来源：http://zu.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://mw.newstarts.cn

PHP:  // 手写递归交换
来源：http://hj.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://dh.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://ep.chemitech.net.cn

Java: // 手写回溯递归
来源：http://wg.shxzukj.cn

Go:   // 手写回溯递归
来源：http://wv.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://de.panjiajie.cn

C#:   // 手写回溯递归
来源：http://bo.huixinmuqiang.cn

[N09] 栈与队列
来源：http://kb.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tj.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mi.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ye.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bs.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wr.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gd.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://af.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mq.szxytkj.cn

[N10] 链表节点定义
来源：http://ed.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fe.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vj.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qz.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kf.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://ms.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lp.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oq.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cl.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://yg.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ls.lnxyls.cn

PHP:  // 手写递归函数
来源：http://bn.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jb.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pl.szsharing.cn

Java: // 手写递归
来源：http://qk.haigaiapp.cn

Go:   // 手写递归
来源：http://qk.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vm.colortex.cn

C#:   // 手写递归
来源：http://rn.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://um.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sy.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dl.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ly.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dl.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zn.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bq.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wd.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.bookmarksfly.cn

================================================================================
来源：http://uw.panjiajie.cn

O. 并发与异步
来源：http://ny.szxytkj.cn

================================================================================
来源：http://hz.shxzskj.cn

[O01] 启动一个线程
来源：http://aw.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jm.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ri.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wt.huixinmuqiang.cn

TS:   // 同 JS
来源：http://xh.521024.cn


<!-- 参考信息 -->