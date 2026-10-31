代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bm.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://af.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://li.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tx.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zj.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ov.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://se.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://sx.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yr.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zo.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lu.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://iz.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dt.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://gb.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nx.jctech888.com.cn

[J06] 计算两时间之差
来源：http://qg.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://zu.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://yo.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rf.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xv.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wv.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://oc.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://ft.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://xh.newstarts.cn

[J07] 比较两个日期
来源：http://vq.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://rw.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tx.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tj.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nc.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pn.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ob.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lq.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://uc.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://ot.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://co.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hw.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mj.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lx.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vt.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://io.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wp.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zt.huixinmuqiang.cn

[J09] 时区处理
来源：http://wv.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pu.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lq.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cl.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://we.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xi.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ez.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xq.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://we.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://af.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vp.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xr.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oe.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cx.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ed.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xm.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://we.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ya.jctech888.com.cn

================================================================================
来源：http://kb.shxzskj.cn

K. JSON 与序列化
来源：http://jc.yuntaijiaju.cn

================================================================================
来源：http://jd.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://bk.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ws.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ny.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ss.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://ov.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wd.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://zs.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pk.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://of.asd995.cn

[K02] JSON 字符串转对象
来源：http://pt.9csxet.cn

Py:   json.loads(s)
来源：http://pl.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nw.huanxung.cn

JS:   JSON.parse(s)
来源：http://aq.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://hc.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yh.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://ez.hahajie.cn

Ruby: JSON.parse(s)
来源：http://lo.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uz.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://za.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wz.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gq.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fo.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bp.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zk.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://er.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vx.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xv.szsharing.cn

[K04] 读取 JSON 文件
来源：http://rn.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uj.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://le.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cm.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://un.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://up.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ee.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dp.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gj.521024.cn

[K05] 深拷贝对象
来源：http://gr.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://nz.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://ul.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ba.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://qr.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://be.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://by.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vt.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://he.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://bz.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mw.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yf.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ea.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ok.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bu.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dj.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ow.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xp.muxihuayi.cn

[K07] 进制转换
来源：http://al.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nr.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://om.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://im.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mi.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yy.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lc.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lm.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pf.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://zh.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ev.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yx.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://lx.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://md.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ca.gzmigu.cn

Go:   encoding/gob
来源：http://ze.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ob.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wm.bookmarksfly.cn

================================================================================
来源：http://wo.bjjhwx.cn

L. 网络请求
来源：http://yz.9csxet.cn

================================================================================
来源：http://ps.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://tq.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wv.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rf.shtwfgs.cn

JS:   await fetch(url)
来源：http://lw.wgjwhj.cn

TS:   await fetch(url)
来源：http://dh.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jg.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://hq.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fb.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yf.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://de.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lr.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://um.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jw.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vs.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uu.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vv.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ed.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wx.9csxet.cn

[L03] 设置自定义请求头
来源：http://bw.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ty.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fd.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cn.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rh.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ht.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hu.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hx.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ox.shxzskj.cn

[L04] 设置超时
来源：http://sh.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://ka.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vg.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xx.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xu.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kd.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ql.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ho.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qk.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://bg.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mt.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xf.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fe.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pd.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nx.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kk.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nk.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://er.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://xn.bjjhwx.cn

Py:   resp.json()
来源：http://ru.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://hs.szxytkj.cn

JS:   await resp.json()
来源：http://qk.huanxung.cn

TS:   await resp.json()
来源：http://lx.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://br.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vd.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ry.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rr.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://dl.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pb.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tg.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://vj.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://xa.huixiangedu.cn

Java: resp.statusCode()
来源：http://ka.shxzskj.cn

Go:   resp.StatusCode
来源：http://tm.szsharing.cn

Ruby: resp.code.to_i
来源：http://zr.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://re.asd995.cn

[L08] 并发请求多个地址
来源：http://ts.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qd.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://vv.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fr.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://co.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kr.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jj.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wz.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dt.szxytkj.cn

================================================================================
来源：http://px.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://jt.huixiangedu.cn

================================================================================
来源：http://kp.huanxung.cn

[M01] 读取命令行参数
来源：http://ib.asd995.cn

Py:   sys.argv[1:]
来源：http://fm.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://nu.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ob.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://uy.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://mm.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://no.521024.cn

Ruby: ARGV
来源：http://ea.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://va.asd995.cn

[M02] 读取环境变量
来源：http://gf.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://xm.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ja.muxihuayi.cn

JS:   process.env.HOME
来源：http://yk.asd995.cn

TS:   process.env.HOME
来源：http://tb.lnxyls.cn

Java: System.getenv("HOME")
来源：http://mc.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gw.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://yj.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ip.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://hn.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eg.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bz.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uq.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wq.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ir.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ck.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://he.asd995.cn

[M04] 获取当前工作目录
来源：http://bk.chemitech.net.cn

Py:   os.getcwd()
来源：http://xo.wgjwhj.cn

PHP:  getcwd();
来源：http://em.szxytkj.cn

JS:   process.cwd()
来源：http://ye.huixinmuqiang.cn

TS:   process.cwd()
来源：http://em.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://es.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://he.colortex.cn

Ruby: Dir.pwd
来源：http://ol.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xp.asd995.cn

[M05] 设置退出码
来源：http://gw.szsharing.cn

Py:   sys.exit(1)
来源：http://mb.nszjky.cn

PHP:  exit(1);
来源：http://lg.asd995.cn

JS:   process.exit(1)
来源：http://rh.gzmigu.cn

TS:   process.exit(1)
来源：http://io.521024.cn

Java: System.exit(1)
来源：http://co.szsharing.cn

Go:   os.Exit(1)
来源：http://hd.bjjhwx.cn

Ruby: exit 1
来源：http://pa.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mc.huanxung.cn

[M06] 向标准错误输出
来源：http://be.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://yx.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dn.szsharing.cn

JS:   console.error("err")
来源：http://ej.shxzukj.cn

TS:   console.error("err")
来源：http://aq.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://pc.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kc.521024.cn

Ruby: warn "err"
来源：http://cp.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://kh.szsharing.cn

[M07] 判断是否为主入口
来源：http://iv.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://vl.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jz.bookmarksfly.cn

JS:   require.main === module
来源：http://bj.colortex.cn

TS:   require.main === module
来源：http://dg.shxzukj.cn

Java: public static void main(String[] args)
来源：http://rf.hnjuh.cn

Go:   func main()
来源：http://cm.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zz.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://qh.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://ic.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://ji.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vt.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://pi.szxytkj.cn

TS:   process.platform;  process.version
来源：http://gx.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xj.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cp.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ff.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pr.nszjky.cn

================================================================================
来源：http://vk.hnjuh.cn

N. 数据结构与算法
来源：http://fi.haigaiapp.cn

================================================================================
来源：http://oj.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://ue.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hh.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tj.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kz.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ri.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cd.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://pu.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://df.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ff.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://yy.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rj.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cz.panjiajie.cn


<!-- 参考信息 -->