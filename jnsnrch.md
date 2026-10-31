代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://or.szxytkj.cn

Go:   defer f.Close()
来源：http://tq.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ur.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ap.shxzukj.cn

================================================================================
来源：http://yo.panjiajie.cn

I. 正则表达式
来源：http://ih.newstarts.cn

================================================================================
来源：http://ue.shtwfgs.cn

[I01] 判断是否匹配
来源：http://dh.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://br.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xg.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://cd.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://mz.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zp.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fu.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://mf.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bj.hnjuh.cn

[I02] 提取所有匹配
来源：http://al.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://id.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dj.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eo.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://sa.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sn.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dx.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://fs.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zd.shtwfgs.cn

[I03] 提取捕获分组
来源：http://bu.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://um.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yn.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hn.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tq.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rm.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ee.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kg.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eu.jctech888.com.cn

[I04] 正则替换
来源：http://lt.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://js.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ce.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gk.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ib.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qq.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jb.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kj.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kb.nicolike.cn

[I05] 按正则拆分
来源：http://yi.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ad.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lw.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://ar.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://tn.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://zd.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dj.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vx.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://er.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fi.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rp.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uc.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pb.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hk.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vp.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sg.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pt.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dz.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://xl.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qx.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yx.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pl.szsharing.cn

TS:   /error/gim
来源：http://nk.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nj.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gj.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://fq.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jc.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://bf.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yr.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xu.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uu.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jz.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wx.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ax.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yt.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xj.huanxung.cn

================================================================================
来源：http://ji.huixinmuqiang.cn

J. 日期与时间
来源：http://at.hahajie.cn

================================================================================
来源：http://ed.szsharing.cn

[J01] 获取当前时间
来源：http://mo.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jk.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qp.hahajie.cn

JS:   new Date();  Date.now()
来源：http://gq.huanxung.cn

TS:   new Date();  Date.now()
来源：http://rw.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://da.szsharing.cn

Go:   time.Now()
来源：http://jm.hnjuh.cn

Ruby: Time.now
来源：http://tw.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fn.haigaiapp.cn

[J02] 格式化输出
来源：http://xu.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ph.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hn.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://la.newstarts.cn

TS:   d.toISOString()
来源：http://ak.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://by.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sn.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tw.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ul.shxzskj.cn

[J03] 字符串解析为日期
来源：http://um.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yx.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://be.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://vj.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://bg.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wa.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zw.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ud.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ez.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://rs.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://od.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pg.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ek.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://we.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sl.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jc.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tz.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zl.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://zk.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://zf.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wq.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qb.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hr.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://px.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vd.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://jb.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hj.nszjky.cn

[J06] 计算两时间之差
来源：http://bz.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://ox.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://zl.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ye.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://od.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dk.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ay.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://qt.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://zm.newstarts.cn

[J07] 比较两个日期
来源：http://ub.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vn.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jz.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://np.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://so.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uf.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ir.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xf.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://zh.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://hq.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jz.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bf.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vj.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qg.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tp.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hh.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://le.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mx.hnjuh.cn

[J09] 时区处理
来源：http://nq.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ca.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zo.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gm.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eo.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vr.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wp.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jy.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ar.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wi.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rw.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nd.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ow.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ly.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cw.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fm.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cs.huixiangedu.cn

================================================================================
来源：http://xo.521024.cn

K. JSON 与序列化
来源：http://fd.colortex.cn

================================================================================
来源：http://bg.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://gj.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eu.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eq.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://gf.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://nm.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ey.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://ky.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nh.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rp.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://gk.muxihuayi.cn

Py:   json.loads(s)
来源：http://za.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bi.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://er.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://lt.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://id.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://cl.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://br.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kh.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://kl.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://st.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vl.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wj.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nl.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bg.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gx.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bt.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sg.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://jj.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qv.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oo.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yd.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wv.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cr.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hy.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hf.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ql.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://dv.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://bv.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://yh.newstarts.cn

TS:   structuredClone(obj)
来源：http://vz.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ji.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://df.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cx.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pu.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://dy.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qp.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ta.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xz.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ka.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tr.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zo.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://he.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zx.jianghongdianzi.cn

[K07] 进制转换
来源：http://ju.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://es.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fy.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ar.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ms.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qi.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ir.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ex.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cb.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://tl.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://ou.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xj.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ld.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://ml.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ti.colortex.cn

Go:   encoding/gob
来源：http://om.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://pp.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rf.shxzskj.cn

================================================================================
来源：http://ds.bjjhwx.cn

L. 网络请求
来源：http://co.wgjwhj.cn

================================================================================
来源：http://wv.lnxyls.cn

[L01] 发送 GET 请求
来源：http://zt.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xk.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rq.wgjwhj.cn

JS:   await fetch(url)
来源：http://bm.haigaiapp.cn

TS:   await fetch(url)
来源：http://ya.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lw.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://lf.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dz.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mh.9csxet.cn

[L02] 发送 POST JSON
来源：http://ny.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ih.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fg.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bb.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mx.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fd.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oh.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dp.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://qf.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yd.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gk.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kt.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gt.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://to.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ia.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ef.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iw.yuexingan06.cn

[L04] 设置超时
来源：http://pj.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://bg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://af.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gr.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uw.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hr.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bi.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bi.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xn.hahajie.cn

[L05] 上传文件（multipart）
来源：http://zu.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ua.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://au.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sz.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zc.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mq.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bt.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://we.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://se.9csxet.cn

[L06] 解析响应为 JSON
来源：http://pt.asd995.cn

Py:   resp.json()
来源：http://my.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ps.huixiangedu.cn

JS:   await resp.json()
来源：http://zg.huanxung.cn

TS:   await resp.json()
来源：http://ob.bookmarksfly.cn


<!-- 参考信息 -->