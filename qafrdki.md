代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://so.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wd.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ap.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ti.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ac.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ya.hahajie.cn

[K04] 读取 JSON 文件
来源：http://lc.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://op.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ck.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dl.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://th.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dz.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vu.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cy.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rm.szsharing.cn

[K05] 深拷贝对象
来源：http://mr.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://up.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://mc.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://nv.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://cp.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://io.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ky.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kw.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://ci.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zu.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yw.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ss.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qz.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tp.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ri.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rm.yuexingan06.cn

[K07] 进制转换
来源：http://mx.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pf.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xr.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ri.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dm.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jh.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://so.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ab.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vr.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://xs.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://go.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qq.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://ul.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://wh.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mf.szxytkj.cn

Go:   encoding/gob
来源：http://wf.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://sv.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ik.hahajie.cn

================================================================================
来源：http://wk.newstarts.cn

L. 网络请求
来源：http://nc.colortex.cn

================================================================================
来源：http://zl.panjiajie.cn

[L01] 发送 GET 请求
来源：http://gs.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jr.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gf.shxzskj.cn

JS:   await fetch(url)
来源：http://sn.shtwfgs.cn

TS:   await fetch(url)
来源：http://rh.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ca.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://fe.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uk.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://it.szsharing.cn

[L02] 发送 POST JSON
来源：http://ne.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nh.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hf.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nj.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jy.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iz.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yv.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mq.asd995.cn

[L03] 设置自定义请求头
来源：http://qn.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cs.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xs.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sz.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hc.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lz.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hw.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ca.muxihuayi.cn

[L04] 设置超时
来源：http://bi.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://sb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rj.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hs.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yc.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dh.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ky.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sb.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ze.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://js.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rs.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xi.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ll.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vb.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wb.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lw.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pw.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jo.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://kp.9csxet.cn

Py:   resp.json()
来源：http://cm.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ae.521024.cn

JS:   await resp.json()
来源：http://ax.521024.cn

TS:   await resp.json()
来源：http://sr.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cn.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hu.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://kc.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ae.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://kk.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://az.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kw.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ur.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://jx.hahajie.cn

Java: resp.statusCode()
来源：http://qr.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://jw.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ag.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://lh.szxytkj.cn

[L08] 并发请求多个地址
来源：http://gm.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ja.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://ii.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ok.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ik.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ev.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tc.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://up.chemitech.net.cn

================================================================================
来源：http://ky.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://pl.chemitech.net.cn

================================================================================
来源：http://ab.huanxung.cn

[M01] 读取命令行参数
来源：http://vs.colortex.cn

Py:   sys.argv[1:]
来源：http://jd.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://nq.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://mj.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://ue.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://nj.shxzskj.cn

Go:   os.Args[1:]
来源：http://nh.shxzukj.cn

Ruby: ARGV
来源：http://gd.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://fx.shxzukj.cn

[M02] 读取环境变量
来源：http://pj.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://oi.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://io.chemitech.net.cn

JS:   process.env.HOME
来源：http://cx.szxytkj.cn

TS:   process.env.HOME
来源：http://ut.asd995.cn

Java: System.getenv("HOME")
来源：http://bl.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ge.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://ul.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qk.chemitech.net.cn

[M03] 执行外部命令
来源：http://pc.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hr.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xl.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pt.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xm.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rc.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ml.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jr.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://wu.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://pj.muxihuayi.cn

Py:   os.getcwd()
来源：http://re.huixiangedu.cn

PHP:  getcwd();
来源：http://je.nicolike.cn

JS:   process.cwd()
来源：http://wd.jianghongdianzi.cn

TS:   process.cwd()
来源：http://sr.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://fc.newstarts.cn

Go:   os.Getwd()
来源：http://ka.yuexingan06.cn

Ruby: Dir.pwd
来源：http://bk.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gz.yuntaijiaju.cn

[M05] 设置退出码
来源：http://id.bjjhwx.cn

Py:   sys.exit(1)
来源：http://po.9csxet.cn

PHP:  exit(1);
来源：http://bi.shtwfgs.cn

JS:   process.exit(1)
来源：http://rt.panjiajie.cn

TS:   process.exit(1)
来源：http://rp.wgjwhj.cn

Java: System.exit(1)
来源：http://fr.yuexingan06.cn

Go:   os.Exit(1)
来源：http://mk.wgjwhj.cn

Ruby: exit 1
来源：http://te.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cs.shxzskj.cn

[M06] 向标准错误输出
来源：http://jv.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://zd.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qt.haigaiapp.cn

JS:   console.error("err")
来源：http://vl.shxzukj.cn

TS:   console.error("err")
来源：http://nd.hnjuh.cn

Java: System.err.println("err")
来源：http://yy.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wc.jctech888.com.cn

Ruby: warn "err"
来源：http://iq.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://wy.newstarts.cn

[M07] 判断是否为主入口
来源：http://fc.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://gr.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.colortex.cn

JS:   require.main === module
来源：http://ww.huanxung.cn

TS:   require.main === module
来源：http://xw.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://zb.521024.cn

Go:   func main()
来源：http://az.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lh.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://tc.colortex.cn

[M08] 获取系统与运行时信息
来源：http://zn.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://xh.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://pc.shxzskj.cn

JS:   process.platform;  process.version
来源：http://iy.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://wf.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ei.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pu.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jm.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hw.newstarts.cn

================================================================================
来源：http://kk.hnjuh.cn

N. 数据结构与算法
来源：http://be.shxzskj.cn

================================================================================
来源：http://fx.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://dg.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cy.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://in.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ze.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qk.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ry.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://st.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mb.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bn.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gf.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://lj.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ea.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://es.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://os.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xe.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://so.panjiajie.cn

Ruby: arr.sort
来源：http://ss.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mp.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://ud.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xy.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://hx.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rr.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fr.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qt.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bh.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gq.nszjky.cn

[N04] 斐波那契数列
来源：http://id.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fb.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xv.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uz.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ue.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oq.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lc.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ju.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xw.jctech888.com.cn

[N05] 最大公约数
来源：http://fk.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://cl.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lx.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hj.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ue.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gg.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://on.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://wn.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pc.colortex.cn

[N06] 判断回文字符串
来源：http://br.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://tz.521024.cn

PHP:  $s === strrev($s);
来源：http://ob.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://bm.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://qr.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zr.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://uc.jctech888.com.cn

Ruby: s == s.reverse
来源：http://hl.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iz.asd995.cn

[N07] 两数之和（返回下标）
来源：http://op.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://df.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iq.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hx.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://xb.shxzukj.cn

Java: // 手写 HashMap
来源：http://nj.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://vt.hahajie.cn

Ruby: // 手写 Hash
来源：http://rb.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dy.521024.cn

[N08] 生成全排列
来源：http://wf.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://hx.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://gy.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://nt.nszjky.cn

TS:   // 手写回溯递归
来源：http://sy.szxytkj.cn

Java: // 手写回溯递归
来源：http://hy.gzmigu.cn

Go:   // 手写回溯递归
来源：http://sw.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://hi.szxytkj.cn

C#:   // 手写回溯递归
来源：http://wp.yuntaijiaju.cn

[N09] 栈与队列
来源：http://jg.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uu.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rl.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fq.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gv.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ta.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ce.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rs.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ky.chemitech.net.cn

[N10] 链表节点定义
来源：http://qv.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lz.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nj.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tu.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://va.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://uf.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://up.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tw.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kq.nicolike.cn

[N11] 二叉树中序遍历
来源：http://pp.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ta.shxzukj.cn

PHP:  // 手写递归函数
来源：http://jo.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kd.huixiangedu.cn

Java: // 手写递归
来源：http://bc.colortex.cn


<!-- 参考信息 -->