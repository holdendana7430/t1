代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hc.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nn.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kh.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xd.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yc.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eo.yuexingan06.cn

[J09] 时区处理
来源：http://aw.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tb.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cg.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://co.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cx.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://on.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vl.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jw.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://du.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://mo.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fo.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://et.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kx.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gv.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nz.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sw.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yn.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nq.gzmigu.cn

================================================================================
来源：http://zx.nszjky.cn

K. JSON 与序列化
来源：http://wv.shtwfgs.cn

================================================================================
来源：http://xx.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://rt.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fs.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pa.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://zm.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://xq.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yd.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://vx.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wv.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ut.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://xh.lnxyls.cn

Py:   json.loads(s)
来源：http://yo.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://he.panjiajie.cn

JS:   JSON.parse(s)
来源：http://qu.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://fm.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://es.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://tf.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://kq.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ll.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://pt.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ar.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jy.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vl.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ix.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yn.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xx.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ee.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qq.colortex.cn

[K04] 读取 JSON 文件
来源：http://tl.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tb.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://we.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ze.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yo.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ns.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gh.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ir.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wd.panjiajie.cn

[K05] 深拷贝对象
来源：http://jh.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://fc.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://pr.colortex.cn

JS:   structuredClone(obj)
来源：http://ef.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://fr.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yt.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sw.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ip.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fu.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://rh.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pj.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qo.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ov.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ai.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jc.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yl.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://be.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nz.panjiajie.cn

[K07] 进制转换
来源：http://ju.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nd.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://er.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vr.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bm.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sj.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uq.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dt.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fx.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://gm.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pq.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://qv.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ee.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sn.9csxet.cn

Go:   encoding/gob
来源：http://ct.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://iz.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jh.9csxet.cn

================================================================================
来源：http://bv.521024.cn

L. 网络请求
来源：http://vc.chemitech.net.cn

================================================================================
来源：http://gq.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ym.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yl.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pd.hnjuh.cn

JS:   await fetch(url)
来源：http://xs.nicolike.cn

TS:   await fetch(url)
来源：http://uo.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cs.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://lp.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lh.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ja.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://ml.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sc.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ot.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eu.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ms.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://al.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sx.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hy.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yi.panjiajie.cn

[L03] 设置自定义请求头
来源：http://up.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://en.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ul.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lo.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yf.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ju.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jh.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kv.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://um.colortex.cn

[L04] 设置超时
来源：http://ae.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://qg.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gt.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ha.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mo.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ga.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sp.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jz.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ij.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://bf.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ch.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qy.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tj.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dd.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uy.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ij.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tb.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ue.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://ll.hnjuh.cn

Py:   resp.json()
来源：http://yb.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://xx.panjiajie.cn

JS:   await resp.json()
来源：http://st.hahajie.cn

TS:   await resp.json()
来源：http://sj.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nf.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aa.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://uc.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xq.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://fq.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://px.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zz.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://ij.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://jl.bjjhwx.cn

Java: resp.statusCode()
来源：http://nk.colortex.cn

Go:   resp.StatusCode
来源：http://rh.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ur.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://zp.shxzskj.cn

[L08] 并发请求多个地址
来源：http://by.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zl.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://tl.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mu.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zd.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oa.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ar.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qg.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xx.huixiangedu.cn

================================================================================
来源：http://ll.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://bv.bjjhwx.cn

================================================================================
来源：http://cr.wgjwhj.cn

[M01] 读取命令行参数
来源：http://gv.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://mt.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://ux.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ih.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://gg.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://yl.lnxyls.cn

Go:   os.Args[1:]
来源：http://zx.hnjuh.cn

Ruby: ARGV
来源：http://ij.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://zv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://pl.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://tb.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ue.huanxung.cn

JS:   process.env.HOME
来源：http://da.chemitech.net.cn

TS:   process.env.HOME
来源：http://zt.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://eh.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bs.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://rx.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qy.shxzukj.cn

[M03] 执行外部命令
来源：http://lj.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kl.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xs.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yp.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yl.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cw.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://co.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xc.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://jz.lnxyls.cn

[M04] 获取当前工作目录
来源：http://lh.bjjhwx.cn

Py:   os.getcwd()
来源：http://he.colortex.cn

PHP:  getcwd();
来源：http://nt.jctech888.com.cn

JS:   process.cwd()
来源：http://xx.shtwfgs.cn

TS:   process.cwd()
来源：http://du.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://gx.wgjwhj.cn

Go:   os.Getwd()
来源：http://fr.shxzukj.cn

Ruby: Dir.pwd
来源：http://hz.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lj.nicolike.cn

[M05] 设置退出码
来源：http://ks.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ld.haigaiapp.cn

PHP:  exit(1);
来源：http://gw.shxzskj.cn

JS:   process.exit(1)
来源：http://fi.panjiajie.cn

TS:   process.exit(1)
来源：http://ud.yuntaijiaju.cn

Java: System.exit(1)
来源：http://wq.lnxyls.cn

Go:   os.Exit(1)
来源：http://iy.huixinmuqiang.cn

Ruby: exit 1
来源：http://ku.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yy.huixiangedu.cn

[M06] 向标准错误输出
来源：http://gm.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://dy.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://de.nicolike.cn

JS:   console.error("err")
来源：http://qn.shxzskj.cn

TS:   console.error("err")
来源：http://jp.bjjhwx.cn

Java: System.err.println("err")
来源：http://sr.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kn.chemitech.net.cn

Ruby: warn "err"
来源：http://gx.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://or.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://xf.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://yn.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xa.colortex.cn

JS:   require.main === module
来源：http://dv.521024.cn

TS:   require.main === module
来源：http://pn.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ww.szxytkj.cn

Go:   func main()
来源：http://py.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mf.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://kr.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://zq.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://st.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://xd.nszjky.cn

JS:   process.platform;  process.version
来源：http://kn.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://me.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sg.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ct.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jp.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pd.bookmarksfly.cn

================================================================================
来源：http://ot.colortex.cn

N. 数据结构与算法
来源：http://kc.huixiangedu.cn

================================================================================
来源：http://nq.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://sj.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qq.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mn.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://if.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dd.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://rz.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wg.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zn.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://mk.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zk.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fk.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rb.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gp.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wf.nicolike.cn

Go:   slices.Sort(arr)
来源：http://vz.hahajie.cn

Ruby: arr.sort
来源：http://nm.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lw.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://uo.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jn.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://zf.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xb.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tz.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qg.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nd.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://no.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ur.chemitech.net.cn

[N04] 斐波那契数列
来源：http://ew.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ex.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://he.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kk.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cv.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dp.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ps.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pe.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xv.muxihuayi.cn

[N05] 最大公约数
来源：http://vw.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://br.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jq.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dn.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ve.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cj.huanxung.cn

Ruby: a.gcd(b)
来源：http://uc.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rm.wgjwhj.cn

[N06] 判断回文字符串
来源：http://nb.szsharing.cn

Py:   s == s[::-1]
来源：http://nm.asd995.cn

PHP:  $s === strrev($s);
来源：http://wf.bookmarksfly.cn


<!-- 参考信息 -->