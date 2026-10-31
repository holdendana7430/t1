代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ye.nszjky.cn

Go:   defer f.Close()
来源：http://fp.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rs.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eq.huanxung.cn

================================================================================
来源：http://wv.gzmigu.cn

I. 正则表达式
来源：http://av.gzmigu.cn

================================================================================
来源：http://gc.hnjuh.cn

[I01] 判断是否匹配
来源：http://jr.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jz.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yt.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ws.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://nd.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hp.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eo.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://pt.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fu.wgjwhj.cn

[I02] 提取所有匹配
来源：http://or.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://km.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vb.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ti.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://rt.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dg.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oj.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://ld.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://il.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://pf.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bd.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uz.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ae.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jh.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jl.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bw.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oz.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rt.newstarts.cn

[I04] 正则替换
来源：http://ea.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jj.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ki.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sm.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wq.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vx.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ra.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jl.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gw.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://ts.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kh.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yr.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://fe.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ei.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://ir.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mj.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zh.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kw.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ol.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bk.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sz.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vj.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ny.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kl.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ph.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qo.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dt.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://yo.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nv.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fh.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vu.nszjky.cn

TS:   /error/gim
来源：http://kw.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xz.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zh.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://cx.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lg.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://jm.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://an.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dn.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zl.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wq.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kq.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jg.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bv.huixinmuqiang.cn

================================================================================
来源：http://oc.521024.cn

J. 日期与时间
来源：http://cf.colortex.cn

================================================================================
来源：http://oj.muxihuayi.cn

[J01] 获取当前时间
来源：http://ct.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wk.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wy.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://yl.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://lm.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mh.szxytkj.cn

Go:   time.Now()
来源：http://qn.hahajie.cn

Ruby: Time.now
来源：http://se.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cp.jianghongdianzi.cn

[J02] 格式化输出
来源：http://ip.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pj.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sm.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qs.szsharing.cn

TS:   d.toISOString()
来源：http://rt.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ao.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://np.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cl.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tq.hahajie.cn

[J03] 字符串解析为日期
来源：http://vq.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lk.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uh.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://hg.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://yg.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zn.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gc.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://mx.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jx.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://ne.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iu.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dp.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qu.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cm.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qf.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xc.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pe.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oh.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://sj.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://xs.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nz.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ui.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zx.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://gr.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qi.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://bu.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gf.newstarts.cn

[J06] 计算两时间之差
来源：http://ja.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://wf.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://rd.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xn.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iz.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ix.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://fa.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://sc.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://iz.bookmarksfly.cn

[J07] 比较两个日期
来源：http://fp.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://em.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fg.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yd.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://it.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vk.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ry.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ks.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://at.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fi.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yk.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fy.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lx.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qf.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zr.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qb.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xv.colortex.cn

[J09] 时区处理
来源：http://fe.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ra.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mh.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cf.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pt.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cj.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mc.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gb.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://ij.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rz.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tb.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yj.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lp.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jm.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eq.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rv.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zi.hnjuh.cn

================================================================================
来源：http://pc.jianghongdianzi.cn

K. JSON 与序列化
来源：http://oa.huixiangedu.cn

================================================================================
来源：http://rk.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://gq.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eg.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nl.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://mg.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://fh.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.newstarts.cn

Go:   json.Marshal(obj)
来源：http://aw.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ra.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oy.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://xv.szsharing.cn

Py:   json.loads(s)
来源：http://fy.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vh.hnjuh.cn

JS:   JSON.parse(s)
来源：http://xm.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://qo.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xx.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://vk.huanxung.cn

Ruby: JSON.parse(s)
来源：http://gx.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://od.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://oi.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zc.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qw.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jh.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sr.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bq.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lw.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ac.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ii.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://pk.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zu.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wa.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cv.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ey.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kz.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ee.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://co.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hd.huanxung.cn

[K05] 深拷贝对象
来源：http://lu.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://lg.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://le.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://wm.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://xm.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ur.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zp.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ev.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tg.colortex.cn

[K06] 解析 URL 查询串
来源：http://au.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pb.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jp.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ob.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ox.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vt.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xn.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ay.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qb.nicolike.cn

[K07] 进制转换
来源：http://nc.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mp.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fx.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uz.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zg.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qv.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ap.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://be.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mk.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://zl.colortex.cn

Py:   pickle.dumps(obj)
来源：http://vk.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hd.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fb.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://gr.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dx.bjjhwx.cn

Go:   encoding/gob
来源：http://ep.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://rt.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dp.nicolike.cn

================================================================================
来源：http://cw.bjjhwx.cn

L. 网络请求
来源：http://qp.shxzukj.cn

================================================================================
来源：http://el.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://hw.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oi.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ey.hnjuh.cn

JS:   await fetch(url)
来源：http://li.szxytkj.cn

TS:   await fetch(url)
来源：http://wn.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kb.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://am.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://he.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cu.shxzukj.cn

[L02] 发送 POST JSON
来源：http://uy.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tv.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jj.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vr.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rg.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fa.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lw.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ae.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tu.gzmigu.cn

[L03] 设置自定义请求头
来源：http://um.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lb.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://op.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://by.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ai.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ki.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gj.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qs.colortex.cn

[L04] 设置超时
来源：http://md.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://pt.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rg.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tl.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hp.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pz.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ts.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tx.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ri.szsharing.cn

[L05] 上传文件（multipart）
来源：http://sh.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zr.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kx.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xp.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sv.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ox.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bf.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gx.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zv.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://nr.hahajie.cn

Py:   resp.json()
来源：http://ra.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://jw.haigaiapp.cn

JS:   await resp.json()
来源：http://an.huixiangedu.cn

TS:   await resp.json()
来源：http://xo.shtwfgs.cn


<!-- 参考信息 -->