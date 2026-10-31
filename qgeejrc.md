代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://ho.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jf.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mi.gzmigu.cn

[I05] 按正则拆分
来源：http://jo.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qn.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aq.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://qc.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://eb.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://mu.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mx.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tn.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sv.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uj.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lt.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yi.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://li.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ic.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ff.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lw.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://er.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rm.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://xj.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cx.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yw.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gx.asd995.cn

TS:   /error/gim
来源：http://fx.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://et.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jh.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://ch.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sq.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://hm.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ii.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uh.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pn.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ws.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tf.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wu.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rf.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ex.muxihuayi.cn

================================================================================
来源：http://tw.panjiajie.cn

J. 日期与时间
来源：http://ip.colortex.cn

================================================================================
来源：http://ja.wgjwhj.cn

[J01] 获取当前时间
来源：http://gi.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://he.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sb.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://jy.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://mg.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ik.newstarts.cn

Go:   time.Now()
来源：http://kf.muxihuayi.cn

Ruby: Time.now
来源：http://cy.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ah.newstarts.cn

[J02] 格式化输出
来源：http://hm.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yc.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tp.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gp.jctech888.com.cn

TS:   d.toISOString()
来源：http://or.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://it.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zg.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lr.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dj.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://gc.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zz.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qq.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://zp.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://bq.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bf.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bl.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://xw.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wc.nszjky.cn

[J04] 时间戳与日期互转
来源：http://xa.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iq.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ke.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iy.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nd.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://as.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lp.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qr.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kc.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ax.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://cq.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eb.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fw.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uy.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://tg.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hx.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://mt.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://li.hahajie.cn

[J06] 计算两时间之差
来源：http://dj.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://tn.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://kf.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dv.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://js.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://he.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://kd.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://aw.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://iv.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://mw.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ex.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pk.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pu.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gc.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rm.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ss.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qt.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://zn.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://br.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gw.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ov.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sn.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aj.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://li.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rn.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rj.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ds.hnjuh.cn

[J09] 时区处理
来源：http://re.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sk.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pi.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cl.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yx.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sv.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ze.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ae.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ny.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://fr.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ev.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cy.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ub.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bo.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lg.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eb.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wi.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jb.haigaiapp.cn

================================================================================
来源：http://zk.521024.cn

K. JSON 与序列化
来源：http://iz.asd995.cn

================================================================================
来源：http://jj.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://il.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iw.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ny.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://dj.colortex.cn

TS:   JSON.stringify(obj)
来源：http://kg.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zd.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://vr.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yb.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oa.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://zg.bookmarksfly.cn

Py:   json.loads(s)
来源：http://vz.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gs.lnxyls.cn

JS:   JSON.parse(s)
来源：http://qk.nicolike.cn

TS:   JSON.parse(s)
来源：http://yg.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nw.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://qi.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://gu.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bk.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://fz.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qr.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zn.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ig.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://em.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yd.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://im.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eu.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tp.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://uv.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yd.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fl.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ri.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ie.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cf.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dc.gzmigu.cn

[K05] 深拷贝对象
来源：http://ao.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://um.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://dh.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://xp.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://ug.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ks.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zv.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://da.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://to.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://xn.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eg.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wp.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fd.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kl.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ts.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zb.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zz.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ah.haigaiapp.cn

[K07] 进制转换
来源：http://hp.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tw.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wt.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zu.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ay.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://je.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gt.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vt.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zz.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://cu.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://vo.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://se.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mq.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://da.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rt.jianghongdianzi.cn

Go:   encoding/gob
来源：http://pf.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://yx.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uf.huanxung.cn

================================================================================
来源：http://af.szsharing.cn

L. 网络请求
来源：http://jy.bjjhwx.cn

================================================================================
来源：http://tx.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://hb.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ts.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://up.shxzukj.cn

JS:   await fetch(url)
来源：http://ah.colortex.cn

TS:   await fetch(url)
来源：http://lh.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jp.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://tk.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dx.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gt.gzmigu.cn

[L02] 发送 POST JSON
来源：http://qk.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bf.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lp.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uy.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fl.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ay.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bw.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bi.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cq.521024.cn

[L03] 设置自定义请求头
来源：http://dc.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zv.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qm.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bn.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cv.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kw.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bh.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hd.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fw.huanxung.cn

[L04] 设置超时
来源：http://yv.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://ms.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ws.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nx.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zp.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rl.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ck.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://um.asd995.cn

[L05] 上传文件（multipart）
来源：http://tc.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lp.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eh.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qx.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cp.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gi.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vs.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ws.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tc.colortex.cn

[L06] 解析响应为 JSON
来源：http://wq.huanxung.cn

Py:   resp.json()
来源：http://tt.colortex.cn

PHP:  json_decode($body, true);
来源：http://ix.shtwfgs.cn

JS:   await resp.json()
来源：http://zu.chemitech.net.cn

TS:   await resp.json()
来源：http://ir.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rh.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jp.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://vb.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hj.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://bx.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cn.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zq.521024.cn

JS:   resp.ok;  resp.status
来源：http://iv.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://vf.gzmigu.cn

Java: resp.statusCode()
来源：http://qh.lnxyls.cn

Go:   resp.StatusCode
来源：http://ty.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://mk.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://ry.9csxet.cn

[L08] 并发请求多个地址
来源：http://vo.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xf.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://pe.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gn.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rf.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yw.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ai.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yn.bjjhwx.cn

================================================================================
来源：http://gc.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://tt.haigaiapp.cn

================================================================================
来源：http://jk.colortex.cn

[M01] 读取命令行参数
来源：http://tn.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://tm.nicolike.cn

PHP:  $argv;  $argc;
来源：http://em.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ok.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://zt.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://mq.gzmigu.cn

Go:   os.Args[1:]
来源：http://ws.huanxung.cn

Ruby: ARGV
来源：http://ir.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://st.newstarts.cn

[M02] 读取环境变量
来源：http://tk.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://rf.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wx.shxzukj.cn

JS:   process.env.HOME
来源：http://zy.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://iu.shxzskj.cn

Java: System.getenv("HOME")
来源：http://iv.yuexingan06.cn


<!-- 参考信息 -->