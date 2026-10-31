代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://jj.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zl.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://my.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zv.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lu.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ga.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uh.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nl.lnxyls.cn

[H03] 主动抛出异常
来源：http://kj.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://sp.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zw.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://pg.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://qe.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rg.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ov.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vr.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ye.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://xi.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://wm.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dv.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://xe.huanxung.cn

TS:   class MyError extends Error {}
来源：http://gm.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://sq.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ej.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://oi.newstarts.cn

C#:   class MyException : Exception {}
来源：http://ex.hnjuh.cn

[H05] 捕获特定类型
来源：http://xi.huixiangedu.cn

Py:   except ValueError as e:
来源：http://gr.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ti.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://zf.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ri.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://gz.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://th.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://zj.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xm.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://jt.newstarts.cn

Py:   value = d.get("k") or default
来源：http://cy.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uu.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ab.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ow.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cx.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sg.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://mw.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://uj.hnjuh.cn

[H07] 断言
来源：http://mk.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://fi.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://ub.colortex.cn

JS:   console.assert(x > 0);
来源：http://eb.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ze.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://kc.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qk.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kh.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://rk.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://qk.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://og.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zt.panjiajie.cn

JS:   e.message;  e.stack
来源：http://kz.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ax.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rm.hahajie.cn

Go:   err.Error()
来源：http://ff.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://wr.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://it.nszjky.cn

[H09] 带错误码的异常
来源：http://ic.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xp.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bu.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qh.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eg.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rp.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ex.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zu.chemitech.net.cn

[H10] 资源自动释放
来源：http://cf.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wn.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dm.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dd.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iy.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://du.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://hy.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jh.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://il.haigaiapp.cn

================================================================================
来源：http://dk.yuexingan06.cn

I. 正则表达式
来源：http://bw.shtwfgs.cn

================================================================================
来源：http://db.newstarts.cn

[I01] 判断是否匹配
来源：http://zt.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://is.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rk.colortex.cn

JS:   /\d+/.test(s)
来源：http://rk.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://ax.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oq.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ph.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://pe.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nj.colortex.cn

[I02] 提取所有匹配
来源：http://cv.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://ia.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jk.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bn.521024.cn

TS:   s.match(/\d+/g)
来源：http://cc.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nm.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ka.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mt.jctech888.com.cn

[I03] 提取捕获分组
来源：http://eb.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lz.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ep.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xm.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yy.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dv.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://au.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gk.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ja.haigaiapp.cn

[I04] 正则替换
来源：http://vj.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://if.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uy.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yf.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rf.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gz.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qy.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hf.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zo.muxihuayi.cn

[I05] 按正则拆分
来源：http://wd.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sv.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nm.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://ix.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ng.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://fn.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zw.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eb.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sk.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tv.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dj.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ip.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nd.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lp.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://le.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hx.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wj.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://yq.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fl.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zw.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bf.colortex.cn

TS:   /error/gim
来源：http://me.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qa.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pt.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://fm.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mv.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://sr.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bk.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kx.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gp.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eb.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cx.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jg.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ai.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pe.colortex.cn

================================================================================
来源：http://na.chemitech.net.cn

J. 日期与时间
来源：http://gq.lnxyls.cn

================================================================================
来源：http://ma.lnxyls.cn

[J01] 获取当前时间
来源：http://dl.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kw.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jy.szsharing.cn

JS:   new Date();  Date.now()
来源：http://ga.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://jb.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mp.chemitech.net.cn

Go:   time.Now()
来源：http://pi.huixiangedu.cn

Ruby: Time.now
来源：http://na.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rb.gzmigu.cn

[J02] 格式化输出
来源：http://ge.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sz.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://us.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wx.hnjuh.cn

TS:   d.toISOString()
来源：http://hg.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ga.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mb.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hy.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ox.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ys.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sg.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nd.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://fe.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://mp.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hz.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vs.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://an.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uz.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://vf.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bq.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xz.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mb.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wv.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sg.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://of.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zn.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rd.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://vo.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://sj.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kn.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rj.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mj.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://tg.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zk.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://pj.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ht.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://mv.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://hl.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://kz.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jl.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lz.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oh.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://pz.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://ed.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://il.muxihuayi.cn

[J07] 比较两个日期
来源：http://ui.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://dm.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ye.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lu.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dv.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gc.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://el.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zf.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://vg.szsharing.cn

[J08] 提取年月日与星期
来源：http://xl.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uu.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rg.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ue.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qm.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zu.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jm.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cv.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ot.huanxung.cn

[J09] 时区处理
来源：http://wn.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ad.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://io.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iw.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ec.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xj.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xv.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gz.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ch.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://fo.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ku.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oj.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oi.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ff.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hj.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bc.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ic.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://em.yuntaijiaju.cn

================================================================================
来源：http://xm.bjjhwx.cn

K. JSON 与序列化
来源：http://uc.nszjky.cn

================================================================================
来源：http://pf.521024.cn

[K01] 对象转 JSON 字符串
来源：http://tu.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gi.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qr.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://uj.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://hj.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ir.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://pl.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ej.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pv.nszjky.cn

[K02] JSON 字符串转对象
来源：http://qz.asd995.cn

Py:   json.loads(s)
来源：http://id.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cr.asd995.cn

JS:   JSON.parse(s)
来源：http://qq.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://fv.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://do.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ak.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://mk.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wn.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://fa.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pn.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zu.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ij.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tt.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nb.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xu.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gm.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rn.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://bi.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://de.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fx.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bh.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ju.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lu.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sv.colortex.cn

[K05] 深拷贝对象
来源：http://ur.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://yl.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://rq.nicolike.cn

JS:   structuredClone(obj)
来源：http://oz.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://xw.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yg.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ag.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zb.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cl.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://af.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jn.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nw.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jo.szxytkj.cn


<!-- 参考信息 -->