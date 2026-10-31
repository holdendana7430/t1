代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://pe.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ia.chemitech.net.cn

[H09] 带错误码的异常
来源：http://tz.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aw.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://li.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rp.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fa.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ue.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kp.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iq.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vr.yuexingan06.cn

[H10] 资源自动释放
来源：http://jb.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fo.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://se.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vz.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dy.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sp.huanxung.cn

Go:   defer f.Close()
来源：http://bl.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://px.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ic.szxytkj.cn

================================================================================
来源：http://nq.asd995.cn

I. 正则表达式
来源：http://vp.szxytkj.cn

================================================================================
来源：http://ce.521024.cn

[I01] 判断是否匹配
来源：http://iq.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yr.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hu.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://bc.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://as.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dy.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wg.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://xf.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://km.huixiangedu.cn

[I02] 提取所有匹配
来源：http://xu.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://ky.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lj.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kt.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ed.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tr.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fo.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://cd.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://me.newstarts.cn

[I03] 提取捕获分组
来源：http://tx.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gr.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ke.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ux.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hs.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wc.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qi.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ts.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cb.asd995.cn

[I04] 正则替换
来源：http://ar.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oo.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ki.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ye.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://un.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fc.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qb.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nw.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qp.colortex.cn

[I05] 按正则拆分
来源：http://uz.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jr.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cq.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://ru.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://cd.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://fo.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ta.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pg.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nh.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rq.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ei.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zd.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qr.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cq.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yd.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://be.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yi.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ox.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://du.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ss.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vp.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fd.9csxet.cn

TS:   /error/gim
来源：http://yw.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qq.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mc.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://yc.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fx.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rp.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://be.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qc.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mv.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wf.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://el.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oy.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zh.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ui.lnxyls.cn

================================================================================
来源：http://lp.huixinmuqiang.cn

J. 日期与时间
来源：http://nr.szxytkj.cn

================================================================================
来源：http://gb.521024.cn

[J01] 获取当前时间
来源：http://bw.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cy.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dc.nicolike.cn

JS:   new Date();  Date.now()
来源：http://ik.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://of.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hb.nicolike.cn

Go:   time.Now()
来源：http://yl.huixiangedu.cn

Ruby: Time.now
来源：http://nn.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xq.huanxung.cn

[J02] 格式化输出
来源：http://ct.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pu.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://se.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jw.hahajie.cn

TS:   d.toISOString()
来源：http://zo.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hs.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cv.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jw.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rz.shxzukj.cn

[J03] 字符串解析为日期
来源：http://pt.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vp.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dg.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://jo.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://mz.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://up.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qy.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://un.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qv.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://xx.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ey.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qh.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rt.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uh.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xw.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ra.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qa.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mo.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://gm.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://qs.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fi.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ep.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bb.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://eo.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eg.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://lk.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gl.huixiangedu.cn

[J06] 计算两时间之差
来源：http://nj.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://fx.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://kb.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zl.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nl.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xy.521024.cn

Go:   end.Sub(start).Hours()
来源：http://ct.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://fw.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://nt.jctech888.com.cn

[J07] 比较两个日期
来源：http://kh.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hk.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iq.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jd.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bl.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ep.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fl.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ot.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://yo.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://lc.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qq.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ah.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sk.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ph.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pe.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zc.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bl.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tr.shxzskj.cn

[J09] 时区处理
来源：http://kq.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hp.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rc.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bp.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xv.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bx.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tz.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ai.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vv.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://dk.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gj.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bi.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ip.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yb.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://en.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vc.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ce.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tb.jianghongdianzi.cn

================================================================================
来源：http://xx.shxzukj.cn

K. JSON 与序列化
来源：http://zh.shtwfgs.cn

================================================================================
来源：http://km.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://rx.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xh.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xo.colortex.cn

JS:   JSON.stringify(obj)
来源：http://bg.colortex.cn

TS:   JSON.stringify(obj)
来源：http://mp.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dq.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://rd.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iu.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ch.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://ic.szxytkj.cn

Py:   json.loads(s)
来源：http://ls.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jb.huanxung.cn

JS:   JSON.parse(s)
来源：http://qz.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://go.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cv.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ff.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://cr.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ka.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://go.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jc.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xb.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yy.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qk.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://al.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ze.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zc.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qv.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://cy.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yr.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xm.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ds.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ua.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pw.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kk.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rk.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qe.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://wv.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://hs.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://hs.newstarts.cn

JS:   structuredClone(obj)
来源：http://py.shxzskj.cn

TS:   structuredClone(obj)
来源：http://kk.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fi.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tg.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lu.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sh.nszjky.cn

[K06] 解析 URL 查询串
来源：http://oj.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zy.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wu.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kf.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wy.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://en.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kz.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uc.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rz.szxytkj.cn

[K07] 进制转换
来源：http://yf.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qz.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tf.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ba.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dl.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ts.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ie.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zz.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jf.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://pt.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://uk.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tf.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://tu.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://zq.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wu.chemitech.net.cn

Go:   encoding/gob
来源：http://qd.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://tr.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xe.szsharing.cn

================================================================================
来源：http://ej.lnxyls.cn

L. 网络请求
来源：http://pg.haigaiapp.cn

================================================================================
来源：http://iw.nicolike.cn

[L01] 发送 GET 请求
来源：http://ef.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eb.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gm.shtwfgs.cn

JS:   await fetch(url)
来源：http://wx.gzmigu.cn

TS:   await fetch(url)
来源：http://hh.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://am.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ey.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hd.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nf.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://vx.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tq.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jh.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zh.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://my.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cp.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://az.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bp.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://jz.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wt.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cp.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qf.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wo.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yf.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hh.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hf.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://it.colortex.cn

[L04] 设置超时
来源：http://ay.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://jh.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ga.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uc.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dz.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ep.newstarts.cn


<!-- 参考信息 -->