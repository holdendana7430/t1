代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://qh.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://si.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://qh.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ns.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ao.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ic.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hc.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://un.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ap.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xe.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xq.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yg.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kw.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ms.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pl.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rw.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://bz.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jl.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rx.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xy.bjjhwx.cn

TS:   /error/gim
来源：http://oa.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ly.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ik.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://ne.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hu.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://tz.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ft.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gj.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ed.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://at.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qi.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sy.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tu.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qo.lnxyls.cn

================================================================================
来源：http://ec.521024.cn

J. 日期与时间
来源：http://xl.panjiajie.cn

================================================================================
来源：http://lt.hahajie.cn

[J01] 获取当前时间
来源：http://fb.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cb.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qy.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ws.colortex.cn

TS:   new Date();  Date.now()
来源：http://rb.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pw.szsharing.cn

Go:   time.Now()
来源：http://mg.huanxung.cn

Ruby: Time.now
来源：http://uf.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lr.jianghongdianzi.cn

[J02] 格式化输出
来源：http://xb.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xk.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nv.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://az.shtwfgs.cn

TS:   d.toISOString()
来源：http://bw.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://td.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vt.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uc.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ee.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://xb.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ax.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://og.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://cm.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ug.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ul.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ko.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://hl.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cy.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://xa.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kk.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jv.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://la.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ey.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vd.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zp.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ds.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lt.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://bs.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://rb.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qo.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vd.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ak.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://lg.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zu.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://cg.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ap.hnjuh.cn

[J06] 计算两时间之差
来源：http://wo.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://do.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://lm.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mk.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://li.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://ka.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://nz.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://ax.9csxet.cn

[J07] 比较两个日期
来源：http://gy.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://lq.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qx.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sr.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fc.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://je.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cz.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zy.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://aq.9csxet.cn

[J08] 提取年月日与星期
来源：http://rw.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ho.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ta.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ze.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xd.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vd.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://co.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mk.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hm.huixiangedu.cn

[J09] 时区处理
来源：http://rl.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tn.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mv.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mt.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zp.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ud.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://we.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jg.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://st.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wc.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ex.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wh.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iw.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oa.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tg.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uu.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qt.wgjwhj.cn

================================================================================
来源：http://lf.szxytkj.cn

K. JSON 与序列化
来源：http://cc.gzmigu.cn

================================================================================
来源：http://zp.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://qq.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fl.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://og.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://jr.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://xe.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lm.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://fh.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wh.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zs.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://xj.521024.cn

Py:   json.loads(s)
来源：http://xd.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vz.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://oo.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://xj.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sx.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://wo.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://wx.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pm.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ru.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cv.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kz.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fe.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cm.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ty.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zd.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nx.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ic.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://su.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vf.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iz.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rw.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rx.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ta.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fl.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ua.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tb.521024.cn

[K05] 深拷贝对象
来源：http://wz.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://ji.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://fe.newstarts.cn

JS:   structuredClone(obj)
来源：http://es.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://xl.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ro.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://je.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ga.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ew.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://fx.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bd.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jt.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nm.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tu.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lz.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rg.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://im.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ce.panjiajie.cn

[K07] 进制转换
来源：http://gh.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tc.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oz.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ph.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bn.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fg.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gg.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kt.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ag.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://ws.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://gu.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mk.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://kb.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://co.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pn.shxzskj.cn

Go:   encoding/gob
来源：http://uv.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://yt.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vx.hnjuh.cn

================================================================================
来源：http://ob.shxzskj.cn

L. 网络请求
来源：http://wq.muxihuayi.cn

================================================================================
来源：http://qu.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://nm.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tq.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kw.muxihuayi.cn

JS:   await fetch(url)
来源：http://jy.asd995.cn

TS:   await fetch(url)
来源：http://pt.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ri.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ok.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xv.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zd.nicolike.cn

[L02] 发送 POST JSON
来源：http://ck.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qx.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rt.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://po.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tp.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aj.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qy.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mr.szxytkj.cn

[L03] 设置自定义请求头
来源：http://bf.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ii.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rt.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ka.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ej.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ll.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mk.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://et.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wn.szsharing.cn

[L04] 设置超时
来源：http://ly.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://jk.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ny.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zw.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ht.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://si.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bb.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uy.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://sz.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ga.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ig.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lm.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ac.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://me.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sm.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kd.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://bb.lnxyls.cn

Py:   resp.json()
来源：http://cb.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://tp.jianghongdianzi.cn

JS:   await resp.json()
来源：http://lz.nszjky.cn

TS:   await resp.json()
来源：http://wz.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jm.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jl.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ge.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ck.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://rx.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ls.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nf.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://ij.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://fw.wgjwhj.cn

Java: resp.statusCode()
来源：http://ky.newstarts.cn

Go:   resp.StatusCode
来源：http://gl.asd995.cn

Ruby: resp.code.to_i
来源：http://cn.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://lz.hahajie.cn

[L08] 并发请求多个地址
来源：http://yb.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hq.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ky.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wf.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hn.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ek.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qj.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dm.521024.cn

================================================================================
来源：http://nx.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://kw.newstarts.cn

================================================================================
来源：http://nm.panjiajie.cn

[M01] 读取命令行参数
来源：http://hl.hnjuh.cn

Py:   sys.argv[1:]
来源：http://gw.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://jh.nszjky.cn

JS:   process.argv.slice(2)
来源：http://hf.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://pt.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://hg.shxzukj.cn

Go:   os.Args[1:]
来源：http://jp.lnxyls.cn

Ruby: ARGV
来源：http://kz.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://ur.asd995.cn

[M02] 读取环境变量
来源：http://kx.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://pu.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oq.colortex.cn

JS:   process.env.HOME
来源：http://do.chemitech.net.cn

TS:   process.env.HOME
来源：http://tk.nszjky.cn

Java: System.getenv("HOME")
来源：http://on.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cj.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://rb.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sx.bookmarksfly.cn

[M03] 执行外部命令
来源：http://hy.haigaiapp.cn


<!-- 参考信息 -->