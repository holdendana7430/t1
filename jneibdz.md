代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wk.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ds.bjjhwx.cn

[I04] 正则替换
来源：http://ry.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rv.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qa.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yj.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lc.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sa.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://es.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gi.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zg.haigaiapp.cn

[I05] 按正则拆分
来源：http://th.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qe.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vq.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://zy.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ke.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://ul.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gz.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ao.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sy.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lg.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://in.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dc.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fs.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ga.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dg.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gn.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sv.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lf.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ce.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uv.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yl.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rd.hahajie.cn

TS:   /error/gim
来源：http://gy.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://le.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mr.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://pu.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xc.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://bz.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vx.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ps.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rx.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ht.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nc.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://im.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vo.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://as.shtwfgs.cn

================================================================================
来源：http://ii.shtwfgs.cn

J. 日期与时间
来源：http://mo.jianghongdianzi.cn

================================================================================
来源：http://bq.szsharing.cn

[J01] 获取当前时间
来源：http://mv.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fb.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hj.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://bd.hahajie.cn

TS:   new Date();  Date.now()
来源：http://bu.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ts.shtwfgs.cn

Go:   time.Now()
来源：http://ic.nszjky.cn

Ruby: Time.now
来源：http://tg.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bq.huanxung.cn

[J02] 格式化输出
来源：http://dk.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bq.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jg.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ic.shtwfgs.cn

TS:   d.toISOString()
来源：http://gg.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ry.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oj.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ru.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ad.shxzskj.cn

[J03] 字符串解析为日期
来源：http://ct.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ch.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dl.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://wp.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://au.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lt.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gw.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://bq.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mp.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://cd.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://az.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yz.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://va.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ph.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ku.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wh.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sa.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rw.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://gp.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://bv.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tp.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://so.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://cw.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mj.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://lr.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tj.haigaiapp.cn

[J06] 计算两时间之差
来源：http://nx.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://dx.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://bi.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yj.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fg.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://th.521024.cn

Go:   end.Sub(start).Hours()
来源：http://hb.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://zy.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ox.huixiangedu.cn

[J07] 比较两个日期
来源：http://ma.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://qy.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kn.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xm.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mp.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qo.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zq.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hi.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://xr.521024.cn

[J08] 提取年月日与星期
来源：http://vr.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ia.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hm.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ad.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ye.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ga.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ry.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xb.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pq.nszjky.cn

[J09] 时区处理
来源：http://yj.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kc.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qf.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zd.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tr.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mp.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ov.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pj.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jb.521024.cn

[J10] 取今天 / 本月第一天
来源：http://gk.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lk.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ke.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tc.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kp.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tq.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rv.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cp.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wj.lnxyls.cn

================================================================================
来源：http://ye.gzmigu.cn

K. JSON 与序列化
来源：http://zc.bjjhwx.cn

================================================================================
来源：http://xj.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://wz.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yx.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pk.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://tc.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://rg.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yr.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://wf.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uk.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ax.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://lc.gzmigu.cn

Py:   json.loads(s)
来源：http://xy.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gi.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ra.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://hp.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ho.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ii.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://ji.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ir.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://db.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dt.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qi.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kl.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fk.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fc.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nc.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ds.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qu.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://vd.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://an.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yy.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zk.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jq.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qr.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ay.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ro.jctech888.com.cn

[K05] 深拷贝对象
来源：http://hh.521024.cn

Py:   copy.deepcopy(obj)
来源：http://jl.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://nx.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ce.huanxung.cn

TS:   structuredClone(obj)
来源：http://cs.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yi.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ha.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://im.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gu.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://rd.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qv.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rv.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wc.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mn.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rv.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://by.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jw.asd995.cn

[K07] 进制转换
来源：http://yo.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ar.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ki.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nu.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dt.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fe.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hx.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yo.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nn.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ct.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://ob.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gr.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ff.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://sl.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mq.wgjwhj.cn

Go:   encoding/gob
来源：http://qf.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://bl.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vo.shxzukj.cn

================================================================================
来源：http://fg.bookmarksfly.cn

L. 网络请求
来源：http://iq.huixinmuqiang.cn

================================================================================
来源：http://rg.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://on.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://db.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pu.shxzukj.cn

JS:   await fetch(url)
来源：http://lv.bjjhwx.cn

TS:   await fetch(url)
来源：http://qf.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nu.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://mv.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yd.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lb.szsharing.cn

[L02] 发送 POST JSON
来源：http://nf.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ty.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cv.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cc.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yv.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mu.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yc.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://au.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ft.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://uw.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pd.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://am.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mn.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ib.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dl.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ty.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rb.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rd.haigaiapp.cn

[L04] 设置超时
来源：http://vc.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://eg.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zk.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oe.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ut.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://le.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fu.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bz.9csxet.cn

[L05] 上传文件（multipart）
来源：http://bd.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jn.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dt.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kf.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kf.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://du.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cr.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rd.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fd.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ry.chemitech.net.cn

Py:   resp.json()
来源：http://on.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ai.hahajie.cn

JS:   await resp.json()
来源：http://bn.521024.cn

TS:   await resp.json()
来源：http://sj.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wr.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yl.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://qk.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ys.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://zr.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sq.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lh.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://oz.asd995.cn

TS:   resp.ok;  resp.status
来源：http://dl.521024.cn

Java: resp.statusCode()
来源：http://rx.newstarts.cn

Go:   resp.StatusCode
来源：http://oa.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://wy.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://vm.szsharing.cn

[L08] 并发请求多个地址
来源：http://ym.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gg.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://wm.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xm.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://to.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ai.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vr.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ov.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pu.hnjuh.cn

================================================================================
来源：http://cv.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://xj.chemitech.net.cn

================================================================================
来源：http://vw.muxihuayi.cn

[M01] 读取命令行参数
来源：http://oe.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://hr.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://vu.asd995.cn

JS:   process.argv.slice(2)
来源：http://qo.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://zp.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://ze.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://yw.newstarts.cn


<!-- 参考信息 -->