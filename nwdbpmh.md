代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://mv.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ex.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ud.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tb.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lt.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bt.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qd.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rr.szsharing.cn

[H03] 主动抛出异常
来源：http://li.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ms.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jg.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://wc.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ji.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ei.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yf.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://py.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vy.shxzskj.cn

[H04] 自定义异常类型
来源：http://xi.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://ae.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gf.nicolike.cn

JS:   class MyError extends Error {}
来源：http://pl.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ot.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://kt.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ir.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://aa.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://si.shtwfgs.cn

[H05] 捕获特定类型
来源：http://sb.yuexingan06.cn

Py:   except ValueError as e:
来源：http://wq.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hc.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://ca.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hm.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://yz.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ky.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://aa.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tr.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://ge.9csxet.cn

Py:   value = d.get("k") or default
来源：http://rw.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wa.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mz.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uz.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jf.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ci.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://xf.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://tq.nszjky.cn

[H07] 断言
来源：http://ca.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://se.lnxyls.cn

PHP:  assert($x > 0);
来源：http://jp.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://ci.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://kn.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ra.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://in.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ly.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://xq.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://qr.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://jl.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://au.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ji.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jh.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wf.muxihuayi.cn

Go:   err.Error()
来源：http://dl.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ka.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://yt.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ui.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dh.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zq.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ke.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://in.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://de.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://co.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://da.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xr.chemitech.net.cn

[H10] 资源自动释放
来源：http://nl.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hp.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://km.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ec.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mv.bjjhwx.cn

Go:   defer f.Close()
来源：http://lk.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eg.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oe.haigaiapp.cn

================================================================================
来源：http://io.bookmarksfly.cn

I. 正则表达式
来源：http://cc.shtwfgs.cn

================================================================================
来源：http://gn.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://ze.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ee.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sq.hahajie.cn

JS:   /\d+/.test(s)
来源：http://nc.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://of.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jg.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gl.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://ry.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dq.muxihuayi.cn

[I02] 提取所有匹配
来源：http://en.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://zs.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://el.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jp.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://lr.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oe.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yl.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://ga.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ri.shtwfgs.cn

[I03] 提取捕获分组
来源：http://eh.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wl.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qw.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tf.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mn.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kt.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fx.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ox.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cn.bookmarksfly.cn

[I04] 正则替换
来源：http://jt.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pv.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kp.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pe.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ev.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://in.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://id.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dc.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xh.jctech888.com.cn

[I05] 按正则拆分
来源：http://tx.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xj.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ce.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://sw.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ie.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://gv.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kb.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hn.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kw.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hv.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gh.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qv.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qa.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zt.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vp.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xv.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rt.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ok.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://oh.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vn.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pz.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zc.chemitech.net.cn

TS:   /error/gim
来源：http://yi.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://et.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qv.asd995.cn

Ruby: s.scan(/error/i)
来源：http://ra.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lo.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ws.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pk.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ts.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dw.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ge.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gc.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nc.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ol.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://td.jianghongdianzi.cn

================================================================================
来源：http://bz.haigaiapp.cn

J. 日期与时间
来源：http://ma.bjjhwx.cn

================================================================================
来源：http://in.nicolike.cn

[J01] 获取当前时间
来源：http://jf.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gw.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zy.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://qq.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://nv.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sx.nszjky.cn

Go:   time.Now()
来源：http://ec.asd995.cn

Ruby: Time.now
来源：http://ig.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vh.newstarts.cn

[J02] 格式化输出
来源：http://rx.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xx.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dp.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sk.panjiajie.cn

TS:   d.toISOString()
来源：http://tr.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ne.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qs.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cb.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cp.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://ts.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wd.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cl.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://jb.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://li.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ix.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tj.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://cw.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kr.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://wo.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://js.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jk.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wy.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fn.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nw.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ut.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ok.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gu.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://mq.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://wf.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nq.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lx.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ja.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://lr.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wn.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://dz.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zk.hahajie.cn

[J06] 计算两时间之差
来源：http://wo.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://by.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://hp.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ks.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gx.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://md.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://hh.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://fw.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://qu.colortex.cn

[J07] 比较两个日期
来源：http://ry.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://dx.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qt.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dc.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bt.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vi.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oc.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xj.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yo.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://xm.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jv.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wb.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vb.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cl.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zw.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://un.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qf.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xl.jctech888.com.cn

[J09] 时区处理
来源：http://ff.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mg.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bq.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ko.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sv.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gw.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rx.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ke.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://up.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://yb.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pe.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ux.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fn.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zk.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://te.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zp.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yx.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yc.asd995.cn

================================================================================
来源：http://uj.szxytkj.cn

K. JSON 与序列化
来源：http://tx.huanxung.cn

================================================================================
来源：http://yt.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://qh.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gi.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://it.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ar.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://br.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mv.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://cx.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zw.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rj.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://su.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://dv.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wu.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ke.521024.cn

TS:   JSON.parse(s)
来源：http://id.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vf.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://gt.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://aj.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pc.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://qu.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uh.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://af.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zz.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://se.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rf.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xm.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ul.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lp.newstarts.cn

[K04] 读取 JSON 文件
来源：http://ah.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wm.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lc.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qz.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://od.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kc.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://do.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sl.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://er.521024.cn

[K05] 深拷贝对象
来源：http://vp.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://bq.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://jb.hnjuh.cn

JS:   structuredClone(obj)
来源：http://ix.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ai.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fv.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hi.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yf.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mo.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://yd.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fc.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ch.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hl.szsharing.cn


<!-- 参考信息 -->