代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://em.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cv.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://vr.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fj.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mi.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sb.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zj.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tv.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://md.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hw.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://am.9csxet.cn

[K05] 深拷贝对象
来源：http://eo.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://mj.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://bw.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://pa.hnjuh.cn

TS:   structuredClone(obj)
来源：http://iy.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ox.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dc.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xr.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iu.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://tu.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qh.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hv.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oz.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mh.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nw.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zl.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ly.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cq.haigaiapp.cn

[K07] 进制转换
来源：http://fl.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mo.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kg.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xy.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fv.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zv.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://si.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iw.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rl.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pb.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://zo.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mz.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://gi.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://di.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sw.nicolike.cn

Go:   encoding/gob
来源：http://xc.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://ra.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://an.bookmarksfly.cn

================================================================================
来源：http://xh.521024.cn

L. 网络请求
来源：http://nq.hnjuh.cn

================================================================================
来源：http://vn.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://di.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sv.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yo.huanxung.cn

JS:   await fetch(url)
来源：http://wc.nicolike.cn

TS:   await fetch(url)
来源：http://rb.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zm.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://al.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://my.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sr.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://mm.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xs.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cd.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eg.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cq.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ox.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sc.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yf.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rm.gzmigu.cn

[L03] 设置自定义请求头
来源：http://sf.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yh.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rd.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iv.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ld.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rv.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lx.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iw.huixiangedu.cn

[L04] 设置超时
来源：http://fm.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://lr.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wv.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://si.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gv.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gy.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pk.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nk.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mg.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://tv.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bo.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lf.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rt.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gg.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://du.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qj.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qb.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jv.nicolike.cn

[L06] 解析响应为 JSON
来源：http://bo.hahajie.cn

Py:   resp.json()
来源：http://mh.colortex.cn

PHP:  json_decode($body, true);
来源：http://dp.colortex.cn

JS:   await resp.json()
来源：http://wx.nicolike.cn

TS:   await resp.json()
来源：http://mf.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oz.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rm.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://rk.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kg.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://jn.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pg.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xj.521024.cn

JS:   resp.ok;  resp.status
来源：http://bt.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://cm.hahajie.cn

Java: resp.statusCode()
来源：http://jv.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://gx.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://pm.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://cx.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://hg.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ji.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://kf.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://er.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ex.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ne.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fh.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://et.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cq.szsharing.cn

================================================================================
来源：http://pa.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://qz.wgjwhj.cn

================================================================================
来源：http://xp.muxihuayi.cn

[M01] 读取命令行参数
来源：http://il.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://tq.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://bh.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://fm.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://jq.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://xj.szxytkj.cn

Go:   os.Args[1:]
来源：http://dm.521024.cn

Ruby: ARGV
来源：http://gg.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://ym.shtwfgs.cn

[M02] 读取环境变量
来源：http://hp.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://ow.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xp.panjiajie.cn

JS:   process.env.HOME
来源：http://us.huixiangedu.cn

TS:   process.env.HOME
来源：http://bc.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://jg.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vv.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://au.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ai.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://fw.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ze.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://st.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wi.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cr.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mu.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qn.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fy.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://qi.9csxet.cn

[M04] 获取当前工作目录
来源：http://mr.colortex.cn

Py:   os.getcwd()
来源：http://pn.colortex.cn

PHP:  getcwd();
来源：http://dx.huixiangedu.cn

JS:   process.cwd()
来源：http://ul.hahajie.cn

TS:   process.cwd()
来源：http://ed.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://zg.gzmigu.cn

Go:   os.Getwd()
来源：http://ur.9csxet.cn

Ruby: Dir.pwd
来源：http://hb.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ra.9csxet.cn

[M05] 设置退出码
来源：http://ga.9csxet.cn

Py:   sys.exit(1)
来源：http://uv.bookmarksfly.cn

PHP:  exit(1);
来源：http://vd.nicolike.cn

JS:   process.exit(1)
来源：http://aq.bjjhwx.cn

TS:   process.exit(1)
来源：http://tt.hahajie.cn

Java: System.exit(1)
来源：http://vy.gzmigu.cn

Go:   os.Exit(1)
来源：http://kj.huixinmuqiang.cn

Ruby: exit 1
来源：http://ft.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ay.hnjuh.cn

[M06] 向标准错误输出
来源：http://bc.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://eu.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fg.haigaiapp.cn

JS:   console.error("err")
来源：http://dv.hnjuh.cn

TS:   console.error("err")
来源：http://km.haigaiapp.cn

Java: System.err.println("err")
来源：http://bd.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xz.lnxyls.cn

Ruby: warn "err"
来源：http://dn.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://tb.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://jz.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://fd.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vy.huanxung.cn

JS:   require.main === module
来源：http://kn.shtwfgs.cn

TS:   require.main === module
来源：http://uy.hnjuh.cn

Java: public static void main(String[] args)
来源：http://tm.szsharing.cn

Go:   func main()
来源：http://vd.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yw.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://jl.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://tf.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://kv.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://qu.521024.cn

JS:   process.platform;  process.version
来源：http://ku.szxytkj.cn

TS:   process.platform;  process.version
来源：http://vb.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hv.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kj.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xl.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://al.lnxyls.cn

================================================================================
来源：http://lg.chemitech.net.cn

N. 数据结构与算法
来源：http://ce.huanxung.cn

================================================================================
来源：http://au.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://hq.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cx.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ll.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gk.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sq.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://si.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://om.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dn.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bb.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ih.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://og.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jg.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ny.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://us.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uk.colortex.cn

Go:   slices.Sort(arr)
来源：http://es.lnxyls.cn

Ruby: arr.sort
来源：http://im.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ui.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://dr.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fe.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://un.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sn.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://re.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gz.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ls.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sm.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zn.nicolike.cn

[N04] 斐波那契数列
来源：http://ap.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ld.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nc.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zs.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dc.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yt.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nc.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gt.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ih.asd995.cn

[N05] 最大公约数
来源：http://ce.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://ms.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://br.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ye.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fz.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xj.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yt.nicolike.cn

Ruby: a.gcd(b)
来源：http://qc.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sw.9csxet.cn

[N06] 判断回文字符串
来源：http://td.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://wk.hahajie.cn

PHP:  $s === strrev($s);
来源：http://kv.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://xw.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://nz.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fp.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://fe.jctech888.com.cn

Ruby: s == s.reverse
来源：http://wt.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dt.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://vp.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wk.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ih.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oz.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://yb.gzmigu.cn

Java: // 手写 HashMap
来源：http://bv.9csxet.cn

Go:   // 手写 map[int]int
来源：http://bn.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://xx.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ox.jianghongdianzi.cn

[N08] 生成全排列
来源：http://xa.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://vf.newstarts.cn

PHP:  // 手写递归交换
来源：http://wq.shxzskj.cn

JS:   // 手写回溯递归
来源：http://lo.lnxyls.cn

TS:   // 手写回溯递归
来源：http://dw.jctech888.com.cn

Java: // 手写回溯递归
来源：http://kg.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://lq.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://ak.521024.cn

C#:   // 手写回溯递归
来源：http://fu.huixiangedu.cn

[N09] 栈与队列
来源：http://rz.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yj.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uy.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jq.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xc.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://th.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ma.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kl.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tt.gzmigu.cn

[N10] 链表节点定义
来源：http://cu.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xf.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qa.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nd.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ng.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://fg.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gl.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jo.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uf.hahajie.cn

[N11] 二叉树中序遍历
来源：http://rn.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mc.szxytkj.cn

PHP:  // 手写递归函数
来源：http://xk.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://or.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gs.huanxung.cn

Java: // 手写递归
来源：http://la.jianghongdianzi.cn

Go:   // 手写递归
来源：http://nx.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rl.bjjhwx.cn

C#:   // 手写递归
来源：http://bw.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wa.haigaiapp.cn


<!-- 参考信息 -->