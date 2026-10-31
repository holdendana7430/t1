代发 wailian999

TS:   s.match(/\d+/g)
来源：http://re.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ii.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vg.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ol.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://it.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://fn.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tv.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dd.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ua.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xx.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://py.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xy.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dj.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jd.lnxyls.cn

[I04] 正则替换
来源：http://vi.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ak.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ag.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iw.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nz.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ch.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sl.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ft.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pc.hnjuh.cn

[I05] 按正则拆分
来源：http://fx.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nk.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hb.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://pp.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://oq.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://kg.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vy.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oj.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xs.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iv.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ej.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qm.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://im.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tz.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aa.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yd.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tw.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://rw.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fl.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://es.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dz.chemitech.net.cn

TS:   /error/gim
来源：http://yi.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://re.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mp.asd995.cn

Ruby: s.scan(/error/i)
来源：http://xj.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qa.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://iz.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wp.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bj.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kj.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vl.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zo.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lh.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yv.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.szsharing.cn

================================================================================
来源：http://iw.chemitech.net.cn

J. 日期与时间
来源：http://jl.haigaiapp.cn

================================================================================
来源：http://yv.jctech888.com.cn

[J01] 获取当前时间
来源：http://qh.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://du.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xr.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://xa.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://xi.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ut.yuexingan06.cn

Go:   time.Now()
来源：http://qa.jctech888.com.cn

Ruby: Time.now
来源：http://bs.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://av.panjiajie.cn

[J02] 格式化输出
来源：http://ci.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cn.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pe.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://im.lnxyls.cn

TS:   d.toISOString()
来源：http://fq.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ga.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ak.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ot.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://at.colortex.cn

[J03] 字符串解析为日期
来源：http://do.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vi.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ee.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://lf.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ga.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ba.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://no.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ao.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vl.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://rp.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zl.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yd.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nu.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fw.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hc.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ma.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qr.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pm.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://gg.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://tn.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rk.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vn.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ab.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xh.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://xp.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yl.muxihuayi.cn

[J06] 计算两时间之差
来源：http://ff.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://xj.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://cy.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tc.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sq.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rq.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://op.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ib.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://dw.nszjky.cn

[J07] 比较两个日期
来源：http://qt.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://oz.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kl.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xb.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bc.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bm.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cj.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://th.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://sm.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ge.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tf.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://de.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://al.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ht.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kk.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dz.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rr.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zy.521024.cn

[J09] 时区处理
来源：http://bz.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vu.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yt.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ac.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qy.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qd.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mg.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wg.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://ll.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fk.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zy.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cw.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ma.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vu.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://la.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vr.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xg.wgjwhj.cn

================================================================================
来源：http://zq.haigaiapp.cn

K. JSON 与序列化
来源：http://ds.asd995.cn

================================================================================
来源：http://xp.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://kr.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gu.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xo.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://pj.colortex.cn

TS:   JSON.stringify(obj)
来源：http://bs.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lu.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://cz.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yi.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://au.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://yp.bookmarksfly.cn

Py:   json.loads(s)
来源：http://hh.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qe.nicolike.cn

JS:   JSON.parse(s)
来源：http://nr.szxytkj.cn

TS:   JSON.parse(s)
来源：http://te.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rm.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://pc.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://dr.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jd.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://uw.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cm.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nu.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jc.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zr.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zq.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nu.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tb.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nf.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://ms.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ri.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ug.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rm.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gy.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ai.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rt.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wb.huanxung.cn

[K05] 深拷贝对象
来源：http://je.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://pk.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://bf.hnjuh.cn

JS:   structuredClone(obj)
来源：http://iy.szsharing.cn

TS:   structuredClone(obj)
来源：http://zl.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tc.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://km.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qs.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bb.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://lb.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bi.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fu.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lh.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vk.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sc.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gx.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bk.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wj.huanxung.cn

[K07] 进制转换
来源：http://yx.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ut.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hm.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dv.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://da.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gz.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sm.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ow.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tt.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://tw.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://fl.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sw.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://cc.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://om.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pi.yuntaijiaju.cn

Go:   encoding/gob
来源：http://yk.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://ac.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kn.chemitech.net.cn

================================================================================
来源：http://ib.bookmarksfly.cn

L. 网络请求
来源：http://je.521024.cn

================================================================================
来源：http://cn.9csxet.cn

[L01] 发送 GET 请求
来源：http://kh.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ke.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ap.shxzskj.cn

JS:   await fetch(url)
来源：http://la.hnjuh.cn

TS:   await fetch(url)
来源：http://bg.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qc.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://js.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zl.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gk.asd995.cn

[L02] 发送 POST JSON
来源：http://nu.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eq.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uo.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gl.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hl.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://an.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xq.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xl.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wh.panjiajie.cn

[L03] 设置自定义请求头
来源：http://la.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ol.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yt.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fl.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ak.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vt.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rf.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ij.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ma.szsharing.cn

[L04] 设置超时
来源：http://mu.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://kv.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vx.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gh.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ll.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fk.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jk.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rx.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ie.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://te.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pd.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mu.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ah.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ur.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qw.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wt.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qi.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ga.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ih.panjiajie.cn

Py:   resp.json()
来源：http://sg.nszjky.cn

PHP:  json_decode($body, true);
来源：http://dk.haigaiapp.cn

JS:   await resp.json()
来源：http://av.shxzskj.cn

TS:   await resp.json()
来源：http://dv.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xw.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ph.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://aw.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bg.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://ux.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lq.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pl.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://to.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://hw.szsharing.cn

Java: resp.statusCode()
来源：http://tl.huixiangedu.cn

Go:   resp.StatusCode
来源：http://dg.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://yf.colortex.cn

C#:   (int)resp.StatusCode
来源：http://hs.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ql.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kh.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://vw.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://am.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ig.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yh.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jt.lnxyls.cn


<!-- 参考信息 -->