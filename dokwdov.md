代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://wf.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qg.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sc.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cv.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://yq.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://oa.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vo.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vl.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cq.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eb.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qx.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ui.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qt.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://na.jctech888.com.cn

[J09] 时区处理
来源：http://qw.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ww.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fq.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uy.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cv.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wk.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ho.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://on.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gv.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://yf.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ug.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bi.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xj.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ct.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vf.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ys.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jt.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cr.9csxet.cn

================================================================================
来源：http://kc.yuexingan06.cn

K. JSON 与序列化
来源：http://gy.szsharing.cn

================================================================================
来源：http://du.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://se.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zd.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ck.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://qi.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://pj.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mn.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://vd.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xk.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bj.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://zk.9csxet.cn

Py:   json.loads(s)
来源：http://ha.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xt.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://yp.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://gc.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vg.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mk.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://kx.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eo.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://ps.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fb.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pj.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fr.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xr.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zv.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nl.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://li.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yh.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ba.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vw.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ag.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ia.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tl.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sk.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wd.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vn.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rm.nicolike.cn

[K05] 深拷贝对象
来源：http://mq.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://mz.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://id.gzmigu.cn

JS:   structuredClone(obj)
来源：http://fd.szsharing.cn

TS:   structuredClone(obj)
来源：http://jm.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qm.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bf.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yt.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fq.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://tl.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://th.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dy.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fu.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yq.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kr.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wk.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kr.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ja.nszjky.cn

[K07] 进制转换
来源：http://md.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sz.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hi.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eo.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fz.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://re.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kh.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qu.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mo.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ft.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://tn.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dg.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://my.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mz.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hr.panjiajie.cn

Go:   encoding/gob
来源：http://tp.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://jw.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vy.wgjwhj.cn

================================================================================
来源：http://nm.shtwfgs.cn

L. 网络请求
来源：http://yu.shtwfgs.cn

================================================================================
来源：http://tv.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://nc.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://as.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ri.szxytkj.cn

JS:   await fetch(url)
来源：http://dw.9csxet.cn

TS:   await fetch(url)
来源：http://en.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ev.521024.cn

Go:   resp, err := http.Get(url)
来源：http://dm.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yz.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sf.521024.cn

[L02] 发送 POST JSON
来源：http://ln.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bf.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jt.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gx.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bn.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jj.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ax.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gh.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://st.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://va.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wf.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ll.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gc.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nq.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rf.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://an.huixiangedu.cn

[L04] 设置超时
来源：http://ai.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://ea.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rc.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vy.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vj.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yx.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hg.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lt.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qe.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://tz.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ub.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qi.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gf.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sx.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qa.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rw.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ez.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qf.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://tk.chemitech.net.cn

Py:   resp.json()
来源：http://fy.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ek.gzmigu.cn

JS:   await resp.json()
来源：http://kk.wgjwhj.cn

TS:   await resp.json()
来源：http://pw.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ak.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ef.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://xa.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ca.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://vc.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://io.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ax.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ng.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://zx.gzmigu.cn

Java: resp.statusCode()
来源：http://lx.hahajie.cn

Go:   resp.StatusCode
来源：http://py.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ko.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://bx.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://lc.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yj.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://eh.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pd.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cv.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zq.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kq.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wx.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://db.szsharing.cn

================================================================================
来源：http://ev.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://vw.huixinmuqiang.cn

================================================================================
来源：http://bn.hnjuh.cn

[M01] 读取命令行参数
来源：http://jz.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://fu.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://wi.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://bi.nszjky.cn

TS:   process.argv.slice(2)
来源：http://il.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://nd.colortex.cn

Go:   os.Args[1:]
来源：http://ah.huixinmuqiang.cn

Ruby: ARGV
来源：http://kr.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ah.bjjhwx.cn

[M02] 读取环境变量
来源：http://no.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://zr.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jn.huanxung.cn

JS:   process.env.HOME
来源：http://vb.huixiangedu.cn

TS:   process.env.HOME
来源：http://ls.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://js.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eu.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ud.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://th.szsharing.cn

[M03] 执行外部命令
来源：http://qo.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zv.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rl.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ww.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://px.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kb.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ca.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jx.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://uu.lnxyls.cn

[M04] 获取当前工作目录
来源：http://yk.jctech888.com.cn

Py:   os.getcwd()
来源：http://gw.chemitech.net.cn

PHP:  getcwd();
来源：http://tq.haigaiapp.cn

JS:   process.cwd()
来源：http://cx.szsharing.cn

TS:   process.cwd()
来源：http://ta.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://pc.wgjwhj.cn

Go:   os.Getwd()
来源：http://ji.shxzukj.cn

Ruby: Dir.pwd
来源：http://rb.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yj.bookmarksfly.cn

[M05] 设置退出码
来源：http://nh.huanxung.cn

Py:   sys.exit(1)
来源：http://cw.lnxyls.cn

PHP:  exit(1);
来源：http://dw.hahajie.cn

JS:   process.exit(1)
来源：http://wl.nicolike.cn

TS:   process.exit(1)
来源：http://xb.jctech888.com.cn

Java: System.exit(1)
来源：http://gy.chemitech.net.cn

Go:   os.Exit(1)
来源：http://wo.hnjuh.cn

Ruby: exit 1
来源：http://rf.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lo.yuexingan06.cn

[M06] 向标准错误输出
来源：http://rc.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ab.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lm.hahajie.cn

JS:   console.error("err")
来源：http://iv.yuexingan06.cn

TS:   console.error("err")
来源：http://ps.bjjhwx.cn

Java: System.err.println("err")
来源：http://gu.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://om.hahajie.cn

Ruby: warn "err"
来源：http://cc.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://jz.szxytkj.cn

[M07] 判断是否为主入口
来源：http://zo.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://nn.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kk.gzmigu.cn

JS:   require.main === module
来源：http://vg.521024.cn

TS:   require.main === module
来源：http://wm.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ea.hnjuh.cn

Go:   func main()
来源：http://ro.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ar.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://ee.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://an.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ci.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ha.hnjuh.cn

JS:   process.platform;  process.version
来源：http://te.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://yh.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lc.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jy.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://be.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nz.yuexingan06.cn

================================================================================
来源：http://qd.lnxyls.cn

N. 数据结构与算法
来源：http://zd.newstarts.cn

================================================================================
来源：http://fw.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://cd.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ku.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lq.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bk.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xv.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wi.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://em.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fm.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://lr.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zu.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vu.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kl.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kk.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://og.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://pl.huixinmuqiang.cn

Ruby: arr.sort
来源：http://yx.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://im.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://pv.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xm.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://mj.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uo.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fs.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uy.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fh.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ag.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lb.yuexingan06.cn

[N04] 斐波那契数列
来源：http://tm.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aa.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qh.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sg.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xj.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mj.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://po.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ih.bjjhwx.cn

[N05] 最大公约数
来源：http://iu.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://ui.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kf.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tv.jianghongdianzi.cn


<!-- 参考信息 -->