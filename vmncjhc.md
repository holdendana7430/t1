代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://gh.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wc.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://ao.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ql.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://cx.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wb.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://xm.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://zn.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://hk.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cl.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hg.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gh.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://in.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://nm.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ft.yuexingan06.cn

[J07] 比较两个日期
来源：http://jc.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://pg.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lr.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dh.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ba.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ov.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fv.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oz.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://cy.lnxyls.cn

[J08] 提取年月日与星期
来源：http://sh.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ot.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://li.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rj.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hq.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wm.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wx.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nm.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nx.newstarts.cn

[J09] 时区处理
来源：http://rf.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ic.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cj.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rg.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dn.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bt.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vu.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xb.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yp.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://rj.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zb.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ux.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ax.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ru.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qy.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://me.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lt.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wj.huanxung.cn

================================================================================
来源：http://vd.nszjky.cn

K. JSON 与序列化
来源：http://re.shtwfgs.cn

================================================================================
来源：http://pc.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://bg.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yi.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zu.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://lv.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://jd.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jj.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://zd.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lf.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sh.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://gu.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://nj.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wl.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://bf.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://wf.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yd.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://ww.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://dt.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ba.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://ow.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jc.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aq.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oo.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vs.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bu.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qw.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kh.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rl.szsharing.cn

[K04] 读取 JSON 文件
来源：http://hd.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nj.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://in.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gp.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://le.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yh.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nu.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cp.newstarts.cn

[K05] 深拷贝对象
来源：http://lg.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://eu.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://yb.szsharing.cn

JS:   structuredClone(obj)
来源：http://sy.lnxyls.cn

TS:   structuredClone(obj)
来源：http://fv.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ya.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qk.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hj.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nz.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ij.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pw.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nu.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cj.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ev.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ff.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zc.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://co.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qm.hnjuh.cn

[K07] 进制转换
来源：http://kg.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zm.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iv.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cl.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oy.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qj.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jz.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nc.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wh.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://mu.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://kx.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ok.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://yx.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://yp.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fu.huixinmuqiang.cn

Go:   encoding/gob
来源：http://iw.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://dy.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mb.jianghongdianzi.cn

================================================================================
来源：http://gv.jianghongdianzi.cn

L. 网络请求
来源：http://vy.jianghongdianzi.cn

================================================================================
来源：http://lv.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://yj.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eb.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lj.bjjhwx.cn

JS:   await fetch(url)
来源：http://dx.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://to.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gp.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://ev.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://js.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://av.9csxet.cn

[L02] 发送 POST JSON
来源：http://yl.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://te.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aj.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qj.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ua.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ii.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wx.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hq.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ad.huanxung.cn

[L03] 设置自定义请求头
来源：http://vk.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ez.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eq.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fk.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wp.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nb.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://af.nszjky.cn

[L04] 设置超时
来源：http://jy.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://ss.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ja.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lq.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ua.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://en.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mp.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gy.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qz.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://tl.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sg.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kc.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ip.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xy.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kn.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hf.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ub.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://yr.muxihuayi.cn

Py:   resp.json()
来源：http://fb.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://pb.haigaiapp.cn

JS:   await resp.json()
来源：http://vn.huanxung.cn

TS:   await resp.json()
来源：http://hd.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yc.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mq.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://nu.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ip.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://ss.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hw.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aj.asd995.cn

JS:   resp.ok;  resp.status
来源：http://ts.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://cw.lnxyls.cn

Java: resp.statusCode()
来源：http://nk.shxzukj.cn

Go:   resp.StatusCode
来源：http://uu.nicolike.cn

Ruby: resp.code.to_i
来源：http://ml.colortex.cn

C#:   (int)resp.StatusCode
来源：http://uh.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://qw.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jp.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://rj.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nc.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ym.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qq.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://um.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tx.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zl.huixinmuqiang.cn

================================================================================
来源：http://lp.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://vw.huixiangedu.cn

================================================================================
来源：http://dx.nszjky.cn

[M01] 读取命令行参数
来源：http://aj.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://sr.nszjky.cn

PHP:  $argv;  $argc;
来源：http://cn.nszjky.cn

JS:   process.argv.slice(2)
来源：http://ed.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://uo.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://bw.huanxung.cn

Go:   os.Args[1:]
来源：http://rg.hnjuh.cn

Ruby: ARGV
来源：http://mm.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://rt.bjjhwx.cn

[M02] 读取环境变量
来源：http://ix.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ue.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oj.521024.cn

JS:   process.env.HOME
来源：http://zv.muxihuayi.cn

TS:   process.env.HOME
来源：http://hp.newstarts.cn

Java: System.getenv("HOME")
来源：http://dn.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://we.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://gt.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cu.panjiajie.cn

[M03] 执行外部命令
来源：http://hz.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fu.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rg.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xs.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mg.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://em.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zx.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kj.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://hq.nicolike.cn

[M04] 获取当前工作目录
来源：http://yd.szsharing.cn

Py:   os.getcwd()
来源：http://fp.colortex.cn

PHP:  getcwd();
来源：http://if.chemitech.net.cn

JS:   process.cwd()
来源：http://mq.yuexingan06.cn

TS:   process.cwd()
来源：http://qv.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://qx.shxzskj.cn

Go:   os.Getwd()
来源：http://xe.huanxung.cn

Ruby: Dir.pwd
来源：http://hd.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bm.jctech888.com.cn

[M05] 设置退出码
来源：http://hk.huanxung.cn

Py:   sys.exit(1)
来源：http://cv.chemitech.net.cn

PHP:  exit(1);
来源：http://uj.hahajie.cn

JS:   process.exit(1)
来源：http://bw.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ee.panjiajie.cn

Java: System.exit(1)
来源：http://ey.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://da.lnxyls.cn

Ruby: exit 1
来源：http://fb.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sy.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://ob.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://wh.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xa.haigaiapp.cn

JS:   console.error("err")
来源：http://gy.huanxung.cn

TS:   console.error("err")
来源：http://vv.muxihuayi.cn

Java: System.err.println("err")
来源：http://no.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xn.521024.cn

Ruby: warn "err"
来源：http://ha.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://ad.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://cq.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://ex.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qw.jctech888.com.cn

JS:   require.main === module
来源：http://xo.hnjuh.cn

TS:   require.main === module
来源：http://dc.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://up.bookmarksfly.cn

Go:   func main()
来源：http://un.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://us.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://oc.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://sp.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://ow.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://jt.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://hf.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://ed.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rc.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xm.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sj.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ko.wgjwhj.cn

================================================================================
来源：http://oo.shtwfgs.cn

N. 数据结构与算法
来源：http://qd.huixinmuqiang.cn

================================================================================
来源：http://xf.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://kt.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kt.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gx.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pc.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qh.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lb.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://nj.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tl.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://im.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ye.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ax.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xd.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qp.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ds.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ck.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://wx.hnjuh.cn

Ruby: arr.sort
来源：http://qa.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mx.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://xl.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fn.jianghongdianzi.cn


<!-- 参考信息 -->