代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kj.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kd.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nx.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://az.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sc.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://al.lnxyls.cn

[K05] 深拷贝对象
来源：http://ko.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://qi.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://po.shxzskj.cn

JS:   structuredClone(obj)
来源：http://qa.nszjky.cn

TS:   structuredClone(obj)
来源：http://vk.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uq.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zx.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://li.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ll.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://te.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fp.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xi.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xp.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yw.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fu.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zs.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iu.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lb.bjjhwx.cn

[K07] 进制转换
来源：http://xh.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qt.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cb.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://og.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mg.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ae.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lb.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vm.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bw.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://dt.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://bt.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hh.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://nv.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://wg.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vk.szsharing.cn

Go:   encoding/gob
来源：http://pp.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://dz.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://im.shtwfgs.cn

================================================================================
来源：http://xf.yuexingan06.cn

L. 网络请求
来源：http://dy.huixinmuqiang.cn

================================================================================
来源：http://pd.panjiajie.cn

[L01] 发送 GET 请求
来源：http://gc.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cd.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xu.szxytkj.cn

JS:   await fetch(url)
来源：http://il.jctech888.com.cn

TS:   await fetch(url)
来源：http://ou.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ee.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://yj.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gx.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ki.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://st.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gn.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jm.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fz.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lk.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mg.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jt.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xj.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://im.asd995.cn

[L03] 设置自定义请求头
来源：http://im.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dx.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tn.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rc.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vh.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tt.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ee.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kw.bjjhwx.cn

[L04] 设置超时
来源：http://pu.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://jc.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nj.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://be.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tm.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ro.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mi.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xj.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://se.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ek.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mh.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jm.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pm.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xz.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tr.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gl.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zn.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mz.colortex.cn

[L06] 解析响应为 JSON
来源：http://jc.newstarts.cn

Py:   resp.json()
来源：http://nu.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://do.hahajie.cn

JS:   await resp.json()
来源：http://hs.szxytkj.cn

TS:   await resp.json()
来源：http://yr.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://na.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sq.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://gh.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jz.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://mo.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oe.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ju.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://la.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://ys.wgjwhj.cn

Java: resp.statusCode()
来源：http://pu.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ji.colortex.cn

Ruby: resp.code.to_i
来源：http://ut.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://vv.shxzukj.cn

[L08] 并发请求多个地址
来源：http://uh.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mm.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://cv.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ew.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jt.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lz.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oy.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bm.chemitech.net.cn

================================================================================
来源：http://ui.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://pi.szxytkj.cn

================================================================================
来源：http://fw.hnjuh.cn

[M01] 读取命令行参数
来源：http://ex.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://uw.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ls.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://fq.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://jg.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://ss.panjiajie.cn

Go:   os.Args[1:]
来源：http://em.gzmigu.cn

Ruby: ARGV
来源：http://nl.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ye.panjiajie.cn

[M02] 读取环境变量
来源：http://zy.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://xz.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nc.gzmigu.cn

JS:   process.env.HOME
来源：http://pk.yuexingan06.cn

TS:   process.env.HOME
来源：http://pa.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://fd.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lz.newstarts.cn

Ruby: ENV["HOME"]
来源：http://uk.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hm.colortex.cn

[M03] 执行外部命令
来源：http://tm.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bz.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ex.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wf.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eb.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yl.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nl.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qe.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://xf.huanxung.cn

[M04] 获取当前工作目录
来源：http://mq.shtwfgs.cn

Py:   os.getcwd()
来源：http://ie.shxzskj.cn

PHP:  getcwd();
来源：http://wy.huixiangedu.cn

JS:   process.cwd()
来源：http://ng.jctech888.com.cn

TS:   process.cwd()
来源：http://oo.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://dm.haigaiapp.cn

Go:   os.Getwd()
来源：http://iy.huixiangedu.cn

Ruby: Dir.pwd
来源：http://ty.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xx.newstarts.cn

[M05] 设置退出码
来源：http://sd.huanxung.cn

Py:   sys.exit(1)
来源：http://hf.szsharing.cn

PHP:  exit(1);
来源：http://sp.colortex.cn

JS:   process.exit(1)
来源：http://tn.nszjky.cn

TS:   process.exit(1)
来源：http://fy.asd995.cn

Java: System.exit(1)
来源：http://fv.shxzskj.cn

Go:   os.Exit(1)
来源：http://xm.jianghongdianzi.cn

Ruby: exit 1
来源：http://gx.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.gzmigu.cn

[M06] 向标准错误输出
来源：http://fe.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://pc.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fq.haigaiapp.cn

JS:   console.error("err")
来源：http://zr.shtwfgs.cn

TS:   console.error("err")
来源：http://hx.shtwfgs.cn

Java: System.err.println("err")
来源：http://bv.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iu.yuexingan06.cn

Ruby: warn "err"
来源：http://ts.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://br.gzmigu.cn

[M07] 判断是否为主入口
来源：http://qi.asd995.cn

Py:   if __name__ == "__main__":
来源：http://aw.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mg.huixinmuqiang.cn

JS:   require.main === module
来源：http://vs.panjiajie.cn

TS:   require.main === module
来源：http://sw.nicolike.cn

Java: public static void main(String[] args)
来源：http://sv.shtwfgs.cn

Go:   func main()
来源：http://xr.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nd.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://qk.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://yu.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://br.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://zx.lnxyls.cn

JS:   process.platform;  process.version
来源：http://mc.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://mh.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://py.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gl.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ec.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zc.huixiangedu.cn

================================================================================
来源：http://bb.9csxet.cn

N. 数据结构与算法
来源：http://jm.nicolike.cn

================================================================================
来源：http://ks.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://ks.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wq.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qb.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pk.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rn.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rt.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://vw.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uw.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://au.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://en.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://je.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fi.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kn.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fw.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rb.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://lw.colortex.cn

Ruby: arr.sort
来源：http://zt.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fd.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://qf.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jk.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://fj.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://un.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qr.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://le.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hw.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mt.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ol.shxzukj.cn

[N04] 斐波那契数列
来源：http://bw.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rr.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zb.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zx.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zv.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://af.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://he.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ro.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ct.huixiangedu.cn

[N05] 最大公约数
来源：http://ua.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ed.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://df.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fe.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oh.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zg.panjiajie.cn

Ruby: a.gcd(b)
来源：http://kp.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fj.hnjuh.cn

[N06] 判断回文字符串
来源：http://vr.shxzukj.cn

Py:   s == s[::-1]
来源：http://cu.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://xk.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://xq.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://cv.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://za.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ph.muxihuayi.cn

Ruby: s == s.reverse
来源：http://vr.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qm.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://cz.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jf.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uw.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://re.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://jl.shxzukj.cn

Java: // 手写 HashMap
来源：http://mv.nszjky.cn

Go:   // 手写 map[int]int
来源：http://jj.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://tp.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fi.lnxyls.cn

[N08] 生成全排列
来源：http://mu.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://fw.newstarts.cn

PHP:  // 手写递归交换
来源：http://sa.panjiajie.cn

JS:   // 手写回溯递归
来源：http://sv.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://vt.hnjuh.cn

Java: // 手写回溯递归
来源：http://gn.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ri.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://kr.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://qd.shtwfgs.cn

[N09] 栈与队列
来源：http://aj.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pw.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zv.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rf.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gb.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ab.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xl.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ro.bookmarksfly.cn

[N10] 链表节点定义
来源：http://yr.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gr.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uc.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ul.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zw.asd995.cn

Java: class Node { int v; Node next; }
来源：http://tz.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gh.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://un.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zq.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ns.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jq.szsharing.cn

PHP:  // 手写递归函数
来源：http://nm.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pk.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bx.panjiajie.cn

Java: // 手写递归
来源：http://nr.newstarts.cn

Go:   // 手写递归
来源：http://gi.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ww.yuntaijiaju.cn

C#:   // 手写递归
来源：http://tv.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cm.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jn.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mz.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://du.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.szsharing.cn


<!-- 参考信息 -->