代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jw.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yx.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://ay.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://cd.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qr.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xn.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ds.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zg.bjjhwx.cn

[I02] 提取所有匹配
来源：http://ul.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://mh.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uq.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bc.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://sv.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ae.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zl.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://ou.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ra.chemitech.net.cn

[I03] 提取捕获分组
来源：http://jm.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cx.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ys.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ta.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://er.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://su.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://su.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cl.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bh.jianghongdianzi.cn

[I04] 正则替换
来源：http://nw.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bm.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kc.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eh.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ha.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://by.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sy.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zq.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vo.shxzukj.cn

[I05] 按正则拆分
来源：http://yh.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dc.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qq.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ab.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://rd.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://tu.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://up.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wk.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eb.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sk.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ah.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ac.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://io.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wo.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jx.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fp.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ba.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cu.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://kk.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sh.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cj.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ed.chemitech.net.cn

TS:   /error/gim
来源：http://sh.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lg.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jj.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://gz.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bj.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://kg.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bu.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hn.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ny.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ao.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ga.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cr.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mx.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qz.nszjky.cn

================================================================================
来源：http://uk.nicolike.cn

J. 日期与时间
来源：http://mi.newstarts.cn

================================================================================
来源：http://pm.szsharing.cn

[J01] 获取当前时间
来源：http://xv.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pq.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zw.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://em.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://wy.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qb.yuexingan06.cn

Go:   time.Now()
来源：http://eo.shtwfgs.cn

Ruby: Time.now
来源：http://qs.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ot.asd995.cn

[J02] 格式化输出
来源：http://er.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vp.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jk.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tq.chemitech.net.cn

TS:   d.toISOString()
来源：http://wt.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://av.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pf.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lp.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xw.newstarts.cn

[J03] 字符串解析为日期
来源：http://ff.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qj.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uu.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://sb.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ek.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bn.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vk.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ss.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jt.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://lh.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eg.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xu.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vb.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bz.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nc.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ug.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zo.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://dz.asd995.cn

Py:   now + timedelta(days=7)
来源：http://pd.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dz.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://na.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qa.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://nx.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ge.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://uc.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tc.shxzukj.cn

[J06] 计算两时间之差
来源：http://dv.asd995.cn

Py:   (end - start).total_seconds()
来源：http://am.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://hb.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fg.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vl.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xs.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://ka.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://cb.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://hb.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://lq.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ts.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ye.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ph.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fy.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ww.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fb.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qr.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://dk.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://yi.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oi.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tm.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yd.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pn.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pq.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qb.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cv.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lz.nszjky.cn

[J09] 时区处理
来源：http://ea.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yv.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xq.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hd.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://my.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fc.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hu.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://un.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lz.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://kf.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://io.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iv.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yy.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sc.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sb.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rq.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hd.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yg.bjjhwx.cn

================================================================================
来源：http://fo.huanxung.cn

K. JSON 与序列化
来源：http://pa.9csxet.cn

================================================================================
来源：http://qi.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://eo.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pj.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nu.colortex.cn

JS:   JSON.stringify(obj)
来源：http://bf.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://ig.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://td.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://wg.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vh.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vu.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://ad.jctech888.com.cn

Py:   json.loads(s)
来源：http://wh.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jd.newstarts.cn

JS:   JSON.parse(s)
来源：http://gv.asd995.cn

TS:   JSON.parse(s)
来源：http://dq.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vn.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://kj.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://go.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://go.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://xz.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cv.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bd.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qm.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://my.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hf.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cq.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ll.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sm.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://kh.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wt.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iy.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://re.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hy.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dl.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wu.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eg.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://if.newstarts.cn

[K05] 深拷贝对象
来源：http://ta.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://so.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://iz.panjiajie.cn

JS:   structuredClone(obj)
来源：http://js.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://qd.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vj.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dv.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bc.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tl.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://bf.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vv.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xe.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hk.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sn.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sl.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gt.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xq.yuntaijiaju.cn

[K07] 进制转换
来源：http://yn.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://io.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bh.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oi.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uf.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yi.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ml.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xt.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nw.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://na.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://qn.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zp.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://cl.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://fe.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cu.muxihuayi.cn

Go:   encoding/gob
来源：http://vj.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://eu.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fx.huixinmuqiang.cn

================================================================================
来源：http://ti.wgjwhj.cn

L. 网络请求
来源：http://az.szxytkj.cn

================================================================================
来源：http://ap.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://xw.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://br.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hc.hnjuh.cn

JS:   await fetch(url)
来源：http://yv.szxytkj.cn

TS:   await fetch(url)
来源：http://cg.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zd.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://uq.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tq.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hd.nicolike.cn

[L02] 发送 POST JSON
来源：http://pr.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://op.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://at.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ms.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vn.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ff.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ld.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ml.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vf.szxytkj.cn

[L03] 设置自定义请求头
来源：http://sb.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sx.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wl.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xu.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pi.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nz.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://he.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ec.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://th.chemitech.net.cn

[L04] 设置超时
来源：http://cq.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://nq.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fz.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dd.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dg.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jm.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eg.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wq.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bg.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ll.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dn.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kx.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ib.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kk.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pm.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tg.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ks.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ki.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://gs.yuntaijiaju.cn

Py:   resp.json()
来源：http://bh.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ue.shxzukj.cn

JS:   await resp.json()
来源：http://ft.lnxyls.cn

TS:   await resp.json()
来源：http://uh.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qg.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://em.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ex.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ep.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://nu.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ba.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bk.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ay.lnxyls.cn


<!-- 参考信息 -->