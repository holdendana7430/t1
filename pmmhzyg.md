代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tg.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zz.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://xh.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bd.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://wz.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://kj.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mi.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yc.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ao.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qz.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tx.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://nz.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iu.shxzukj.cn

[I03] 提取捕获分组
来源：http://lv.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://df.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bu.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://je.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oo.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qp.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ou.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ay.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sk.hahajie.cn

[I04] 正则替换
来源：http://zn.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wq.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ue.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qb.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sp.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nz.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ys.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rz.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://om.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://qx.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nm.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vh.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://me.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://zt.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://cx.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hx.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mo.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kw.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fq.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ay.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mb.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ep.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://za.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://de.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xl.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dv.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://km.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gd.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qo.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ld.colortex.cn

TS:   /error/gim
来源：http://xp.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fa.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qd.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://wc.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ro.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://nr.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fm.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://id.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vt.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yx.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ym.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ky.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xi.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pc.huixiangedu.cn

================================================================================
来源：http://gh.szsharing.cn

J. 日期与时间
来源：http://ia.bookmarksfly.cn

================================================================================
来源：http://uj.muxihuayi.cn

[J01] 获取当前时间
来源：http://jf.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gm.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sb.9csxet.cn

JS:   new Date();  Date.now()
来源：http://wp.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://ty.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://br.shtwfgs.cn

Go:   time.Now()
来源：http://wz.shtwfgs.cn

Ruby: Time.now
来源：http://xm.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://an.nicolike.cn

[J02] 格式化输出
来源：http://kp.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tq.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sr.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pd.hahajie.cn

TS:   d.toISOString()
来源：http://od.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rr.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hd.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ck.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lq.521024.cn

[J03] 字符串解析为日期
来源：http://mg.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://da.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uk.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://zf.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://zi.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://im.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mw.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://gy.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sz.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ch.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kc.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dj.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jo.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hj.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://db.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rn.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kj.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qb.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://qw.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://or.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jv.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qu.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ig.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fe.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pf.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://bo.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xj.huixiangedu.cn

[J06] 计算两时间之差
来源：http://sl.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://pk.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://wc.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://es.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wm.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lk.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://da.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://go.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://sa.szxytkj.cn

[J07] 比较两个日期
来源：http://mg.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ki.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bx.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jv.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ma.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://io.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ew.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jz.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://sa.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://il.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ux.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kr.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ix.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fl.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://un.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cu.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kx.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uy.huanxung.cn

[J09] 时区处理
来源：http://kr.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ci.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://og.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xq.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yb.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ye.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sj.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ln.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nc.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ri.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cx.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dt.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ay.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vz.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nh.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pe.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://av.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zc.nicolike.cn

================================================================================
来源：http://lm.asd995.cn

K. JSON 与序列化
来源：http://ro.huanxung.cn

================================================================================
来源：http://oo.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://de.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fg.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ln.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://vx.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://au.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qu.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://zh.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gu.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fa.nicolike.cn

[K02] JSON 字符串转对象
来源：http://zd.521024.cn

Py:   json.loads(s)
来源：http://bk.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yd.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://dy.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://mf.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qe.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://vh.asd995.cn

Ruby: JSON.parse(s)
来源：http://oc.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bs.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://lu.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fi.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pf.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://av.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ng.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lq.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ol.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bs.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tu.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://rt.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rm.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tg.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iz.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ml.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tb.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zg.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dy.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ir.muxihuayi.cn

[K05] 深拷贝对象
来源：http://xx.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://en.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ir.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ff.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://lu.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bk.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bc.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://by.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kt.colortex.cn

[K06] 解析 URL 查询串
来源：http://ns.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gj.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uz.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qf.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ff.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dw.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lf.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://co.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gs.bookmarksfly.cn

[K07] 进制转换
来源：http://kz.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jb.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gf.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://km.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bi.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pv.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xt.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://os.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oj.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ep.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://fw.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wu.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://sp.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ye.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uo.jianghongdianzi.cn

Go:   encoding/gob
来源：http://by.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ha.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rc.asd995.cn

================================================================================
来源：http://fc.shxzukj.cn

L. 网络请求
来源：http://kd.yuntaijiaju.cn

================================================================================
来源：http://lx.hahajie.cn

[L01] 发送 GET 请求
来源：http://tb.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dq.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kj.huanxung.cn

JS:   await fetch(url)
来源：http://dc.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://md.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bm.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://qk.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nh.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kd.shxzskj.cn

[L02] 发送 POST JSON
来源：http://nv.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ce.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mw.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qr.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lj.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gt.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hv.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ns.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cn.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://er.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ms.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lp.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://os.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wj.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cs.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://or.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ir.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qe.gzmigu.cn

[L04] 设置超时
来源：http://vf.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ek.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pl.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mg.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fz.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sc.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://st.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mz.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://dt.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ch.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mp.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bq.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cm.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dx.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nk.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bd.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ul.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://cl.gzmigu.cn

Py:   resp.json()
来源：http://xr.521024.cn

PHP:  json_decode($body, true);
来源：http://pr.szxytkj.cn

JS:   await resp.json()
来源：http://kj.huanxung.cn

TS:   await resp.json()
来源：http://fu.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uq.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ne.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://il.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ai.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://rv.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xo.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://js.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ky.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://xj.gzmigu.cn

Java: resp.statusCode()
来源：http://hm.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://ms.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://do.521024.cn


<!-- 参考信息 -->