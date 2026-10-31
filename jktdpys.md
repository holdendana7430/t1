代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://xo.huanxung.cn

[J08] 提取年月日与星期
来源：http://xu.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cs.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pr.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jj.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vo.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gr.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ts.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fu.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ta.hahajie.cn

[J09] 时区处理
来源：http://oz.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dl.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ar.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ck.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ar.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aq.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kh.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://po.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cb.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://jj.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://te.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sr.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cu.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iy.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jz.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fm.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://em.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oz.colortex.cn

================================================================================
来源：http://ac.panjiajie.cn

K. JSON 与序列化
来源：http://ek.hahajie.cn

================================================================================
来源：http://il.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://sm.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zo.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://po.colortex.cn

JS:   JSON.stringify(obj)
来源：http://kc.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://oc.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ir.szsharing.cn

Go:   json.Marshal(obj)
来源：http://pv.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pz.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://da.nicolike.cn

[K02] JSON 字符串转对象
来源：http://qs.bookmarksfly.cn

Py:   json.loads(s)
来源：http://xb.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zz.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://oj.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://mj.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wn.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://bs.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://ol.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qr.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://nw.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qm.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ky.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vm.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dd.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wh.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://av.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sv.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kt.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://mj.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://me.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nb.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lo.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ba.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rh.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qr.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dd.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xp.shxzskj.cn

[K05] 深拷贝对象
来源：http://zz.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://ax.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://yv.nicolike.cn

JS:   structuredClone(obj)
来源：http://gi.hnjuh.cn

TS:   structuredClone(obj)
来源：http://ap.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kp.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sy.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ln.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zh.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://rn.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dw.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yz.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zt.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rr.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fy.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://av.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hd.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sd.hahajie.cn

[K07] 进制转换
来源：http://cb.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pp.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://el.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vk.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wg.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vr.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hu.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ho.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xw.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://hm.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://tj.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kr.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://lc.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://nr.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://df.9csxet.cn

Go:   encoding/gob
来源：http://ic.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://gp.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gr.chemitech.net.cn

================================================================================
来源：http://qn.haigaiapp.cn

L. 网络请求
来源：http://av.yuntaijiaju.cn

================================================================================
来源：http://cw.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://uj.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wb.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zc.gzmigu.cn

JS:   await fetch(url)
来源：http://zn.jctech888.com.cn

TS:   await fetch(url)
来源：http://fw.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pi.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://mw.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wj.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dq.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://kl.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lo.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://it.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ib.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://id.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cu.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ax.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jp.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qm.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://yz.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ec.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ju.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yf.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://th.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rw.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://im.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://we.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mj.bjjhwx.cn

[L04] 设置超时
来源：http://xh.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://mh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ax.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jx.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kh.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yj.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aw.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bk.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://eq.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oq.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zu.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ow.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://da.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vv.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bb.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://en.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hc.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://jf.huixinmuqiang.cn

Py:   resp.json()
来源：http://ny.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://kl.nszjky.cn

JS:   await resp.json()
来源：http://jv.shxzskj.cn

TS:   await resp.json()
来源：http://na.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://er.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gs.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://mf.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uq.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ot.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pg.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oh.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://kp.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://nt.9csxet.cn

Java: resp.statusCode()
来源：http://jt.gzmigu.cn

Go:   resp.StatusCode
来源：http://iz.szxytkj.cn

Ruby: resp.code.to_i
来源：http://ip.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://ek.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://pq.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://df.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://un.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://va.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ee.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tr.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qq.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fi.hahajie.cn

================================================================================
来源：http://py.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://us.9csxet.cn

[M01] 读取命令行参数
来源：http://av.szxytkj.cn

Py:   sys.argv[1:]
来源：http://vq.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://uh.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://lz.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://il.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://pb.bjjhwx.cn

Go:   os.Args[1:]
来源：http://og.nicolike.cn

Ruby: ARGV
来源：http://au.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://tz.gzmigu.cn

[M02] 读取环境变量
来源：http://qd.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://pk.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rm.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://sg.bjjhwx.cn

TS:   process.env.HOME
来源：http://ez.9csxet.cn

Java: System.getenv("HOME")
来源：http://rt.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://he.huanxung.cn

Ruby: ENV["HOME"]
来源：http://fx.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vb.nszjky.cn

[M03] 执行外部命令
来源：http://jj.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zu.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ju.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rs.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ie.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hk.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ps.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gl.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://fd.521024.cn

[M04] 获取当前工作目录
来源：http://pf.huixiangedu.cn

Py:   os.getcwd()
来源：http://hw.nszjky.cn

PHP:  getcwd();
来源：http://hl.shtwfgs.cn

JS:   process.cwd()
来源：http://uj.panjiajie.cn

TS:   process.cwd()
来源：http://lj.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://pr.szxytkj.cn

Go:   os.Getwd()
来源：http://cv.wgjwhj.cn

Ruby: Dir.pwd
来源：http://gt.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xt.szsharing.cn

[M05] 设置退出码
来源：http://fi.hahajie.cn

Py:   sys.exit(1)
来源：http://sv.bjjhwx.cn

PHP:  exit(1);
来源：http://xw.huixiangedu.cn

JS:   process.exit(1)
来源：http://ii.szxytkj.cn

TS:   process.exit(1)
来源：http://ps.nszjky.cn

Java: System.exit(1)
来源：http://ct.lnxyls.cn

Go:   os.Exit(1)
来源：http://hs.shxzukj.cn

Ruby: exit 1
来源：http://vf.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bo.hahajie.cn

[M06] 向标准错误输出
来源：http://of.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://vq.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jg.shxzskj.cn

JS:   console.error("err")
来源：http://va.chemitech.net.cn

TS:   console.error("err")
来源：http://fw.bjjhwx.cn

Java: System.err.println("err")
来源：http://to.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dj.hahajie.cn

Ruby: warn "err"
来源：http://oy.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://rl.huanxung.cn

[M07] 判断是否为主入口
来源：http://ul.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://bs.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ut.bookmarksfly.cn

JS:   require.main === module
来源：http://uq.szxytkj.cn

TS:   require.main === module
来源：http://hu.huanxung.cn

Java: public static void main(String[] args)
来源：http://nt.hahajie.cn

Go:   func main()
来源：http://yb.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bf.colortex.cn

C#:   static void Main(string[] args)
来源：http://dz.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://jg.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ds.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gs.shxzskj.cn

JS:   process.platform;  process.version
来源：http://vu.nicolike.cn

TS:   process.platform;  process.version
来源：http://fc.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://be.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xq.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vw.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ku.huanxung.cn

================================================================================
来源：http://dd.jianghongdianzi.cn

N. 数据结构与算法
来源：http://gs.huixinmuqiang.cn

================================================================================
来源：http://um.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://bj.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wt.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oz.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wm.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ko.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vu.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://td.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ra.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ou.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://qk.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://dv.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zx.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qd.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pd.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kc.huanxung.cn

Go:   slices.Sort(arr)
来源：http://gr.nicolike.cn

Ruby: arr.sort
来源：http://xm.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cs.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://bl.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vz.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://dm.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qf.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vk.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://up.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ng.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qy.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zk.shxzukj.cn

[N04] 斐波那契数列
来源：http://px.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nk.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wb.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://be.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dd.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ti.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ih.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mw.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ww.newstarts.cn

[N05] 最大公约数
来源：http://kj.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://lr.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gl.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ri.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kk.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cr.hnjuh.cn

Ruby: a.gcd(b)
来源：http://cn.shxzskj.cn


<!-- 参考信息 -->