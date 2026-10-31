代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qk.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rk.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pb.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pm.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zh.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ag.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dz.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://tg.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://js.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ei.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ar.muxihuayi.cn

TS:   /error/gim
来源：http://vg.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://da.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zp.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://oj.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hp.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rw.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nu.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hx.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dk.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gf.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://du.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qw.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rk.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://de.huanxung.cn

================================================================================
来源：http://rj.huanxung.cn

J. 日期与时间
来源：http://pa.chemitech.net.cn

================================================================================
来源：http://aq.chemitech.net.cn

[J01] 获取当前时间
来源：http://qq.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mh.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bk.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://sq.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://sd.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ki.huanxung.cn

Go:   time.Now()
来源：http://cm.asd995.cn

Ruby: Time.now
来源：http://pc.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yw.nszjky.cn

[J02] 格式化输出
来源：http://mn.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://em.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lk.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://on.haigaiapp.cn

TS:   d.toISOString()
来源：http://zf.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dc.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://je.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bi.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nb.shxzukj.cn

[J03] 字符串解析为日期
来源：http://rf.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sz.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sz.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://dx.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://af.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qk.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xa.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://kj.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mz.521024.cn

[J04] 时间戳与日期互转
来源：http://xg.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gd.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pl.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mv.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fd.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gf.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uu.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ug.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ry.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://qs.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://pn.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ha.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xf.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pw.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://dk.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mx.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://sm.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ih.gzmigu.cn

[J06] 计算两时间之差
来源：http://sn.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://pw.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://jb.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hn.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rk.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ji.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://zy.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://se.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://jh.colortex.cn

[J07] 比较两个日期
来源：http://br.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://zl.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mq.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dx.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yl.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gf.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ww.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ww.huanxung.cn

[J08] 提取年月日与星期
来源：http://xz.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vm.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://le.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xk.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ur.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ss.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pr.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yk.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yj.huixiangedu.cn

[J09] 时区处理
来源：http://xm.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xa.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://we.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://il.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cv.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ss.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ai.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ad.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://um.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://al.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sf.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cs.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qv.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cj.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eb.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tv.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bz.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hb.jctech888.com.cn

================================================================================
来源：http://jy.chemitech.net.cn

K. JSON 与序列化
来源：http://ot.wgjwhj.cn

================================================================================
来源：http://du.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://zs.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yh.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ku.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://sz.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://lj.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dh.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ty.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://is.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zc.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://hf.wgjwhj.cn

Py:   json.loads(s)
来源：http://wb.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tu.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://oo.lnxyls.cn

TS:   JSON.parse(s)
来源：http://nz.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pz.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://hf.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://cq.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zm.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://kn.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ej.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qw.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yj.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zj.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hc.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vu.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yz.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wq.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://rs.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ie.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uq.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ab.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hv.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cr.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gn.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yp.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ev.nicolike.cn

[K05] 深拷贝对象
来源：http://xs.521024.cn

Py:   copy.deepcopy(obj)
来源：http://bg.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://zj.nicolike.cn

JS:   structuredClone(obj)
来源：http://hx.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://vv.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xp.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pa.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://is.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://za.hahajie.cn

[K06] 解析 URL 查询串
来源：http://yr.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://td.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kz.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ee.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kv.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eo.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mo.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bg.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hb.lnxyls.cn

[K07] 进制转换
来源：http://rq.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ng.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nc.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lb.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gv.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nt.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pn.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fa.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wl.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://ux.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://fh.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lg.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://pr.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://bh.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yc.huixiangedu.cn

Go:   encoding/gob
来源：http://zm.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://bv.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cn.wgjwhj.cn

================================================================================
来源：http://oj.jianghongdianzi.cn

L. 网络请求
来源：http://iz.szxytkj.cn

================================================================================
来源：http://hj.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://xf.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zz.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://us.nicolike.cn

JS:   await fetch(url)
来源：http://to.bookmarksfly.cn

TS:   await fetch(url)
来源：http://uf.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qy.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ca.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rk.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://py.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://iz.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kr.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vz.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kg.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vf.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gh.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wj.huanxung.cn

[L03] 设置自定义请求头
来源：http://hm.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sx.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qc.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sj.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tg.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ax.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dz.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gi.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jx.huixinmuqiang.cn

[L04] 设置超时
来源：http://gu.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://aj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rf.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aq.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zs.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pw.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vv.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zz.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ga.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://qh.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xs.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://it.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pu.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aq.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ha.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://km.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ws.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dk.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://ri.muxihuayi.cn

Py:   resp.json()
来源：http://vi.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://tn.huixiangedu.cn

JS:   await resp.json()
来源：http://nc.521024.cn

TS:   await resp.json()
来源：http://ga.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xd.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dk.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://bx.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uq.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://cw.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zp.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ey.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://qm.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://nf.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://zz.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://su.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ik.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://vc.shxzukj.cn

[L08] 并发请求多个地址
来源：http://bj.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iw.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://mk.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://af.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mr.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ap.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pc.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yg.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hl.jctech888.com.cn

================================================================================
来源：http://ui.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://eb.szxytkj.cn

================================================================================
来源：http://tw.szxytkj.cn

[M01] 读取命令行参数
来源：http://vo.hahajie.cn

Py:   sys.argv[1:]
来源：http://mf.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://wc.huanxung.cn

JS:   process.argv.slice(2)
来源：http://me.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://iq.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ge.shxzukj.cn

Go:   os.Args[1:]
来源：http://sf.chemitech.net.cn

Ruby: ARGV
来源：http://aw.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://pv.bookmarksfly.cn

[M02] 读取环境变量
来源：http://yw.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ty.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vw.yuexingan06.cn

JS:   process.env.HOME
来源：http://ee.wgjwhj.cn

TS:   process.env.HOME
来源：http://eg.gzmigu.cn

Java: System.getenv("HOME")
来源：http://kk.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vr.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ma.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nk.9csxet.cn

[M03] 执行外部命令
来源：http://ay.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://na.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fg.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hw.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ug.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yh.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pl.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cu.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ua.szsharing.cn


<!-- 参考信息 -->