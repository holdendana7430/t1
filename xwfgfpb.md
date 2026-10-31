代发 wailian999

TS:   s.match(/\d+/g)
来源：http://sr.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://du.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://po.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cp.haigaiapp.cn

[I03] 提取捕获分组
来源：http://xx.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cd.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ks.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sb.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ei.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lp.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sq.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sp.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ly.huixinmuqiang.cn

[I04] 正则替换
来源：http://jd.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://el.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qy.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ho.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ig.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dl.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yk.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xx.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dy.gzmigu.cn

[I05] 按正则拆分
来源：http://yn.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ei.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sa.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://pp.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://dm.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://ec.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gt.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zm.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sy.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kg.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rg.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bv.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vl.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pi.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zd.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zf.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vt.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://la.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://zc.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cd.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jc.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ot.521024.cn

TS:   /error/gim
来源：http://qu.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vp.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uj.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://if.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sd.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://mq.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ur.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vw.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zx.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kg.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://er.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dx.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wj.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uk.asd995.cn

================================================================================
来源：http://ui.haigaiapp.cn

J. 日期与时间
来源：http://oy.jctech888.com.cn

================================================================================
来源：http://ax.huixiangedu.cn

[J01] 获取当前时间
来源：http://sq.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xj.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://op.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://em.colortex.cn

TS:   new Date();  Date.now()
来源：http://bl.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wz.nszjky.cn

Go:   time.Now()
来源：http://hg.hnjuh.cn

Ruby: Time.now
来源：http://xp.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wb.jianghongdianzi.cn

[J02] 格式化输出
来源：http://fm.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://po.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ak.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gq.newstarts.cn

TS:   d.toISOString()
来源：http://jx.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eh.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wh.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lg.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rk.nicolike.cn

[J03] 字符串解析为日期
来源：http://ur.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ag.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fy.asd995.cn

JS:   new Date("2024-01-02")
来源：http://ab.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ff.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rq.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://by.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://jv.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hl.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://py.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mf.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uv.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yl.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hx.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vz.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ry.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tj.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://as.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://pa.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uz.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ww.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ih.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ej.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://vj.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wv.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://my.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ei.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://xg.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uv.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hj.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bi.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://tx.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://ng.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://va.panjiajie.cn

[J07] 比较两个日期
来源：http://zt.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ov.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ev.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yw.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gq.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wb.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xj.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ap.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ga.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://jj.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hd.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pq.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wr.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rr.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ob.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jt.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ft.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hi.haigaiapp.cn

[J09] 时区处理
来源：http://rk.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xq.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cx.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://py.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fk.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ef.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dp.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nh.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nw.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://yp.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xu.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hf.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rd.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nz.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lq.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bb.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cf.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ui.521024.cn

================================================================================
来源：http://lh.colortex.cn

K. JSON 与序列化
来源：http://ex.huixinmuqiang.cn

================================================================================
来源：http://rh.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://oh.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yc.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gg.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ns.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://fv.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ns.nicolike.cn

Go:   json.Marshal(obj)
来源：http://bx.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ks.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iv.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ij.9csxet.cn

Py:   json.loads(s)
来源：http://dk.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kp.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://lv.huanxung.cn

TS:   JSON.parse(s)
来源：http://yn.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ju.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://on.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://pc.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zi.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://bv.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ko.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nj.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vu.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ew.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pc.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://or.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ek.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fq.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://bb.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vy.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bf.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zj.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://do.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hl.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ip.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://if.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pk.nszjky.cn

[K05] 深拷贝对象
来源：http://am.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://st.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://ap.lnxyls.cn

JS:   structuredClone(obj)
来源：http://gc.nszjky.cn

TS:   structuredClone(obj)
来源：http://hy.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lo.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ot.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qk.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hj.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://ad.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cy.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oa.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vj.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yh.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rs.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fq.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pg.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://in.haigaiapp.cn

[K07] 进制转换
来源：http://zo.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nw.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bj.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sa.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hm.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ew.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bq.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://he.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ph.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://bo.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://jh.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xx.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://zk.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://yh.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vs.gzmigu.cn

Go:   encoding/gob
来源：http://qq.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ko.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ap.chemitech.net.cn

================================================================================
来源：http://qi.panjiajie.cn

L. 网络请求
来源：http://fg.nicolike.cn

================================================================================
来源：http://eb.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://id.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zh.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jd.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://yh.9csxet.cn

TS:   await fetch(url)
来源：http://zr.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vx.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://fo.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nf.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xd.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://gl.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pd.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tg.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mg.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oc.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ys.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://li.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yq.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dy.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://eg.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ll.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rr.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://at.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mi.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sv.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tc.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iu.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yj.panjiajie.cn

[L04] 设置超时
来源：http://wr.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://wo.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xo.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eh.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kf.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sz.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ub.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tb.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ou.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cx.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yp.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qf.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ic.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zz.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rp.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ls.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qo.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://ly.huixiangedu.cn

Py:   resp.json()
来源：http://jc.nicolike.cn

PHP:  json_decode($body, true);
来源：http://ha.nszjky.cn

JS:   await resp.json()
来源：http://ct.jianghongdianzi.cn

TS:   await resp.json()
来源：http://zn.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pz.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ad.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://zt.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://if.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://vm.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ar.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ge.521024.cn

JS:   resp.ok;  resp.status
来源：http://fs.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ek.hahajie.cn

Java: resp.statusCode()
来源：http://ah.yuexingan06.cn

Go:   resp.StatusCode
来源：http://wd.lnxyls.cn

Ruby: resp.code.to_i
来源：http://gp.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://jr.lnxyls.cn

[L08] 并发请求多个地址
来源：http://cx.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zc.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://dc.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://py.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vp.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ad.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hs.chemitech.net.cn


<!-- 参考信息 -->