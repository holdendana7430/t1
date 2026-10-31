代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dq.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ts.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sj.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zw.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xf.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://df.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fo.hnjuh.cn

[K05] 深拷贝对象
来源：http://rz.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://lo.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://yp.szsharing.cn

JS:   structuredClone(obj)
来源：http://am.shxzukj.cn

TS:   structuredClone(obj)
来源：http://bi.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pp.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ac.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gi.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zs.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://cl.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xn.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vf.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mx.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ik.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jm.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gg.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://io.jctech888.com.cn

[K07] 进制转换
来源：http://fv.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bn.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://de.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iq.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dj.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oj.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rf.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ik.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qm.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://au.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ry.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ep.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://fq.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://bu.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ba.nszjky.cn

Go:   encoding/gob
来源：http://kb.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://vy.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xq.chemitech.net.cn

================================================================================
来源：http://kl.panjiajie.cn

L. 网络请求
来源：http://gw.hnjuh.cn

================================================================================
来源：http://hb.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://cw.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pv.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sm.colortex.cn

JS:   await fetch(url)
来源：http://lm.hnjuh.cn

TS:   await fetch(url)
来源：http://jb.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rt.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://kl.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ij.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tq.colortex.cn

[L02] 发送 POST JSON
来源：http://jp.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cu.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gi.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ro.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bk.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nn.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qx.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yc.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://md.lnxyls.cn

[L03] 设置自定义请求头
来源：http://sz.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ev.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cq.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dk.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ul.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wy.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gi.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xd.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://di.shtwfgs.cn

[L04] 设置超时
来源：http://vz.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://un.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ny.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cb.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xf.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bq.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uc.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ed.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vp.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ip.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://my.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nq.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nq.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gk.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aa.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ob.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pq.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ua.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://bg.yuntaijiaju.cn

Py:   resp.json()
来源：http://te.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://ro.wgjwhj.cn

JS:   await resp.json()
来源：http://to.gzmigu.cn

TS:   await resp.json()
来源：http://fz.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ml.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mn.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://fx.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jb.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://vf.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fo.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gv.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://dc.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://oo.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://fw.szxytkj.cn

Go:   resp.StatusCode
来源：http://db.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ko.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://wn.gzmigu.cn

[L08] 并发请求多个地址
来源：http://in.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://da.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://cc.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gx.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ho.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://io.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hd.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xo.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lt.huixiangedu.cn

================================================================================
来源：http://iq.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://al.chemitech.net.cn

================================================================================
来源：http://uw.colortex.cn

[M01] 读取命令行参数
来源：http://my.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://al.colortex.cn

PHP:  $argv;  $argc;
来源：http://wc.9csxet.cn

JS:   process.argv.slice(2)
来源：http://bt.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://lq.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://df.gzmigu.cn

Go:   os.Args[1:]
来源：http://xw.shxzskj.cn

Ruby: ARGV
来源：http://xc.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://gf.muxihuayi.cn

[M02] 读取环境变量
来源：http://ig.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://op.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jk.lnxyls.cn

JS:   process.env.HOME
来源：http://qw.gzmigu.cn

TS:   process.env.HOME
来源：http://xn.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://vs.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fp.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://tc.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yh.lnxyls.cn

[M03] 执行外部命令
来源：http://us.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ru.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jp.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://me.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ca.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://md.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rq.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hc.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://wb.hahajie.cn

[M04] 获取当前工作目录
来源：http://yd.nszjky.cn

Py:   os.getcwd()
来源：http://ro.szxytkj.cn

PHP:  getcwd();
来源：http://ly.colortex.cn

JS:   process.cwd()
来源：http://fz.9csxet.cn

TS:   process.cwd()
来源：http://wm.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://vx.shtwfgs.cn

Go:   os.Getwd()
来源：http://pq.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://jg.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://px.szxytkj.cn

[M05] 设置退出码
来源：http://qf.nicolike.cn

Py:   sys.exit(1)
来源：http://ez.bjjhwx.cn

PHP:  exit(1);
来源：http://du.nszjky.cn

JS:   process.exit(1)
来源：http://kv.huixiangedu.cn

TS:   process.exit(1)
来源：http://ih.hnjuh.cn

Java: System.exit(1)
来源：http://tx.panjiajie.cn

Go:   os.Exit(1)
来源：http://fl.panjiajie.cn

Ruby: exit 1
来源：http://ik.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hj.lnxyls.cn

[M06] 向标准错误输出
来源：http://ip.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://co.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ci.521024.cn

JS:   console.error("err")
来源：http://nt.bjjhwx.cn

TS:   console.error("err")
来源：http://lq.szxytkj.cn

Java: System.err.println("err")
来源：http://nh.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ki.newstarts.cn

Ruby: warn "err"
来源：http://nz.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://fx.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://ip.asd995.cn

Py:   if __name__ == "__main__":
来源：http://hw.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zm.nszjky.cn

JS:   require.main === module
来源：http://jt.lnxyls.cn

TS:   require.main === module
来源：http://jj.huanxung.cn

Java: public static void main(String[] args)
来源：http://bc.bjjhwx.cn

Go:   func main()
来源：http://tj.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qo.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://at.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://eb.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://cb.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ya.nicolike.cn

JS:   process.platform;  process.version
来源：http://ms.newstarts.cn

TS:   process.platform;  process.version
来源：http://vi.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uw.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bp.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fp.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iw.yuntaijiaju.cn

================================================================================
来源：http://tz.panjiajie.cn

N. 数据结构与算法
来源：http://ul.chemitech.net.cn

================================================================================
来源：http://tn.521024.cn

[N01] 二分查找（有序数组）
来源：http://zc.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oa.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gn.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dz.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://se.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tm.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://pv.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zh.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lp.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://re.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://cw.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://do.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bi.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dk.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jd.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ld.haigaiapp.cn

Ruby: arr.sort
来源：http://qj.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ok.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://ye.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://za.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://ru.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://za.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zc.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cv.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yx.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://go.huanxung.cn

[N04] 斐波那契数列
来源：http://oz.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mj.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dr.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://et.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dm.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vl.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ol.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qs.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cb.panjiajie.cn

[N05] 最大公约数
来源：http://yf.nszjky.cn

Py:   math.gcd(a, b)
来源：http://gb.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uu.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ey.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pd.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ja.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fz.shxzukj.cn

Ruby: a.gcd(b)
来源：http://tg.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ln.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://op.shxzukj.cn

Py:   s == s[::-1]
来源：http://qq.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ul.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://zk.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://ni.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zq.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://rq.jctech888.com.cn

Ruby: s == s.reverse
来源：http://zl.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ix.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ri.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vq.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zj.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ix.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://qc.wgjwhj.cn

Java: // 手写 HashMap
来源：http://jy.nicolike.cn

Go:   // 手写 map[int]int
来源：http://fi.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://ss.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://km.chemitech.net.cn

[N08] 生成全排列
来源：http://wn.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ey.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://on.nicolike.cn

JS:   // 手写回溯递归
来源：http://zl.newstarts.cn

TS:   // 手写回溯递归
来源：http://xc.hahajie.cn

Java: // 手写回溯递归
来源：http://kk.huanxung.cn

Go:   // 手写回溯递归
来源：http://hd.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://fu.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://jr.huixiangedu.cn

[N09] 栈与队列
来源：http://tx.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jv.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://un.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ut.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ha.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ov.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qr.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yo.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pq.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://rh.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ik.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dn.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sp.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://li.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://iu.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tn.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uw.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mj.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://he.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wu.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://hn.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gs.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://au.bjjhwx.cn

Java: // 手写递归
来源：http://bs.9csxet.cn

Go:   // 手写递归
来源：http://gi.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kc.hnjuh.cn

C#:   // 手写递归
来源：http://ai.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fn.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://un.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wt.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vo.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zr.jctech888.com.cn


<!-- 参考信息 -->