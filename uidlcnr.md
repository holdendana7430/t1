代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xt.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ss.bookmarksfly.cn

[J09] 时区处理
来源：http://jn.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gn.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vt.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ge.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://az.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zk.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dz.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vf.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://fr.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yl.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://td.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sq.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sq.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ev.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zk.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ip.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zk.yuntaijiaju.cn

================================================================================
来源：http://ad.colortex.cn

K. JSON 与序列化
来源：http://ks.hnjuh.cn

================================================================================
来源：http://vt.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://uk.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ay.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ws.521024.cn

JS:   JSON.stringify(obj)
来源：http://xt.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://to.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lj.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://bb.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://or.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hk.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://bh.muxihuayi.cn

Py:   json.loads(s)
来源：http://qf.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bf.colortex.cn

JS:   JSON.parse(s)
来源：http://hx.huanxung.cn

TS:   JSON.parse(s)
来源：http://sg.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dc.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://pk.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://fp.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lt.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://gs.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oj.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vt.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xb.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qn.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ui.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ks.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ed.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qr.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://lp.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hy.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://au.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fl.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oe.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sg.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ub.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fi.9csxet.cn

[K05] 深拷贝对象
来源：http://gu.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://si.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://hh.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://uh.hnjuh.cn

TS:   structuredClone(obj)
来源：http://xz.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zm.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ng.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://px.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kw.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://mg.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gz.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bg.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yl.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gk.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ni.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zg.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cg.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rh.bookmarksfly.cn

[K07] 进制转换
来源：http://un.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://at.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yt.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aa.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ge.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zd.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://id.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mj.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jo.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://ma.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://mf.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vw.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://uk.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://bt.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tr.bjjhwx.cn

Go:   encoding/gob
来源：http://jd.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://dx.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uu.huixiangedu.cn

================================================================================
来源：http://ms.hahajie.cn

L. 网络请求
来源：http://nv.muxihuayi.cn

================================================================================
来源：http://dd.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://da.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dh.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xv.muxihuayi.cn

JS:   await fetch(url)
来源：http://js.chemitech.net.cn

TS:   await fetch(url)
来源：http://bz.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ht.521024.cn

Go:   resp, err := http.Get(url)
来源：http://tu.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oz.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xq.colortex.cn

[L02] 发送 POST JSON
来源：http://pz.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sd.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gr.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yc.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yr.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ag.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qo.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://up.newstarts.cn

[L03] 设置自定义请求头
来源：http://ea.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xc.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fn.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://de.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vz.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wb.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dw.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yy.asd995.cn

[L04] 设置超时
来源：http://ix.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://fb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nf.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fo.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ve.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nf.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ym.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ik.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://mr.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kk.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://io.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zm.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jt.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bx.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sx.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vs.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://ru.haigaiapp.cn

Py:   resp.json()
来源：http://ha.nicolike.cn

PHP:  json_decode($body, true);
来源：http://ka.bookmarksfly.cn

JS:   await resp.json()
来源：http://qb.nicolike.cn

TS:   await resp.json()
来源：http://mh.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oa.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://np.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://wx.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gt.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://pn.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://if.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cr.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://rc.asd995.cn

TS:   resp.ok;  resp.status
来源：http://gl.hnjuh.cn

Java: resp.statusCode()
来源：http://fk.shxzukj.cn

Go:   resp.StatusCode
来源：http://rv.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://ml.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://eo.9csxet.cn

[L08] 并发请求多个地址
来源：http://gi.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pe.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://gf.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vj.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://te.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dd.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sp.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qd.nicolike.cn

================================================================================
来源：http://zs.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://pw.wgjwhj.cn

================================================================================
来源：http://ty.gzmigu.cn

[M01] 读取命令行参数
来源：http://fa.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://hc.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://mo.newstarts.cn

JS:   process.argv.slice(2)
来源：http://mx.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://gg.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://bg.lnxyls.cn

Go:   os.Args[1:]
来源：http://zb.nicolike.cn

Ruby: ARGV
来源：http://wb.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://bf.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://em.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://sv.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dw.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://bk.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://lj.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://ft.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hp.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ke.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ic.haigaiapp.cn

[M03] 执行外部命令
来源：http://ov.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ua.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dc.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ti.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bn.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kg.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ni.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vn.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://dt.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://lu.chemitech.net.cn

Py:   os.getcwd()
来源：http://vm.nszjky.cn

PHP:  getcwd();
来源：http://hg.nszjky.cn

JS:   process.cwd()
来源：http://bk.gzmigu.cn

TS:   process.cwd()
来源：http://za.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://dg.bjjhwx.cn

Go:   os.Getwd()
来源：http://fd.shtwfgs.cn

Ruby: Dir.pwd
来源：http://bh.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://te.muxihuayi.cn

[M05] 设置退出码
来源：http://gn.huixiangedu.cn

Py:   sys.exit(1)
来源：http://px.bookmarksfly.cn

PHP:  exit(1);
来源：http://ed.nicolike.cn

JS:   process.exit(1)
来源：http://dl.panjiajie.cn

TS:   process.exit(1)
来源：http://oa.yuexingan06.cn

Java: System.exit(1)
来源：http://oo.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://zb.lnxyls.cn

Ruby: exit 1
来源：http://ck.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jl.521024.cn

[M06] 向标准错误输出
来源：http://rn.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://mx.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ln.panjiajie.cn

JS:   console.error("err")
来源：http://hu.chemitech.net.cn

TS:   console.error("err")
来源：http://be.panjiajie.cn

Java: System.err.println("err")
来源：http://mh.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yc.yuexingan06.cn

Ruby: warn "err"
来源：http://ig.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://iz.9csxet.cn

[M07] 判断是否为主入口
来源：http://ad.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://fz.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pp.chemitech.net.cn

JS:   require.main === module
来源：http://xy.panjiajie.cn

TS:   require.main === module
来源：http://dv.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ur.shtwfgs.cn

Go:   func main()
来源：http://ua.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hk.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://ax.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://qc.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://sj.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://rh.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://cz.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://gv.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qt.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tr.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yo.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uy.wgjwhj.cn

================================================================================
来源：http://js.haigaiapp.cn

N. 数据结构与算法
来源：http://in.hahajie.cn

================================================================================
来源：http://io.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://qn.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kk.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jd.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ie.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uy.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://io.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://la.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ps.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://up.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://kq.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://ps.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://js.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jx.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://za.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pu.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://zb.huanxung.cn

Ruby: arr.sort
来源：http://qw.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ei.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://lg.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://up.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ae.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zy.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kk.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fw.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ay.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mp.nszjky.cn

[N04] 斐波那契数列
来源：http://ak.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://px.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vh.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mu.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://to.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://td.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zv.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ut.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qq.shxzskj.cn

[N05] 最大公约数
来源：http://lw.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://mt.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tx.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ra.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ch.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qc.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://as.hahajie.cn

Ruby: a.gcd(b)
来源：http://os.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ct.lnxyls.cn

[N06] 判断回文字符串
来源：http://ja.szxytkj.cn

Py:   s == s[::-1]
来源：http://ue.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://qm.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ic.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://ju.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sw.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://sv.huanxung.cn


<!-- 参考信息 -->