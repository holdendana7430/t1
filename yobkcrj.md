代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://iz.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aq.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dr.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ew.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qh.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fr.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://bh.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rb.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iu.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gc.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bp.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lq.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qi.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://km.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ti.hnjuh.cn

[K05] 深拷贝对象
来源：http://ve.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://zy.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://ax.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://su.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://as.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ci.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yt.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fd.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yp.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://de.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qy.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uw.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ec.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fd.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uy.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pk.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sw.gzmigu.cn

[K07] 进制转换
来源：http://dt.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ol.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ft.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rd.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ex.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ps.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pj.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yn.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wj.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ds.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://vd.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pk.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://eh.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://qr.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hs.haigaiapp.cn

Go:   encoding/gob
来源：http://ki.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://bv.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://to.yuexingan06.cn

================================================================================
来源：http://lx.szxytkj.cn

L. 网络请求
来源：http://zw.yuexingan06.cn

================================================================================
来源：http://jl.shxzukj.cn

[L01] 发送 GET 请求
来源：http://wa.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sk.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tp.huanxung.cn

JS:   await fetch(url)
来源：http://rm.bookmarksfly.cn

TS:   await fetch(url)
来源：http://fc.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ok.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://xg.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bt.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ty.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://wp.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wz.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fu.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aq.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uy.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xs.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fo.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ot.nszjky.cn

[L03] 设置自定义请求头
来源：http://iv.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zz.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uh.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jw.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ts.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oy.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sl.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://el.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jq.9csxet.cn

[L04] 设置超时
来源：http://xw.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://yc.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rn.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ai.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tl.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pp.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nr.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sf.nicolike.cn

[L05] 上传文件（multipart）
来源：http://wx.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ig.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://om.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sf.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pj.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hg.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fr.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ya.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oz.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://nt.lnxyls.cn

Py:   resp.json()
来源：http://fu.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://wi.szxytkj.cn

JS:   await resp.json()
来源：http://rc.colortex.cn

TS:   await resp.json()
来源：http://wr.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ac.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ej.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://qr.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ag.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://oy.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://an.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ia.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://uw.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://jp.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://ek.haigaiapp.cn

Go:   resp.StatusCode
来源：http://mc.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://ln.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ih.9csxet.cn

[L08] 并发请求多个地址
来源：http://si.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://au.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://pn.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ct.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://db.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fj.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vk.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jb.jctech888.com.cn

================================================================================
来源：http://wy.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://xo.9csxet.cn

================================================================================
来源：http://os.newstarts.cn

[M01] 读取命令行参数
来源：http://wl.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://jz.9csxet.cn

PHP:  $argv;  $argc;
来源：http://ws.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://xe.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://sb.colortex.cn

Java: args 数组（main 方法参数）
来源：http://mb.gzmigu.cn

Go:   os.Args[1:]
来源：http://qo.chemitech.net.cn

Ruby: ARGV
来源：http://ln.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://ky.muxihuayi.cn

[M02] 读取环境变量
来源：http://cr.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://gg.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zs.haigaiapp.cn

JS:   process.env.HOME
来源：http://vy.shxzskj.cn

TS:   process.env.HOME
来源：http://pm.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://zm.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ew.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://tk.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hc.muxihuayi.cn

[M03] 执行外部命令
来源：http://ld.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fd.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wk.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qo.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iu.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ut.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jx.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://vl.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://ga.gzmigu.cn

Py:   os.getcwd()
来源：http://ir.yuntaijiaju.cn

PHP:  getcwd();
来源：http://fn.huixinmuqiang.cn

JS:   process.cwd()
来源：http://cw.huanxung.cn

TS:   process.cwd()
来源：http://hn.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://oi.newstarts.cn

Go:   os.Getwd()
来源：http://wx.gzmigu.cn

Ruby: Dir.pwd
来源：http://ig.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jv.hnjuh.cn

[M05] 设置退出码
来源：http://vn.yuexingan06.cn

Py:   sys.exit(1)
来源：http://yb.bookmarksfly.cn

PHP:  exit(1);
来源：http://wy.shtwfgs.cn

JS:   process.exit(1)
来源：http://fh.gzmigu.cn

TS:   process.exit(1)
来源：http://dd.yuexingan06.cn

Java: System.exit(1)
来源：http://bj.hahajie.cn

Go:   os.Exit(1)
来源：http://rk.jctech888.com.cn

Ruby: exit 1
来源：http://ig.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qd.bjjhwx.cn

[M06] 向标准错误输出
来源：http://sv.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://nw.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sy.bookmarksfly.cn

JS:   console.error("err")
来源：http://is.newstarts.cn

TS:   console.error("err")
来源：http://fu.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ya.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zo.szsharing.cn

Ruby: warn "err"
来源：http://ge.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://pa.hnjuh.cn

[M07] 判断是否为主入口
来源：http://jv.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://hb.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ni.yuntaijiaju.cn

JS:   require.main === module
来源：http://ok.nicolike.cn

TS:   require.main === module
来源：http://ws.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://yo.chemitech.net.cn

Go:   func main()
来源：http://jg.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mb.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://st.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://xf.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://dd.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://be.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://wi.colortex.cn

TS:   process.platform;  process.version
来源：http://rv.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jm.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zr.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cn.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fu.nszjky.cn

================================================================================
来源：http://px.shxzukj.cn

N. 数据结构与算法
来源：http://wk.newstarts.cn

================================================================================
来源：http://oi.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://xp.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://le.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oj.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yb.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rr.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://uc.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cw.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ep.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://gl.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://ku.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rf.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ar.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kp.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tx.hahajie.cn

Go:   slices.Sort(arr)
来源：http://md.haigaiapp.cn

Ruby: arr.sort
来源：http://kf.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vk.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://qw.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fv.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://db.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cn.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hp.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bc.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eb.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hf.nszjky.cn

[N04] 斐波那契数列
来源：http://dn.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sz.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ng.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ae.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ct.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vq.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qt.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ep.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bx.gzmigu.cn

[N05] 最大公约数
来源：http://cm.nicolike.cn

Py:   math.gcd(a, b)
来源：http://vo.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tu.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gg.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pt.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dh.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jq.shxzukj.cn

Ruby: a.gcd(b)
来源：http://th.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fr.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ag.newstarts.cn

Py:   s == s[::-1]
来源：http://qr.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://gp.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ra.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://rl.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tf.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://qb.hahajie.cn

Ruby: s == s.reverse
来源：http://wo.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yy.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://jm.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://az.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pp.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jv.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://ev.szxytkj.cn

Java: // 手写 HashMap
来源：http://xo.asd995.cn

Go:   // 手写 map[int]int
来源：http://ok.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://om.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://og.muxihuayi.cn

[N08] 生成全排列
来源：http://tn.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://rx.szsharing.cn

PHP:  // 手写递归交换
来源：http://bf.hnjuh.cn

JS:   // 手写回溯递归
来源：http://cf.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://my.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://mf.szxytkj.cn

Go:   // 手写回溯递归
来源：http://at.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://kx.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://uv.nszjky.cn

[N09] 栈与队列
来源：http://ck.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lq.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pb.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ds.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vo.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mf.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://os.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ph.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ix.asd995.cn

[N10] 链表节点定义
来源：http://sp.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ar.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lx.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ka.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://he.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://ck.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zs.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ut.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fg.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://jt.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xt.szxytkj.cn

PHP:  // 手写递归函数
来源：http://sv.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ay.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wd.chemitech.net.cn

Java: // 手写递归
来源：http://tm.wgjwhj.cn


<!-- 参考信息 -->