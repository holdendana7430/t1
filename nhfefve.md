代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://xs.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fc.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pd.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nd.hnjuh.cn

[J08] 提取年月日与星期
来源：http://tk.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hl.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pr.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://up.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://la.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://it.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://st.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://go.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fu.szsharing.cn

[J09] 时区处理
来源：http://mz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fv.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yp.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bt.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://px.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yw.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ef.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://th.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mi.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://cf.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ox.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wb.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sn.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xg.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cp.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wx.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oi.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cq.jianghongdianzi.cn

================================================================================
来源：http://jq.hnjuh.cn

K. JSON 与序列化
来源：http://zc.huanxung.cn

================================================================================
来源：http://gm.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://te.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bd.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xq.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://el.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://in.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://no.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://kt.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ux.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gj.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://jw.muxihuayi.cn

Py:   json.loads(s)
来源：http://ez.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uq.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ft.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://yb.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mi.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://fb.nszjky.cn

Ruby: JSON.parse(s)
来源：http://hb.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iv.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://lh.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vy.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ok.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ao.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xp.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vs.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vo.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ct.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dr.colortex.cn

[K04] 读取 JSON 文件
来源：http://gt.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ll.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qz.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ez.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jk.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qb.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mh.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kb.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yg.wgjwhj.cn

[K05] 深拷贝对象
来源：http://tv.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://xu.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://xl.panjiajie.cn

JS:   structuredClone(obj)
来源：http://fe.hnjuh.cn

TS:   structuredClone(obj)
来源：http://xz.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yx.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jo.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qb.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sr.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://ce.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ea.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dq.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qw.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oc.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zt.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vd.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yu.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pm.shxzskj.cn

[K07] 进制转换
来源：http://am.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ke.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yj.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uv.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hh.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://km.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://my.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nl.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vr.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://us.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ri.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://uh.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://tz.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.jianghongdianzi.cn

Go:   encoding/gob
来源：http://rx.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://po.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nb.chemitech.net.cn

================================================================================
来源：http://gl.shtwfgs.cn

L. 网络请求
来源：http://uc.hnjuh.cn

================================================================================
来源：http://kl.hahajie.cn

[L01] 发送 GET 请求
来源：http://si.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gw.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jm.bookmarksfly.cn

JS:   await fetch(url)
来源：http://ts.9csxet.cn

TS:   await fetch(url)
来源：http://bb.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dt.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://tr.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dk.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ea.gzmigu.cn

[L02] 发送 POST JSON
来源：http://rb.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pz.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uc.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mt.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gy.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zw.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jo.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ky.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mb.panjiajie.cn

[L03] 设置自定义请求头
来源：http://vp.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fy.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://op.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mw.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rk.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wb.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ls.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dv.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eg.lnxyls.cn

[L04] 设置超时
来源：http://ov.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://hs.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cu.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fh.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zz.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kq.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lf.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jm.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tu.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://qh.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hg.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qd.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rb.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yn.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ca.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yl.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://le.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ad.nicolike.cn

[L06] 解析响应为 JSON
来源：http://zg.huixiangedu.cn

Py:   resp.json()
来源：http://vl.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://te.szxytkj.cn

JS:   await resp.json()
来源：http://ie.521024.cn

TS:   await resp.json()
来源：http://eh.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ua.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fg.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://hp.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wl.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://er.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://at.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://fy.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://tm.hnjuh.cn

Java: resp.statusCode()
来源：http://nd.hnjuh.cn

Go:   resp.StatusCode
来源：http://db.shxzukj.cn

Ruby: resp.code.to_i
来源：http://ir.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ui.asd995.cn

[L08] 并发请求多个地址
来源：http://nd.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sg.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://un.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kx.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pq.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jb.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uj.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yc.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sv.newstarts.cn

================================================================================
来源：http://jr.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://dg.muxihuayi.cn

================================================================================
来源：http://mp.colortex.cn

[M01] 读取命令行参数
来源：http://kr.szsharing.cn

Py:   sys.argv[1:]
来源：http://tu.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://ow.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://qn.szsharing.cn

TS:   process.argv.slice(2)
来源：http://lj.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://zl.haigaiapp.cn

Go:   os.Args[1:]
来源：http://eq.shtwfgs.cn

Ruby: ARGV
来源：http://wi.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://oi.wgjwhj.cn

[M02] 读取环境变量
来源：http://cj.asd995.cn

Py:   os.environ.get("HOME")
来源：http://kl.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ex.shtwfgs.cn

JS:   process.env.HOME
来源：http://av.lnxyls.cn

TS:   process.env.HOME
来源：http://mu.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://ss.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bj.szsharing.cn

Ruby: ENV["HOME"]
来源：http://qy.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ub.bjjhwx.cn

[M03] 执行外部命令
来源：http://jg.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ij.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qw.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eg.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://co.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zj.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wf.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rl.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ea.hnjuh.cn

[M04] 获取当前工作目录
来源：http://za.gzmigu.cn

Py:   os.getcwd()
来源：http://gb.nszjky.cn

PHP:  getcwd();
来源：http://hu.yuntaijiaju.cn

JS:   process.cwd()
来源：http://hi.shxzukj.cn

TS:   process.cwd()
来源：http://cg.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ab.nszjky.cn

Go:   os.Getwd()
来源：http://sr.muxihuayi.cn

Ruby: Dir.pwd
来源：http://tf.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rb.asd995.cn

[M05] 设置退出码
来源：http://qh.colortex.cn

Py:   sys.exit(1)
来源：http://xk.asd995.cn

PHP:  exit(1);
来源：http://wy.panjiajie.cn

JS:   process.exit(1)
来源：http://de.jctech888.com.cn

TS:   process.exit(1)
来源：http://hj.szsharing.cn

Java: System.exit(1)
来源：http://uk.lnxyls.cn

Go:   os.Exit(1)
来源：http://bn.muxihuayi.cn

Ruby: exit 1
来源：http://ub.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xf.521024.cn

[M06] 向标准错误输出
来源：http://sr.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://we.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tp.yuntaijiaju.cn

JS:   console.error("err")
来源：http://fj.nicolike.cn

TS:   console.error("err")
来源：http://xq.bjjhwx.cn

Java: System.err.println("err")
来源：http://jv.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nb.chemitech.net.cn

Ruby: warn "err"
来源：http://ar.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://lg.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://iu.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://wb.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ds.asd995.cn

JS:   require.main === module
来源：http://ug.nszjky.cn

TS:   require.main === module
来源：http://ne.hnjuh.cn

Java: public static void main(String[] args)
来源：http://xw.panjiajie.cn

Go:   func main()
来源：http://cq.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ad.521024.cn

C#:   static void Main(string[] args)
来源：http://kt.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://an.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://hr.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://qt.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://jd.huanxung.cn

TS:   process.platform;  process.version
来源：http://vd.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yq.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jj.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pr.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gb.chemitech.net.cn

================================================================================
来源：http://ab.chemitech.net.cn

N. 数据结构与算法
来源：http://lz.hahajie.cn

================================================================================
来源：http://kk.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://il.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ej.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kq.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fw.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tn.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://or.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ob.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://in.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://me.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://tj.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qm.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gp.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rh.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bu.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ge.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://ly.bookmarksfly.cn

Ruby: arr.sort
来源：http://cm.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ep.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://fq.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lj.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://yv.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ln.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hl.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uk.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iq.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oz.shxzskj.cn

[N04] 斐波那契数列
来源：http://qm.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tv.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ir.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nz.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pq.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ka.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vv.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zs.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jh.asd995.cn

[N05] 最大公约数
来源：http://hq.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://vq.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bm.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pa.hahajie.cn


<!-- 参考信息 -->