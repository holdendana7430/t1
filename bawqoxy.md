代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://kn.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yy.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xk.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nq.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://dm.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mx.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ti.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ii.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lg.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mk.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zf.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ry.huixinmuqiang.cn

[K07] 进制转换
来源：http://vh.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://by.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mi.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qh.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ia.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://am.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sv.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://db.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kp.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://nx.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://wf.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lb.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://hp.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://qv.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oz.hahajie.cn

Go:   encoding/gob
来源：http://uc.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://av.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://nx.szxytkj.cn

L. 网络请求
来源：http://ww.huixiangedu.cn

================================================================================
来源：http://xp.panjiajie.cn

[L01] 发送 GET 请求
来源：http://lb.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bw.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bd.lnxyls.cn

JS:   await fetch(url)
来源：http://hr.haigaiapp.cn

TS:   await fetch(url)
来源：http://ha.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ed.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://sz.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tv.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jy.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ff.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bu.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vz.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vi.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mx.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://az.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gj.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jl.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uk.gzmigu.cn

[L03] 设置自定义请求头
来源：http://rs.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hj.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xs.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fs.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jy.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://do.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sh.shxzskj.cn

[L04] 设置超时
来源：http://cq.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://xo.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yu.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://si.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cn.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kk.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uh.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iw.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pn.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://py.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://is.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lu.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nd.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ij.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jg.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fm.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qs.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jh.hahajie.cn

[L06] 解析响应为 JSON
来源：http://wj.9csxet.cn

Py:   resp.json()
来源：http://wc.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://de.jctech888.com.cn

JS:   await resp.json()
来源：http://sb.szxytkj.cn

TS:   await resp.json()
来源：http://wf.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pk.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mo.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://sl.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ry.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://td.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ab.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tl.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://tn.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://jt.wgjwhj.cn

Java: resp.statusCode()
来源：http://cz.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://ux.521024.cn

Ruby: resp.code.to_i
来源：http://fk.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://eb.huanxung.cn

[L08] 并发请求多个地址
来源：http://uv.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rm.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://xj.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ap.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ha.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ic.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uc.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sy.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rt.huanxung.cn

================================================================================
来源：http://uy.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://zx.shxzskj.cn

================================================================================
来源：http://fx.huanxung.cn

[M01] 读取命令行参数
来源：http://zi.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ty.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://oi.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://pd.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://qz.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://qu.panjiajie.cn

Go:   os.Args[1:]
来源：http://go.shxzskj.cn

Ruby: ARGV
来源：http://uu.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://kf.lnxyls.cn

[M02] 读取环境变量
来源：http://uv.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://fc.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ri.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ek.colortex.cn

TS:   process.env.HOME
来源：http://yd.hahajie.cn

Java: System.getenv("HOME")
来源：http://nn.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cm.9csxet.cn

Ruby: ENV["HOME"]
来源：http://nc.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fw.9csxet.cn

[M03] 执行外部命令
来源：http://ki.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yz.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ii.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kh.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://em.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ad.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tk.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qi.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://ds.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://kg.bookmarksfly.cn

Py:   os.getcwd()
来源：http://gp.gzmigu.cn

PHP:  getcwd();
来源：http://pk.chemitech.net.cn

JS:   process.cwd()
来源：http://zr.bjjhwx.cn

TS:   process.cwd()
来源：http://ob.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://wc.huanxung.cn

Go:   os.Getwd()
来源：http://oq.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://sq.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://db.521024.cn

[M05] 设置退出码
来源：http://af.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://gy.chemitech.net.cn

PHP:  exit(1);
来源：http://gu.newstarts.cn

JS:   process.exit(1)
来源：http://vj.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ie.gzmigu.cn

Java: System.exit(1)
来源：http://lv.huixiangedu.cn

Go:   os.Exit(1)
来源：http://qa.bookmarksfly.cn

Ruby: exit 1
来源：http://na.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hg.521024.cn

[M06] 向标准错误输出
来源：http://ez.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://jc.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lf.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ll.9csxet.cn

TS:   console.error("err")
来源：http://lx.shxzskj.cn

Java: System.err.println("err")
来源：http://hu.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fw.nicolike.cn

Ruby: warn "err"
来源：http://cc.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://sm.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://mv.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://tk.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lz.newstarts.cn

JS:   require.main === module
来源：http://ca.shxzskj.cn

TS:   require.main === module
来源：http://bh.asd995.cn

Java: public static void main(String[] args)
来源：http://dh.shtwfgs.cn

Go:   func main()
来源：http://po.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ds.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://cz.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://ou.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://ae.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://cb.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://qu.hahajie.cn

TS:   process.platform;  process.version
来源：http://sk.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bn.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fq.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xe.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rx.jianghongdianzi.cn

================================================================================
来源：http://is.gzmigu.cn

N. 数据结构与算法
来源：http://ya.asd995.cn

================================================================================
来源：http://lc.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://tm.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ur.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mh.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ya.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vs.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://tn.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ci.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://md.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ld.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://sh.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yt.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fo.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sl.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ul.521024.cn

Go:   slices.Sort(arr)
来源：http://xh.gzmigu.cn

Ruby: arr.sort
来源：http://hx.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jn.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://mr.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fi.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://oy.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yi.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ps.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mq.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ky.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wq.wgjwhj.cn

[N04] 斐波那契数列
来源：http://ri.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://im.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xm.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hu.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ye.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uo.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://um.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ln.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ei.huixiangedu.cn

[N05] 最大公约数
来源：http://xr.521024.cn

Py:   math.gcd(a, b)
来源：http://na.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://id.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ke.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yd.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nk.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qy.panjiajie.cn

Ruby: a.gcd(b)
来源：http://si.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ud.colortex.cn

[N06] 判断回文字符串
来源：http://hs.colortex.cn

Py:   s == s[::-1]
来源：http://mu.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://dd.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://rw.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://gw.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ak.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://hw.szsharing.cn

Ruby: s == s.reverse
来源：http://et.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://um.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://pb.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cb.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qy.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oa.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://fa.colortex.cn

Java: // 手写 HashMap
来源：http://yb.nszjky.cn

Go:   // 手写 map[int]int
来源：http://tg.hahajie.cn

Ruby: // 手写 Hash
来源：http://eo.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ra.shxzukj.cn

[N08] 生成全排列
来源：http://ca.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://vr.szsharing.cn

PHP:  // 手写递归交换
来源：http://zs.shxzukj.cn

JS:   // 手写回溯递归
来源：http://qx.nicolike.cn

TS:   // 手写回溯递归
来源：http://fs.asd995.cn

Java: // 手写回溯递归
来源：http://zy.huanxung.cn

Go:   // 手写回溯递归
来源：http://fi.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ko.hnjuh.cn

C#:   // 手写回溯递归
来源：http://tq.yuexingan06.cn

[N09] 栈与队列
来源：http://bm.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bu.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ms.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eh.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yv.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uo.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yr.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sf.wgjwhj.cn

[N10] 链表节点定义
来源：http://zi.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vl.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kr.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qk.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iz.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ik.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://po.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xc.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lx.huanxung.cn

[N11] 二叉树中序遍历
来源：http://lr.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cu.szsharing.cn

PHP:  // 手写递归函数
来源：http://da.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tw.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ew.shxzskj.cn

Java: // 手写递归
来源：http://nc.gzmigu.cn

Go:   // 手写递归
来源：http://no.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://il.wgjwhj.cn

C#:   // 手写递归
来源：http://qo.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ab.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wb.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://by.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ck.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pi.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dq.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sm.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vy.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://si.gzmigu.cn

================================================================================
来源：http://nb.chemitech.net.cn

O. 并发与异步
来源：http://ly.panjiajie.cn

================================================================================
来源：http://aj.szxytkj.cn

[O01] 启动一个线程
来源：http://tq.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mz.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vv.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vp.yuntaijiaju.cn

TS:   // 同 JS
来源：http://mo.hnjuh.cn


<!-- 参考信息 -->