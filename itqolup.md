代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://jx.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kb.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mb.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tw.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gv.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bp.9csxet.cn

[K04] 读取 JSON 文件
来源：http://et.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gw.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ig.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ct.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zj.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tv.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qo.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://px.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rc.colortex.cn

[K05] 深拷贝对象
来源：http://jx.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://ul.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://zq.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://ox.521024.cn

TS:   structuredClone(obj)
来源：http://xp.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ut.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wg.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ju.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ar.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://kz.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zs.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cs.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ta.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ml.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zi.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ev.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sr.shxzukj.cn

[K07] 进制转换
来源：http://my.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://it.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gy.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oe.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mg.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sp.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hl.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dt.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ir.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://cw.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://id.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mg.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://gg.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://zs.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vb.huixinmuqiang.cn

Go:   encoding/gob
来源：http://zy.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://sf.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://je.shxzukj.cn

================================================================================
来源：http://bj.gzmigu.cn

L. 网络请求
来源：http://bz.yuntaijiaju.cn

================================================================================
来源：http://cd.asd995.cn

[L01] 发送 GET 请求
来源：http://uk.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mv.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wy.haigaiapp.cn

JS:   await fetch(url)
来源：http://pr.hahajie.cn

TS:   await fetch(url)
来源：http://xf.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zt.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://cg.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yy.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gi.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://le.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ah.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hf.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://go.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ss.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aj.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vm.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ae.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://mp.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zh.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://km.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://st.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fi.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cj.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bo.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ig.szxytkj.cn

[L04] 设置超时
来源：http://gj.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://kb.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ja.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hy.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tx.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yu.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yf.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zq.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://be.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://nw.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bn.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mn.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cs.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wc.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qh.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ge.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wz.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://th.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://fx.haigaiapp.cn

Py:   resp.json()
来源：http://he.9csxet.cn

PHP:  json_decode($body, true);
来源：http://wf.szsharing.cn

JS:   await resp.json()
来源：http://lv.colortex.cn

TS:   await resp.json()
来源：http://cx.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cu.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tn.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://mc.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://up.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://yi.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://br.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wm.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://fe.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://hp.9csxet.cn

Java: resp.statusCode()
来源：http://ji.hnjuh.cn

Go:   resp.StatusCode
来源：http://wm.panjiajie.cn

Ruby: resp.code.to_i
来源：http://of.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://rk.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://xj.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eh.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://er.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://el.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ub.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oq.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nf.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jl.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cm.yuexingan06.cn

================================================================================
来源：http://nm.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://jm.colortex.cn

================================================================================
来源：http://af.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://bg.newstarts.cn

Py:   sys.argv[1:]
来源：http://iq.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://dt.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://lq.nszjky.cn

TS:   process.argv.slice(2)
来源：http://cl.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://wa.shxzukj.cn

Go:   os.Args[1:]
来源：http://dg.yuexingan06.cn

Ruby: ARGV
来源：http://dh.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ee.hahajie.cn

[M02] 读取环境变量
来源：http://tx.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://jc.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zc.bjjhwx.cn

JS:   process.env.HOME
来源：http://ns.huixiangedu.cn

TS:   process.env.HOME
来源：http://ti.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://kp.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cl.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://xa.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eh.lnxyls.cn

[M03] 执行外部命令
来源：http://rr.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ua.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zw.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cj.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gk.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xd.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uq.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pl.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://en.panjiajie.cn

[M04] 获取当前工作目录
来源：http://kx.asd995.cn

Py:   os.getcwd()
来源：http://ey.nszjky.cn

PHP:  getcwd();
来源：http://to.haigaiapp.cn

JS:   process.cwd()
来源：http://no.lnxyls.cn

TS:   process.cwd()
来源：http://em.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://qw.panjiajie.cn

Go:   os.Getwd()
来源：http://za.chemitech.net.cn

Ruby: Dir.pwd
来源：http://rz.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tp.haigaiapp.cn

[M05] 设置退出码
来源：http://zu.lnxyls.cn

Py:   sys.exit(1)
来源：http://jf.nicolike.cn

PHP:  exit(1);
来源：http://ue.nicolike.cn

JS:   process.exit(1)
来源：http://am.hnjuh.cn

TS:   process.exit(1)
来源：http://qi.szxytkj.cn

Java: System.exit(1)
来源：http://ib.muxihuayi.cn

Go:   os.Exit(1)
来源：http://sw.nszjky.cn

Ruby: exit 1
来源：http://lu.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nn.9csxet.cn

[M06] 向标准错误输出
来源：http://qi.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://jl.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pd.newstarts.cn

JS:   console.error("err")
来源：http://fv.huanxung.cn

TS:   console.error("err")
来源：http://pn.nszjky.cn

Java: System.err.println("err")
来源：http://ob.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ax.shxzskj.cn

Ruby: warn "err"
来源：http://sg.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://mc.521024.cn

[M07] 判断是否为主入口
来源：http://ha.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://sg.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hq.huixiangedu.cn

JS:   require.main === module
来源：http://vf.bjjhwx.cn

TS:   require.main === module
来源：http://ei.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://wx.shxzukj.cn

Go:   func main()
来源：http://ev.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cg.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://ub.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://wp.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ws.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://dt.shxzukj.cn

JS:   process.platform;  process.version
来源：http://qj.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://st.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nm.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vj.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://az.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tl.hahajie.cn

================================================================================
来源：http://ha.bjjhwx.cn

N. 数据结构与算法
来源：http://ji.yuntaijiaju.cn

================================================================================
来源：http://ha.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://db.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yg.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ba.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://my.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ng.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yu.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ne.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vx.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qf.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://pk.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://cv.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kb.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://px.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qs.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kl.szsharing.cn

Go:   slices.Sort(arr)
来源：http://za.lnxyls.cn

Ruby: arr.sort
来源：http://xl.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xt.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://ij.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://de.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://co.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hh.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gu.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tl.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lh.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ak.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pe.jctech888.com.cn

[N04] 斐波那契数列
来源：http://hx.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ps.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nk.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rh.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ro.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eg.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ig.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cj.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kp.shxzskj.cn

[N05] 最大公约数
来源：http://yh.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://qk.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ks.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://po.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hr.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rt.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ar.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://yo.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bp.yuexingan06.cn

[N06] 判断回文字符串
来源：http://na.521024.cn

Py:   s == s[::-1]
来源：http://qv.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://rw.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://og.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://kg.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kv.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://ux.wgjwhj.cn

Ruby: s == s.reverse
来源：http://ii.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jg.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ax.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zy.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ew.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zu.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://js.9csxet.cn

Java: // 手写 HashMap
来源：http://bf.nszjky.cn

Go:   // 手写 map[int]int
来源：http://op.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://tn.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vq.jianghongdianzi.cn

[N08] 生成全排列
来源：http://pi.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://us.nszjky.cn

PHP:  // 手写递归交换
来源：http://pa.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://qr.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://ik.nszjky.cn

Java: // 手写回溯递归
来源：http://ev.shxzukj.cn

Go:   // 手写回溯递归
来源：http://gr.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://hw.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://kv.shtwfgs.cn

[N09] 栈与队列
来源：http://kc.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fr.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wd.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pn.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sf.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yb.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yp.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ge.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xa.hahajie.cn

[N10] 链表节点定义
来源：http://nh.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oz.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aq.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://if.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ob.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://qg.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ax.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fj.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kn.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://ji.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ww.huanxung.cn

PHP:  // 手写递归函数
来源：http://jo.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tc.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ly.shxzskj.cn

Java: // 手写递归
来源：http://th.jianghongdianzi.cn


<!-- 参考信息 -->