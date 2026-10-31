代发 wailian999

[H07] 断言
来源：http://le.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://hq.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://ga.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://my.nszjky.cn

TS:   console.assert(x > 0);
来源：http://cp.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://mz.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ee.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://im.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://hr.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://lx.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://iw.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rp.huanxung.cn

JS:   e.message;  e.stack
来源：http://wj.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xl.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wb.colortex.cn

Go:   err.Error()
来源：http://ml.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ms.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://vj.lnxyls.cn

[H09] 带错误码的异常
来源：http://vg.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sf.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jd.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rr.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://md.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bq.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uv.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ug.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yi.9csxet.cn

[H10] 资源自动释放
来源：http://rj.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zd.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ps.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rk.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sv.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tb.huanxung.cn

Go:   defer f.Close()
来源：http://eo.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dc.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vy.huixiangedu.cn

================================================================================
来源：http://kv.nszjky.cn

I. 正则表达式
来源：http://kf.bjjhwx.cn

================================================================================
来源：http://zc.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://uk.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bg.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ru.9csxet.cn

JS:   /\d+/.test(s)
来源：http://rl.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://wj.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://re.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gs.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://oz.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gp.szxytkj.cn

[I02] 提取所有匹配
来源：http://kz.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://bm.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wq.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yh.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://fy.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ce.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hd.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://yt.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hm.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ud.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ii.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vc.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yb.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pn.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ou.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mo.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qb.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qm.shxzskj.cn

[I04] 正则替换
来源：http://cf.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tb.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ih.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ym.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xm.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nv.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://an.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ff.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nf.521024.cn

[I05] 按正则拆分
来源：http://dx.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uc.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qh.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://ws.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://pf.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ah.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bb.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rp.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yk.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xe.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vg.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nt.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yd.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ig.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://db.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sg.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nn.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yc.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://kf.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://us.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fp.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dk.bjjhwx.cn

TS:   /error/gim
来源：http://te.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bg.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tx.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://um.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://px.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://vc.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ov.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vw.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wn.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xm.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zv.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ih.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oz.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cu.haigaiapp.cn

================================================================================
来源：http://ub.lnxyls.cn

J. 日期与时间
来源：http://vt.muxihuayi.cn

================================================================================
来源：http://jt.shxzukj.cn

[J01] 获取当前时间
来源：http://jn.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fn.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kp.hahajie.cn

JS:   new Date();  Date.now()
来源：http://ib.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://no.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qf.yuexingan06.cn

Go:   time.Now()
来源：http://yf.muxihuayi.cn

Ruby: Time.now
来源：http://xo.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cx.shtwfgs.cn

[J02] 格式化输出
来源：http://ua.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nm.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mg.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://px.chemitech.net.cn

TS:   d.toISOString()
来源：http://zw.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cr.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ow.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jw.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ug.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://ld.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xm.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ri.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ya.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://ak.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cv.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vw.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://hp.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://um.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://mb.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hk.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gz.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pi.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rx.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xp.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sl.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oz.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://in.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://bg.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://uk.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://np.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jb.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cl.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://hl.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uh.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://vv.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oc.huanxung.cn

[J06] 计算两时间之差
来源：http://de.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://hg.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://vf.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cs.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gy.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sf.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://td.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ni.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://to.521024.cn

[J07] 比较两个日期
来源：http://nr.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://lc.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gv.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mh.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ar.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zb.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dx.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mp.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://xn.nicolike.cn

[J08] 提取年月日与星期
来源：http://vf.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yp.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nc.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fc.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oy.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ai.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kx.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ry.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ny.muxihuayi.cn

[J09] 时区处理
来源：http://eo.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://in.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gd.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ax.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xz.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ja.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ja.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mw.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zp.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://qs.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jo.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kz.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://as.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wo.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yj.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gg.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xs.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jw.jctech888.com.cn

================================================================================
来源：http://ed.chemitech.net.cn

K. JSON 与序列化
来源：http://mx.hnjuh.cn

================================================================================
来源：http://tp.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://wd.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qx.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ib.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://mu.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uy.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://qd.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ed.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gh.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://yo.hahajie.cn

Py:   json.loads(s)
来源：http://fx.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oz.nszjky.cn

JS:   JSON.parse(s)
来源：http://vh.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://vu.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xt.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://ov.nicolike.cn

Ruby: JSON.parse(s)
来源：http://ku.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tv.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://jo.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ti.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ga.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yp.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zf.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sv.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lu.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://av.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ul.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://rl.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ii.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ti.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vf.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bc.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pu.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pb.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dm.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jb.shtwfgs.cn

[K05] 深拷贝对象
来源：http://kw.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://le.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ue.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ml.lnxyls.cn

TS:   structuredClone(obj)
来源：http://sj.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://my.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hh.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hj.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://av.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://by.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mp.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tw.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ki.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wi.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fr.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gz.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pc.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qz.panjiajie.cn

[K07] 进制转换
来源：http://nx.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wa.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nw.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tv.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fg.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aw.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pu.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://be.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cp.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ae.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://cb.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qd.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://le.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ir.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vc.shxzskj.cn

Go:   encoding/gob
来源：http://bl.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://cx.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ku.shxzukj.cn

================================================================================
来源：http://wb.panjiajie.cn

L. 网络请求
来源：http://nj.nicolike.cn

================================================================================
来源：http://sc.nszjky.cn

[L01] 发送 GET 请求
来源：http://uh.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vn.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fb.szsharing.cn

JS:   await fetch(url)
来源：http://oy.colortex.cn

TS:   await fetch(url)
来源：http://ed.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ni.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://zj.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fs.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wi.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://ja.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rk.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://am.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sd.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gv.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fh.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jd.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pn.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://um.wgjwhj.cn


<!-- 参考信息 -->