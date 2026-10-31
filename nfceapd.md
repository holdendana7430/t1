代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zl.panjiajie.cn

Go:   defer f.Close()
来源：http://er.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://th.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sp.yuntaijiaju.cn

================================================================================
来源：http://mg.shxzukj.cn

I. 正则表达式
来源：http://cb.lnxyls.cn

================================================================================
来源：http://ap.shxzukj.cn

[I01] 判断是否匹配
来源：http://aq.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gs.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ms.hahajie.cn

JS:   /\d+/.test(s)
来源：http://nx.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://nj.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://av.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yz.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://nb.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qi.wgjwhj.cn

[I02] 提取所有匹配
来源：http://va.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://fr.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ke.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lz.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://hm.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rs.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pk.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://vb.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zy.huanxung.cn

[I03] 提取捕获分组
来源：http://vv.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vh.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nj.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://go.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://au.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jy.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qw.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://en.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ii.gzmigu.cn

[I04] 正则替换
来源：http://hd.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gb.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hg.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nb.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://on.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rj.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oh.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ca.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ba.muxihuayi.cn

[I05] 按正则拆分
来源：http://mi.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://op.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ao.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ua.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://re.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://bm.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ql.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xp.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mv.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vb.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ee.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bc.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fg.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lc.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xa.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://km.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://gy.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kj.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://og.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gy.newstarts.cn

TS:   /error/gim
来源：http://gy.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xb.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bw.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://yk.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nm.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://ut.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ur.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hj.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uh.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hr.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fr.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://md.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mw.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fh.hahajie.cn

================================================================================
来源：http://qx.jianghongdianzi.cn

J. 日期与时间
来源：http://sh.wgjwhj.cn

================================================================================
来源：http://do.chemitech.net.cn

[J01] 获取当前时间
来源：http://wm.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mm.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aj.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://xm.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://fo.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ls.szsharing.cn

Go:   time.Now()
来源：http://ly.shxzskj.cn

Ruby: Time.now
来源：http://lt.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sk.jianghongdianzi.cn

[J02] 格式化输出
来源：http://wd.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ni.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qn.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iz.szxytkj.cn

TS:   d.toISOString()
来源：http://rn.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ag.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rt.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xk.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zm.nszjky.cn

[J03] 字符串解析为日期
来源：http://vz.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://by.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yl.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://yv.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ts.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ss.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sf.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://fa.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ng.9csxet.cn

[J04] 时间戳与日期互转
来源：http://lf.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uy.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fd.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jl.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oj.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://by.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zs.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pi.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://av.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ca.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://bv.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wh.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rq.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dm.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://yx.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://qj.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sh.muxihuayi.cn

[J06] 计算两时间之差
来源：http://eh.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://pv.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://fm.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nk.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wd.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ul.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://xp.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://ic.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://gx.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://fu.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://zs.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qj.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hk.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://in.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ze.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cr.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ti.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://jx.hahajie.cn

[J08] 提取年月日与星期
来源：http://rr.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fn.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hh.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jj.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ar.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qn.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wt.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qe.newstarts.cn

[J09] 时区处理
来源：http://dd.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gj.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dr.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uh.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ee.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ll.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ej.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://na.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jo.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://cv.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sa.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ub.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wn.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tw.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hn.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wn.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vg.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://of.bjjhwx.cn

================================================================================
来源：http://uh.asd995.cn

K. JSON 与序列化
来源：http://zu.9csxet.cn

================================================================================
来源：http://mn.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://lj.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ef.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wl.521024.cn

JS:   JSON.stringify(obj)
来源：http://ue.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://kr.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pe.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ov.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vt.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dv.colortex.cn

[K02] JSON 字符串转对象
来源：http://fy.shxzukj.cn

Py:   json.loads(s)
来源：http://wj.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pw.szxytkj.cn

JS:   JSON.parse(s)
来源：http://ul.colortex.cn

TS:   JSON.parse(s)
来源：http://mp.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bi.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://on.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://km.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://is.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://ad.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zd.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yd.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qf.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eg.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nn.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kp.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ir.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://jm.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cc.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vd.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gp.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oq.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bc.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zl.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://im.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ji.szxytkj.cn

[K05] 深拷贝对象
来源：http://mc.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://ws.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://sh.colortex.cn

JS:   structuredClone(obj)
来源：http://hr.colortex.cn

TS:   structuredClone(obj)
来源：http://tz.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iu.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gy.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ab.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vl.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://lh.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hb.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lv.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://we.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ti.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ml.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ew.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nj.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uv.shtwfgs.cn

[K07] 进制转换
来源：http://fg.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vp.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ga.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sa.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kp.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lg.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mw.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ii.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tu.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gh.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://ij.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qh.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://sz.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://gw.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://do.bookmarksfly.cn

Go:   encoding/gob
来源：http://kx.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://ye.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mj.nszjky.cn

================================================================================
来源：http://lr.shxzskj.cn

L. 网络请求
来源：http://kh.hnjuh.cn

================================================================================
来源：http://jb.szsharing.cn

[L01] 发送 GET 请求
来源：http://zl.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fe.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xg.huanxung.cn

JS:   await fetch(url)
来源：http://od.wgjwhj.cn

TS:   await fetch(url)
来源：http://pp.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ud.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://rp.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mr.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bv.colortex.cn

[L02] 发送 POST JSON
来源：http://xc.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kg.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yx.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tv.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ds.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://og.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wh.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ou.asd995.cn

[L03] 设置自定义请求头
来源：http://np.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://re.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hl.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wa.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eh.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pj.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://du.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fb.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dz.haigaiapp.cn

[L04] 设置超时
来源：http://na.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://lm.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kg.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://df.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cy.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vw.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ac.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hs.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wz.newstarts.cn

[L05] 上传文件（multipart）
来源：http://pw.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ko.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yo.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qu.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gz.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dw.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gt.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ny.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vd.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://lz.yuntaijiaju.cn

Py:   resp.json()
来源：http://io.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://bl.colortex.cn

JS:   await resp.json()
来源：http://jy.shxzskj.cn

TS:   await resp.json()
来源：http://tk.nszjky.cn


<!-- 参考信息 -->