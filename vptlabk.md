代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://yu.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nt.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wy.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vv.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ft.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://xe.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vu.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dn.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fa.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://us.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qr.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lm.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kl.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oy.shxzskj.cn

[J09] 时区处理
来源：http://jm.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tm.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zr.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cf.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ek.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tg.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://th.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mr.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uu.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://iv.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nr.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ln.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://de.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qq.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sj.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ey.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lv.521024.cn

================================================================================
来源：http://bu.bookmarksfly.cn

K. JSON 与序列化
来源：http://td.szsharing.cn

================================================================================
来源：http://er.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://oo.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qr.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ps.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://rs.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://nf.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://co.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://zs.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wq.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dz.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://du.huixiangedu.cn

Py:   json.loads(s)
来源：http://pl.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zy.colortex.cn

JS:   JSON.parse(s)
来源：http://ba.szxytkj.cn

TS:   JSON.parse(s)
来源：http://eg.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lt.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://qe.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://rn.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zt.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://gj.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jc.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vp.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eo.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mi.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pp.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ww.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ip.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://io.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://yl.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bz.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dt.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cm.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gk.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mc.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pu.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ug.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ho.colortex.cn

[K05] 深拷贝对象
来源：http://ah.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://wa.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ym.521024.cn

JS:   structuredClone(obj)
来源：http://de.asd995.cn

TS:   structuredClone(obj)
来源：http://me.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tl.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pm.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cs.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qz.9csxet.cn

[K06] 解析 URL 查询串
来源：http://da.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ya.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hf.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vv.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ux.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mp.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cc.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://go.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vx.yuexingan06.cn

[K07] 进制转换
来源：http://zm.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ws.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kk.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gr.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hy.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kl.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kq.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oq.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cv.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://yl.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://en.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ex.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ir.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://dz.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bf.hnjuh.cn

Go:   encoding/gob
来源：http://fz.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://cb.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xx.szxytkj.cn

================================================================================
来源：http://ou.shxzukj.cn

L. 网络请求
来源：http://yh.colortex.cn

================================================================================
来源：http://xb.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ee.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lx.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vz.hahajie.cn

JS:   await fetch(url)
来源：http://vk.chemitech.net.cn

TS:   await fetch(url)
来源：http://yg.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mp.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ht.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bs.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ns.colortex.cn

[L02] 发送 POST JSON
来源：http://ur.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://du.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sc.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aw.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dt.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xj.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://st.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sg.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xl.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://nw.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sm.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://df.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fy.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kq.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cm.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ks.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iq.hahajie.cn

[L04] 设置超时
来源：http://su.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://ee.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fx.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://px.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pf.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ju.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ii.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qu.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://km.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oy.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hx.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rg.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iv.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iv.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wg.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qq.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ug.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ic.hahajie.cn

Py:   resp.json()
来源：http://rc.szsharing.cn

PHP:  json_decode($body, true);
来源：http://pf.jctech888.com.cn

JS:   await resp.json()
来源：http://it.yuexingan06.cn

TS:   await resp.json()
来源：http://aq.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mm.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://le.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://rc.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rh.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://gs.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qm.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oy.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ij.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://da.panjiajie.cn

Java: resp.statusCode()
来源：http://xl.huanxung.cn

Go:   resp.StatusCode
来源：http://qs.huanxung.cn

Ruby: resp.code.to_i
来源：http://sb.521024.cn

C#:   (int)resp.StatusCode
来源：http://mt.shxzukj.cn

[L08] 并发请求多个地址
来源：http://zo.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vc.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://on.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wm.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ly.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wn.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yr.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ow.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dg.shxzskj.cn

================================================================================
来源：http://im.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://gd.lnxyls.cn

================================================================================
来源：http://qd.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://xj.521024.cn

Py:   sys.argv[1:]
来源：http://vc.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://hu.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://hj.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://un.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://tf.nicolike.cn

Go:   os.Args[1:]
来源：http://km.szxytkj.cn

Ruby: ARGV
来源：http://li.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://er.jctech888.com.cn

[M02] 读取环境变量
来源：http://rp.colortex.cn

Py:   os.environ.get("HOME")
来源：http://bv.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qb.asd995.cn

JS:   process.env.HOME
来源：http://iz.yuexingan06.cn

TS:   process.env.HOME
来源：http://ep.hahajie.cn

Java: System.getenv("HOME")
来源：http://ii.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jo.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://sx.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gr.bjjhwx.cn

[M03] 执行外部命令
来源：http://sa.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xn.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://py.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://px.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yh.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zb.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ec.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yb.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://jr.nszjky.cn

[M04] 获取当前工作目录
来源：http://in.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://ma.chemitech.net.cn

PHP:  getcwd();
来源：http://tw.huanxung.cn

JS:   process.cwd()
来源：http://vp.bookmarksfly.cn

TS:   process.cwd()
来源：http://ve.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://uk.hahajie.cn

Go:   os.Getwd()
来源：http://oi.hnjuh.cn

Ruby: Dir.pwd
来源：http://zt.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rh.haigaiapp.cn

[M05] 设置退出码
来源：http://bh.wgjwhj.cn

Py:   sys.exit(1)
来源：http://vz.lnxyls.cn

PHP:  exit(1);
来源：http://vs.jctech888.com.cn

JS:   process.exit(1)
来源：http://fz.jctech888.com.cn

TS:   process.exit(1)
来源：http://yf.huixinmuqiang.cn

Java: System.exit(1)
来源：http://na.muxihuayi.cn

Go:   os.Exit(1)
来源：http://sx.9csxet.cn

Ruby: exit 1
来源：http://mi.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uy.newstarts.cn

[M06] 向标准错误输出
来源：http://pn.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://gd.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://er.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ms.hahajie.cn

TS:   console.error("err")
来源：http://ow.jctech888.com.cn

Java: System.err.println("err")
来源：http://qc.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qq.szxytkj.cn

Ruby: warn "err"
来源：http://ft.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://um.9csxet.cn

[M07] 判断是否为主入口
来源：http://km.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ca.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hp.yuntaijiaju.cn

JS:   require.main === module
来源：http://nk.haigaiapp.cn

TS:   require.main === module
来源：http://cu.szsharing.cn

Java: public static void main(String[] args)
来源：http://bb.hahajie.cn

Go:   func main()
来源：http://hy.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yb.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ct.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://uk.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://gw.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://wq.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ty.szxytkj.cn

TS:   process.platform;  process.version
来源：http://nu.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lx.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mo.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ba.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ni.szsharing.cn

================================================================================
来源：http://fd.yuntaijiaju.cn

N. 数据结构与算法
来源：http://oc.jianghongdianzi.cn

================================================================================
来源：http://ys.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://sp.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wf.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ah.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://se.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uy.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rs.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ir.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yg.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://st.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://du.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://kp.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ke.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lq.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fh.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ev.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://dy.chemitech.net.cn

Ruby: arr.sort
来源：http://hb.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sb.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://so.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lo.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://xh.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uw.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wl.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bu.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hy.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dw.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ne.hahajie.cn

[N04] 斐波那契数列
来源：http://to.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cm.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yl.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pm.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qs.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uk.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nr.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://us.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yv.shxzskj.cn

[N05] 最大公约数
来源：http://ui.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://jl.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nw.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ua.nicolike.cn


<!-- 参考信息 -->