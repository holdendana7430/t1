代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://ia.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://er.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mg.asd995.cn

[I05] 按正则拆分
来源：http://mu.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cs.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fu.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ui.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://gc.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://mv.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pz.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yg.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wv.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ir.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tc.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eb.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://op.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wu.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nr.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ie.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fi.521024.cn

[I07] 忽略大小写与多行模式
来源：http://oy.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uy.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pb.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://br.hnjuh.cn

TS:   /error/gim
来源：http://fy.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rk.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zi.521024.cn

Ruby: s.scan(/error/i)
来源：http://er.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pm.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://co.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bz.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dt.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bn.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ec.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wj.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kk.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fb.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ei.colortex.cn

================================================================================
来源：http://ce.chemitech.net.cn

J. 日期与时间
来源：http://cp.lnxyls.cn

================================================================================
来源：http://qv.shxzskj.cn

[J01] 获取当前时间
来源：http://mb.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nz.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oi.huanxung.cn

JS:   new Date();  Date.now()
来源：http://hi.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://dd.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://en.hnjuh.cn

Go:   time.Now()
来源：http://yy.shxzukj.cn

Ruby: Time.now
来源：http://yi.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ui.9csxet.cn

[J02] 格式化输出
来源：http://cj.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lu.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oc.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ax.newstarts.cn

TS:   d.toISOString()
来源：http://nl.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bf.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sr.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ru.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bd.colortex.cn

[J03] 字符串解析为日期
来源：http://gd.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aa.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xx.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://wb.521024.cn

TS:   new Date("2024-01-02")
来源：http://kz.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wu.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mx.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://rn.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tz.nicolike.cn

[J04] 时间戳与日期互转
来源：http://zc.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hk.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ad.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tu.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gq.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://be.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hi.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kf.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ot.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://qh.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://na.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xi.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ty.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xz.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://jo.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nq.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://xi.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uj.szxytkj.cn

[J06] 计算两时间之差
来源：http://of.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://al.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://br.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ei.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zh.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sw.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://dp.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://jp.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://dd.szsharing.cn

[J07] 比较两个日期
来源：http://eq.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://wp.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qw.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jt.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dc.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ou.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gz.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ts.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ap.szsharing.cn

[J08] 提取年月日与星期
来源：http://ud.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ds.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://om.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rv.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kf.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fi.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sk.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nz.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vy.shxzukj.cn

[J09] 时区处理
来源：http://in.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://no.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://og.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ft.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hg.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nn.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mr.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pw.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://dv.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fb.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lw.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ce.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ft.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lh.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jx.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hh.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://th.panjiajie.cn

================================================================================
来源：http://kr.newstarts.cn

K. JSON 与序列化
来源：http://cn.521024.cn

================================================================================
来源：http://hh.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://qm.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yx.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zk.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://ep.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ju.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ju.szsharing.cn

Go:   json.Marshal(obj)
来源：http://rd.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ql.nicolike.cn

[K02] JSON 字符串转对象
来源：http://cw.hahajie.cn

Py:   json.loads(s)
来源：http://ll.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sx.521024.cn

JS:   JSON.parse(s)
来源：http://xc.newstarts.cn

TS:   JSON.parse(s)
来源：http://eu.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yb.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://bn.521024.cn

Ruby: JSON.parse(s)
来源：http://gy.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kh.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://cr.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qs.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jb.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zq.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qy.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://es.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qb.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xr.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://co.521024.cn

[K04] 读取 JSON 文件
来源：http://ri.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ra.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zk.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cl.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xc.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tv.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vz.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ug.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lq.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://li.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://zc.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://oc.szsharing.cn

JS:   structuredClone(obj)
来源：http://lt.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://gy.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fg.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bp.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kx.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xf.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://lk.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://db.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aa.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yn.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://go.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lo.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rb.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ts.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kw.huixinmuqiang.cn

[K07] 进制转换
来源：http://ka.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lq.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cr.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uy.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zs.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://te.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yr.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bz.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wl.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://vs.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://cv.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tc.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://ku.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://xv.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vu.lnxyls.cn

Go:   encoding/gob
来源：http://zd.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ol.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yg.wgjwhj.cn

================================================================================
来源：http://oe.bjjhwx.cn

L. 网络请求
来源：http://xj.shtwfgs.cn

================================================================================
来源：http://lz.szxytkj.cn

[L01] 发送 GET 请求
来源：http://az.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bd.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cm.lnxyls.cn

JS:   await fetch(url)
来源：http://xn.yuexingan06.cn

TS:   await fetch(url)
来源：http://tt.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://en.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://ol.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://og.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ba.lnxyls.cn

[L02] 发送 POST JSON
来源：http://fe.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aa.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lk.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ip.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ka.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ij.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gi.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://se.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ot.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://wp.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dy.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nb.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gg.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://my.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lo.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yc.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jq.shtwfgs.cn

[L04] 设置超时
来源：http://qy.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://jw.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://py.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sb.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wt.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kr.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gd.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uu.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ui.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ag.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yy.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://go.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://in.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pm.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mc.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vz.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lk.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cj.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://jz.shtwfgs.cn

Py:   resp.json()
来源：http://xh.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://nw.hnjuh.cn

JS:   await resp.json()
来源：http://vu.lnxyls.cn

TS:   await resp.json()
来源：http://pq.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ns.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://li.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://nu.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fm.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://fe.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uo.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ou.asd995.cn

JS:   resp.ok;  resp.status
来源：http://ct.asd995.cn

TS:   resp.ok;  resp.status
来源：http://dt.szxytkj.cn

Java: resp.statusCode()
来源：http://kx.shxzskj.cn

Go:   resp.StatusCode
来源：http://ou.nicolike.cn

Ruby: resp.code.to_i
来源：http://rv.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://kz.gzmigu.cn

[L08] 并发请求多个地址
来源：http://pw.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ee.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://la.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bj.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lz.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fl.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ux.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vn.yuntaijiaju.cn

================================================================================
来源：http://vd.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://vs.shtwfgs.cn

================================================================================
来源：http://zi.hnjuh.cn

[M01] 读取命令行参数
来源：http://im.hnjuh.cn

Py:   sys.argv[1:]
来源：http://gc.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://vs.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ld.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://if.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://ed.huixiangedu.cn

Go:   os.Args[1:]
来源：http://sa.hnjuh.cn

Ruby: ARGV
来源：http://rn.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://ie.szsharing.cn

[M02] 读取环境变量
来源：http://vh.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://md.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ce.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://to.bjjhwx.cn

TS:   process.env.HOME
来源：http://bj.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://oz.nicolike.cn


<!-- 参考信息 -->