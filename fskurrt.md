代发 wailian999

[H07] 断言
来源：http://qi.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://nz.colortex.cn

PHP:  assert($x > 0);
来源：http://xv.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://yp.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://mv.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://xc.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gl.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gr.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://vh.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://fj.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://jt.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mk.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://ce.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dm.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aa.muxihuayi.cn

Go:   err.Error()
来源：http://zh.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://oy.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://xm.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://us.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ek.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nm.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gv.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gw.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ju.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cu.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ev.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tj.yuexingan06.cn

[H10] 资源自动释放
来源：http://qt.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ji.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bh.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zu.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ni.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sm.nszjky.cn

Go:   defer f.Close()
来源：http://pg.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://th.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://co.wgjwhj.cn

================================================================================
来源：http://gq.bjjhwx.cn

I. 正则表达式
来源：http://sl.szxytkj.cn

================================================================================
来源：http://ws.szxytkj.cn

[I01] 判断是否匹配
来源：http://rz.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gc.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://td.nszjky.cn

JS:   /\d+/.test(s)
来源：http://wb.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://sk.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qu.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://da.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://jn.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xf.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://oc.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://cd.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dx.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lm.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://fn.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://je.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rz.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://nu.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bq.szxytkj.cn

[I03] 提取捕获分组
来源：http://hp.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ub.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sp.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hs.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://go.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jq.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iy.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xt.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ic.shxzukj.cn

[I04] 正则替换
来源：http://lk.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vu.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://th.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ev.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wq.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ec.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lf.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ho.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vw.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://bl.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ss.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bf.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://dv.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ap.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://dz.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ev.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ix.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ql.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fd.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sa.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iy.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://de.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lx.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://og.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gw.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fc.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zp.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ui.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qe.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://al.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tv.szxytkj.cn

TS:   /error/gim
来源：http://ej.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bw.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ad.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://mg.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gj.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://wk.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wo.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rk.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ef.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ov.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://me.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zk.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rr.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nr.asd995.cn

================================================================================
来源：http://av.huixiangedu.cn

J. 日期与时间
来源：http://kp.nszjky.cn

================================================================================
来源：http://xy.asd995.cn

[J01] 获取当前时间
来源：http://dy.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zm.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ve.nszjky.cn

JS:   new Date();  Date.now()
来源：http://zt.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://zd.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ej.wgjwhj.cn

Go:   time.Now()
来源：http://ze.shxzukj.cn

Ruby: Time.now
来源：http://mw.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zp.huixiangedu.cn

[J02] 格式化输出
来源：http://rd.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jh.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cb.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ub.jctech888.com.cn

TS:   d.toISOString()
来源：http://bu.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ct.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hh.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bx.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ps.nszjky.cn

[J03] 字符串解析为日期
来源：http://pi.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xy.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xg.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://my.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://aj.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rs.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vl.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://xx.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vz.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://jn.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ed.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ym.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wr.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mc.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ua.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nn.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://md.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xe.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://ru.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://ab.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xv.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nf.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bk.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://rp.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rk.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://yr.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yp.hnjuh.cn

[J06] 计算两时间之差
来源：http://mr.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ag.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ot.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wh.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ki.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wg.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://er.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://hp.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://hv.colortex.cn

[J07] 比较两个日期
来源：http://pf.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://oy.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vz.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vb.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aa.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hm.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vd.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ut.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://kx.lnxyls.cn

[J08] 提取年月日与星期
来源：http://bl.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yg.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xt.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ro.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uv.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wf.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gj.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gr.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sn.haigaiapp.cn

[J09] 时区处理
来源：http://fx.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bv.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://np.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ra.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sj.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rh.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://io.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mo.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://db.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://db.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://an.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://my.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dt.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sy.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jr.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sd.huixinmuqiang.cn

================================================================================
来源：http://nj.huixinmuqiang.cn

K. JSON 与序列化
来源：http://lq.521024.cn

================================================================================
来源：http://md.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://xi.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kq.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ni.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://eu.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://bi.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ax.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://nd.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qq.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zr.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://qk.shxzukj.cn

Py:   json.loads(s)
来源：http://je.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://op.huanxung.cn

JS:   JSON.parse(s)
来源：http://hi.hnjuh.cn

TS:   JSON.parse(s)
来源：http://kw.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vc.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://sm.colortex.cn

Ruby: JSON.parse(s)
来源：http://nv.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rg.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://yc.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://at.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ru.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zi.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://se.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vl.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xf.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tl.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zu.colortex.cn

[K04] 读取 JSON 文件
来源：http://rt.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jn.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kn.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kl.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mw.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mq.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xw.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sy.panjiajie.cn

[K05] 深拷贝对象
来源：http://lc.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://ar.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ru.gzmigu.cn

JS:   structuredClone(obj)
来源：http://re.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ab.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zw.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bm.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://is.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xk.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://ot.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wx.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://th.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cq.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xl.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zf.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mm.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uw.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lc.hnjuh.cn

[K07] 进制转换
来源：http://ab.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mg.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fw.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aq.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://li.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tr.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eg.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rs.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nb.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://qi.521024.cn

Py:   pickle.dumps(obj)
来源：http://uq.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yb.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zd.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://xp.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sp.yuexingan06.cn

Go:   encoding/gob
来源：http://lt.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://ov.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jc.nszjky.cn

================================================================================
来源：http://bp.jianghongdianzi.cn

L. 网络请求
来源：http://ph.yuntaijiaju.cn

================================================================================
来源：http://ue.colortex.cn

[L01] 发送 GET 请求
来源：http://pw.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gi.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uf.521024.cn

JS:   await fetch(url)
来源：http://aq.jctech888.com.cn

TS:   await fetch(url)
来源：http://gi.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uy.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://mn.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ml.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gi.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://he.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ek.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ai.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gl.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yd.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://th.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sv.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fe.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://li.wgjwhj.cn


<!-- 参考信息 -->