代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jp.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yw.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ah.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://db.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vd.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lt.wgjwhj.cn

[J09] 时区处理
来源：http://pn.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zf.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xl.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kw.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nz.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vs.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vs.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xf.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uv.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://qg.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hy.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nt.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zv.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wp.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ao.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wf.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nl.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ak.haigaiapp.cn

================================================================================
来源：http://wh.huixinmuqiang.cn

K. JSON 与序列化
来源：http://yy.haigaiapp.cn

================================================================================
来源：http://jk.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://bf.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gw.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://al.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://do.asd995.cn

TS:   JSON.stringify(obj)
来源：http://vd.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rx.hahajie.cn

Go:   json.Marshal(obj)
来源：http://qw.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://at.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nt.colortex.cn

[K02] JSON 字符串转对象
来源：http://co.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://xr.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rw.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://jt.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://qt.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yr.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://gb.521024.cn

Ruby: JSON.parse(s)
来源：http://mu.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rc.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://dl.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bw.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zt.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vy.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ws.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ea.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bo.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://af.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zg.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://vn.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xb.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ec.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://el.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rr.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bv.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kc.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sm.hnjuh.cn

[K05] 深拷贝对象
来源：http://vs.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://rm.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ee.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://es.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://bz.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hm.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://th.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lo.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ma.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://no.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ej.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yo.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gd.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gq.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qf.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zs.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lm.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rr.muxihuayi.cn

[K07] 进制转换
来源：http://rx.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dy.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eg.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ok.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oi.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ms.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ee.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zz.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://km.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://yy.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://xy.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zj.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zl.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://sy.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://do.wgjwhj.cn

Go:   encoding/gob
来源：http://cr.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://al.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ev.muxihuayi.cn

================================================================================
来源：http://nb.hahajie.cn

L. 网络请求
来源：http://sw.colortex.cn

================================================================================
来源：http://lj.szxytkj.cn

[L01] 发送 GET 请求
来源：http://zh.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ow.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xh.hnjuh.cn

JS:   await fetch(url)
来源：http://vk.chemitech.net.cn

TS:   await fetch(url)
来源：http://wb.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cg.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://nz.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zn.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://br.hahajie.cn

[L02] 发送 POST JSON
来源：http://kh.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ly.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hb.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ko.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nf.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nl.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mm.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://th.newstarts.cn

[L03] 设置自定义请求头
来源：http://xq.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ke.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ig.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ta.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dn.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gq.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hc.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hm.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jw.gzmigu.cn

[L04] 设置超时
来源：http://yo.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://fv.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qx.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ch.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://la.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uf.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xy.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qw.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rz.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://rg.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yo.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eq.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vx.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://et.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lp.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ao.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rm.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jl.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ef.asd995.cn

Py:   resp.json()
来源：http://im.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://us.panjiajie.cn

JS:   await resp.json()
来源：http://iq.huanxung.cn

TS:   await resp.json()
来源：http://ib.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ns.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jb.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://br.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cr.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://vw.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gy.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qw.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://sz.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ps.shxzskj.cn

Java: resp.statusCode()
来源：http://eb.shxzukj.cn

Go:   resp.StatusCode
来源：http://ry.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://vg.521024.cn

C#:   (int)resp.StatusCode
来源：http://ya.521024.cn

[L08] 并发请求多个地址
来源：http://pr.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nj.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://zl.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pt.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fn.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hx.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ab.asd995.cn

================================================================================
来源：http://eh.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://qr.shtwfgs.cn

================================================================================
来源：http://gr.huanxung.cn

[M01] 读取命令行参数
来源：http://um.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://pe.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://kk.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://ec.colortex.cn

TS:   process.argv.slice(2)
来源：http://xh.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://gw.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ex.panjiajie.cn

Ruby: ARGV
来源：http://am.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://fj.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://iw.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://eo.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vc.hahajie.cn

JS:   process.env.HOME
来源：http://gp.huixiangedu.cn

TS:   process.env.HOME
来源：http://cf.521024.cn

Java: System.getenv("HOME")
来源：http://dy.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yu.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://su.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hx.wgjwhj.cn

[M03] 执行外部命令
来源：http://tv.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nl.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tm.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oz.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://az.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tj.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bv.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bd.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ss.lnxyls.cn

[M04] 获取当前工作目录
来源：http://cq.521024.cn

Py:   os.getcwd()
来源：http://gy.jctech888.com.cn

PHP:  getcwd();
来源：http://cq.colortex.cn

JS:   process.cwd()
来源：http://ay.jctech888.com.cn

TS:   process.cwd()
来源：http://kx.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://ee.shtwfgs.cn

Go:   os.Getwd()
来源：http://pk.gzmigu.cn

Ruby: Dir.pwd
来源：http://yx.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hc.hnjuh.cn

[M05] 设置退出码
来源：http://lz.panjiajie.cn

Py:   sys.exit(1)
来源：http://qd.jctech888.com.cn

PHP:  exit(1);
来源：http://my.newstarts.cn

JS:   process.exit(1)
来源：http://gz.shxzukj.cn

TS:   process.exit(1)
来源：http://uv.wgjwhj.cn

Java: System.exit(1)
来源：http://ba.muxihuayi.cn

Go:   os.Exit(1)
来源：http://po.lnxyls.cn

Ruby: exit 1
来源：http://lw.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ms.jctech888.com.cn

[M06] 向标准错误输出
来源：http://nw.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://pa.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cq.yuexingan06.cn

JS:   console.error("err")
来源：http://lc.gzmigu.cn

TS:   console.error("err")
来源：http://jm.521024.cn

Java: System.err.println("err")
来源：http://yt.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nc.newstarts.cn

Ruby: warn "err"
来源：http://pv.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ot.asd995.cn

[M07] 判断是否为主入口
来源：http://wt.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://ln.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hh.hnjuh.cn

JS:   require.main === module
来源：http://eg.jctech888.com.cn

TS:   require.main === module
来源：http://vs.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://sb.szsharing.cn

Go:   func main()
来源：http://sf.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pi.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ec.521024.cn

[M08] 获取系统与运行时信息
来源：http://qe.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://tx.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://xx.nicolike.cn

JS:   process.platform;  process.version
来源：http://tm.huanxung.cn

TS:   process.platform;  process.version
来源：http://uk.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bp.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ri.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qp.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xj.jctech888.com.cn

================================================================================
来源：http://nq.yuntaijiaju.cn

N. 数据结构与算法
来源：http://mb.jctech888.com.cn

================================================================================
来源：http://fs.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://cx.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://py.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pf.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xd.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://di.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qq.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://fa.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://os.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dd.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://sn.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://hn.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fb.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://og.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://br.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ax.nicolike.cn

Go:   slices.Sort(arr)
来源：http://ts.bjjhwx.cn

Ruby: arr.sort
来源：http://pp.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://db.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://py.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mr.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://al.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qk.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://at.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cq.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hf.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eh.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ek.9csxet.cn

[N04] 斐波那契数列
来源：http://ly.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zw.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dj.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kb.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://db.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ba.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gq.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cx.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pl.bookmarksfly.cn

[N05] 最大公约数
来源：http://ex.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://aa.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://la.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://em.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nb.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vx.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sz.panjiajie.cn

Ruby: a.gcd(b)
来源：http://uz.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fj.panjiajie.cn

[N06] 判断回文字符串
来源：http://wo.panjiajie.cn

Py:   s == s[::-1]
来源：http://ad.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://zu.haigaiapp.cn


<!-- 参考信息 -->