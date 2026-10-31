代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://pv.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://kh.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://vy.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hq.szxytkj.cn

JS:   e.message;  e.stack
来源：http://dj.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lj.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bt.szsharing.cn

Go:   err.Error()
来源：http://jy.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://qd.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://oz.lnxyls.cn

[H09] 带错误码的异常
来源：http://ir.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://si.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ld.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uw.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bu.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qr.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hp.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kf.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mc.szxytkj.cn

[H10] 资源自动释放
来源：http://xh.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gr.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wb.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zb.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ir.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sq.shxzukj.cn

Go:   defer f.Close()
来源：http://ak.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pt.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://px.shxzukj.cn

================================================================================
来源：http://gy.9csxet.cn

I. 正则表达式
来源：http://zg.chemitech.net.cn

================================================================================
来源：http://sm.hnjuh.cn

[I01] 判断是否匹配
来源：http://kv.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://il.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ba.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://mu.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://qr.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gj.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sf.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://cw.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vn.newstarts.cn

[I02] 提取所有匹配
来源：http://xq.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://di.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zn.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nw.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://da.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ua.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wk.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://pl.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yb.521024.cn

[I03] 提取捕获分组
来源：http://po.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yt.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://il.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://va.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vo.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uq.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ts.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ty.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jr.haigaiapp.cn

[I04] 正则替换
来源：http://yw.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xr.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qd.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zl.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ps.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cd.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xm.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fk.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ke.shtwfgs.cn

[I05] 按正则拆分
来源：http://dz.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tx.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://el.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://wh.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://wy.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://wy.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vs.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ae.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qc.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dg.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iq.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ny.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gh.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bf.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bv.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oe.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ss.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cw.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://jm.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pn.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://at.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wk.nicolike.cn

TS:   /error/gim
来源：http://cf.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cu.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vw.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://rj.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rb.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xq.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fo.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lw.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://by.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bs.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oh.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qm.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zm.shtwfgs.cn

================================================================================
来源：http://jc.yuntaijiaju.cn

J. 日期与时间
来源：http://uo.yuexingan06.cn

================================================================================
来源：http://sf.nszjky.cn

[J01] 获取当前时间
来源：http://kl.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cl.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ye.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://vt.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://kg.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ga.bookmarksfly.cn

Go:   time.Now()
来源：http://df.bookmarksfly.cn

Ruby: Time.now
来源：http://af.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wl.colortex.cn

[J02] 格式化输出
来源：http://mm.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mj.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vh.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rp.muxihuayi.cn

TS:   d.toISOString()
来源：http://oh.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ks.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sj.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ww.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kd.nicolike.cn

[J03] 字符串解析为日期
来源：http://gg.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sl.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://jm.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://dt.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ag.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sc.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://ww.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gi.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://nc.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kd.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gy.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wt.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gu.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cm.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zz.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://er.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sg.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://mi.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://vl.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cg.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gq.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nz.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://uz.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lw.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://kt.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tb.szsharing.cn

[J06] 计算两时间之差
来源：http://uu.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://mo.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://uw.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zx.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hv.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zr.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://zm.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ww.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://jn.asd995.cn

[J07] 比较两个日期
来源：http://ie.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://dy.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xv.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rk.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ck.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iy.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yv.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vo.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://bl.asd995.cn

[J08] 提取年月日与星期
来源：http://ci.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hc.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ve.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iq.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://as.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://no.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yg.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vi.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xj.nicolike.cn

[J09] 时区处理
来源：http://um.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bw.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ft.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ug.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tx.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cl.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vy.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xj.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ig.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://sx.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sy.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ia.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pt.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fu.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ih.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jj.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hc.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oh.huanxung.cn

================================================================================
来源：http://lm.muxihuayi.cn

K. JSON 与序列化
来源：http://tj.shxzukj.cn

================================================================================
来源：http://ai.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://al.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lc.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fr.asd995.cn

JS:   JSON.stringify(obj)
来源：http://dw.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ki.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://px.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ox.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kp.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zd.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://ks.haigaiapp.cn

Py:   json.loads(s)
来源：http://hp.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gz.newstarts.cn

JS:   JSON.parse(s)
来源：http://xi.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://dh.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cz.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://bu.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ay.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://da.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://km.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ut.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://am.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yy.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uy.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ct.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rx.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rt.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kz.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://oa.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jw.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://by.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mt.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://du.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mg.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xl.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ip.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tx.9csxet.cn

[K05] 深拷贝对象
来源：http://jb.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://jp.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ad.newstarts.cn

JS:   structuredClone(obj)
来源：http://yt.colortex.cn

TS:   structuredClone(obj)
来源：http://ul.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://im.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oe.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lt.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://va.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://yg.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jf.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dp.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vu.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tp.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aw.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gn.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bm.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zv.jctech888.com.cn

[K07] 进制转换
来源：http://go.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dr.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dt.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dc.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vp.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sh.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dm.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ui.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://hg.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://zp.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ut.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://lt.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://rb.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nl.jianghongdianzi.cn

Go:   encoding/gob
来源：http://ap.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://yq.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qv.newstarts.cn

================================================================================
来源：http://tc.jianghongdianzi.cn

L. 网络请求
来源：http://kb.gzmigu.cn

================================================================================
来源：http://et.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://qu.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iw.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ig.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://qf.shtwfgs.cn

TS:   await fetch(url)
来源：http://me.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xw.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://yv.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://px.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oh.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://my.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ky.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ly.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ge.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zs.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cl.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bo.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dq.colortex.cn

[L03] 设置自定义请求头
来源：http://kz.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jv.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pl.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bu.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ng.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rl.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fv.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tx.szsharing.cn


<!-- 参考信息 -->