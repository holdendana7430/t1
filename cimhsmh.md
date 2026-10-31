代发 wailian999

================================================================================
来源：http://db.huixinmuqiang.cn

I. 正则表达式
来源：http://ut.huixinmuqiang.cn

================================================================================
来源：http://gf.szxytkj.cn

[I01] 判断是否匹配
来源：http://un.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ap.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zy.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://kf.521024.cn

TS:   /\d+/.test(s)
来源：http://ir.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sz.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jn.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://rs.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nn.nicolike.cn

[I02] 提取所有匹配
来源：http://pv.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://mt.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ak.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zk.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://le.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ch.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://li.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://il.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lc.panjiajie.cn

[I03] 提取捕获分组
来源：http://zr.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sp.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vo.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ay.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gg.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gm.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vc.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yy.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ye.haigaiapp.cn

[I04] 正则替换
来源：http://ll.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kt.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vx.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xn.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mj.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bf.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vy.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cg.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lz.nicolike.cn

[I05] 按正则拆分
来源：http://jx.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ky.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xu.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://bk.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://yv.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://dm.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wn.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ij.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cv.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://we.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ed.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zg.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ez.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://as.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rj.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fv.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bh.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://xv.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dq.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yk.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ta.hahajie.cn

TS:   /error/gim
来源：http://nb.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ap.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://px.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://mf.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pg.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://xl.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vp.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bp.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xp.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lt.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fa.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ii.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jy.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lw.chemitech.net.cn

================================================================================
来源：http://wl.huanxung.cn

J. 日期与时间
来源：http://nd.huixiangedu.cn

================================================================================
来源：http://ga.wgjwhj.cn

[J01] 获取当前时间
来源：http://ct.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dj.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fx.hahajie.cn

JS:   new Date();  Date.now()
来源：http://bc.nicolike.cn

TS:   new Date();  Date.now()
来源：http://mf.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dw.panjiajie.cn

Go:   time.Now()
来源：http://gi.yuexingan06.cn

Ruby: Time.now
来源：http://me.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sy.hnjuh.cn

[J02] 格式化输出
来源：http://ks.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cq.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gf.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ee.shxzukj.cn

TS:   d.toISOString()
来源：http://gt.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vu.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ik.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ya.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pq.521024.cn

[J03] 字符串解析为日期
来源：http://yc.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://di.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dl.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://hz.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ep.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hs.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ss.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://hn.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lr.9csxet.cn

[J04] 时间戳与日期互转
来源：http://cp.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dk.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rf.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gg.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://re.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qi.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ae.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qe.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ey.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://mu.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://dw.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://en.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://op.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wp.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://kd.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://em.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://ir.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oj.gzmigu.cn

[J06] 计算两时间之差
来源：http://zn.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://dn.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://jz.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xa.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://go.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hy.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://cq.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://fd.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://tx.szxytkj.cn

[J07] 比较两个日期
来源：http://wl.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ht.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mg.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dw.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mh.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rf.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vp.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hm.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://wx.9csxet.cn

[J08] 提取年月日与星期
来源：http://rn.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://za.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kr.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ag.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yt.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lr.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pf.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://je.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iu.yuntaijiaju.cn

[J09] 时区处理
来源：http://fc.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fy.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oj.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rg.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vs.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ls.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://si.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sz.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://se.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://fq.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xj.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ov.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yo.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ag.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://le.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sc.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://js.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uh.jianghongdianzi.cn

================================================================================
来源：http://hw.szxytkj.cn

K. JSON 与序列化
来源：http://po.yuexingan06.cn

================================================================================
来源：http://hw.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://ks.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yj.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ig.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://vt.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://ks.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qy.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://dw.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nw.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://el.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://rj.nszjky.cn

Py:   json.loads(s)
来源：http://jl.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vh.szxytkj.cn

JS:   JSON.parse(s)
来源：http://sl.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://uq.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ee.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://pw.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://yw.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://es.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zb.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yh.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oc.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hi.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sy.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bq.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pu.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vt.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://co.szsharing.cn

[K04] 读取 JSON 文件
来源：http://cp.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dq.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fe.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jw.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ku.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eg.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fh.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://da.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vx.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://pp.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://cl.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://gk.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ok.shxzukj.cn

TS:   structuredClone(obj)
来源：http://cw.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ka.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qa.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lo.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://av.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://kc.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eh.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bh.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vn.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gr.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qz.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ct.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nw.jctech888.com.cn

[K07] 进制转换
来源：http://kj.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yc.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tz.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://el.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rf.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iw.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yx.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ka.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ds.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://hi.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://yl.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nd.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mr.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://xs.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xv.gzmigu.cn

Go:   encoding/gob
来源：http://bq.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://qp.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zc.bjjhwx.cn

================================================================================
来源：http://vi.nicolike.cn

L. 网络请求
来源：http://ii.bookmarksfly.cn

================================================================================
来源：http://mq.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ig.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://du.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://al.muxihuayi.cn

JS:   await fetch(url)
来源：http://pd.muxihuayi.cn

TS:   await fetch(url)
来源：http://uu.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uz.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://zb.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bi.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lw.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ej.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yk.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wc.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cy.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ai.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oj.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bb.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tz.shxzskj.cn

[L03] 设置自定义请求头
来源：http://hs.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oj.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tl.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dt.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dh.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vi.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kn.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gz.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bc.newstarts.cn

[L04] 设置超时
来源：http://td.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://cn.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pn.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fe.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ux.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mt.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zu.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nh.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://no.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nk.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://we.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lq.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xd.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ji.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xi.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mx.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nk.colortex.cn

[L06] 解析响应为 JSON
来源：http://ny.bjjhwx.cn

Py:   resp.json()
来源：http://ma.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://tf.huixiangedu.cn

JS:   await resp.json()
来源：http://aq.nicolike.cn

TS:   await resp.json()
来源：http://pt.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ua.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ri.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://fi.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hq.shxzskj.cn


<!-- 参考信息 -->