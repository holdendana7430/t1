代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://xb.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xw.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xi.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ys.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fk.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tp.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ba.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://px.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://ck.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://gl.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gp.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://xl.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://la.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tw.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xq.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://si.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iq.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://ac.asd995.cn

Py:   class MyError(Exception): pass
来源：http://md.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lc.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://hp.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://du.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://ff.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aq.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://dk.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://ad.hahajie.cn

[H05] 捕获特定类型
来源：http://js.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://nh.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://co.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://dv.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://pz.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://uu.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lu.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://vv.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xl.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://vb.asd995.cn

Py:   value = d.get("k") or default
来源：http://wt.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vx.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hh.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dv.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oe.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nn.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://zl.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://wa.hnjuh.cn

[H07] 断言
来源：http://hd.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://dx.hahajie.cn

PHP:  assert($x > 0);
来源：http://ht.asd995.cn

JS:   console.assert(x > 0);
来源：http://io.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://vr.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://hf.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iz.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ry.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://bj.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://vu.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://lt.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rb.newstarts.cn

JS:   e.message;  e.stack
来源：http://gb.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rm.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gq.chemitech.net.cn

Go:   err.Error()
来源：http://ac.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://js.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://af.hahajie.cn

[H09] 带错误码的异常
来源：http://ci.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sh.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bo.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sl.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cj.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jo.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ki.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nv.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ng.9csxet.cn

[H10] 资源自动释放
来源：http://wg.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gn.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fq.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ud.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vo.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oc.muxihuayi.cn

Go:   defer f.Close()
来源：http://fn.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ku.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wg.newstarts.cn

================================================================================
来源：http://ji.shtwfgs.cn

I. 正则表达式
来源：http://hg.hnjuh.cn

================================================================================
来源：http://nh.bjjhwx.cn

[I01] 判断是否匹配
来源：http://xf.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aq.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fc.9csxet.cn

JS:   /\d+/.test(s)
来源：http://va.9csxet.cn

TS:   /\d+/.test(s)
来源：http://iv.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gb.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tc.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://oy.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dm.huixiangedu.cn

[I02] 提取所有匹配
来源：http://yi.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://zg.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mr.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zw.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://cm.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vl.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://me.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://sv.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qz.newstarts.cn

[I03] 提取捕获分组
来源：http://ak.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qg.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wn.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zq.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nz.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cz.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zl.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lb.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://td.huixinmuqiang.cn

[I04] 正则替换
来源：http://lt.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qk.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ei.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cw.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ub.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zh.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yz.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cu.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kl.hnjuh.cn

[I05] 按正则拆分
来源：http://id.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hk.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xn.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://qt.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://wc.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ha.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kr.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vq.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ao.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://js.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zm.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ws.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bn.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sq.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mb.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xk.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vj.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fx.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://lp.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bh.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bc.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nv.yuntaijiaju.cn

TS:   /error/gim
来源：http://gj.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ab.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zf.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://lu.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qp.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://oe.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lb.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://be.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dd.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iv.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fd.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bk.szsharing.cn

================================================================================
来源：http://ig.chemitech.net.cn

J. 日期与时间
来源：http://ek.wgjwhj.cn

================================================================================
来源：http://tn.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://db.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oy.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sa.hahajie.cn

JS:   new Date();  Date.now()
来源：http://hi.521024.cn

TS:   new Date();  Date.now()
来源：http://vq.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yv.jctech888.com.cn

Go:   time.Now()
来源：http://cn.shxzskj.cn

Ruby: Time.now
来源：http://na.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jk.nszjky.cn

[J02] 格式化输出
来源：http://ry.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mf.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gb.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nj.jctech888.com.cn

TS:   d.toISOString()
来源：http://ri.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ht.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mf.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gh.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wl.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ev.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://st.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pu.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://sp.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ov.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jx.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://da.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ji.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qe.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ti.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yo.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hv.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lf.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gq.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mz.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ea.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bg.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hw.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://im.521024.cn

Py:   now + timedelta(days=7)
来源：http://rk.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cq.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kl.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://of.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ei.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tm.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://gh.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uv.hnjuh.cn

[J06] 计算两时间之差
来源：http://ik.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://yb.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://bs.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ei.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sf.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bk.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://pt.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://ho.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://is.szxytkj.cn

[J07] 比较两个日期
来源：http://mx.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hb.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ml.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://as.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oz.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://il.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sr.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://du.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://ps.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://xc.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://te.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aj.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ts.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gq.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ty.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mb.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bm.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vs.yuntaijiaju.cn

[J09] 时区处理
来源：http://hg.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jx.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gl.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://so.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ty.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wk.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gc.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qa.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://or.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://kr.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://in.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ge.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ig.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vv.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qs.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wi.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uy.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lu.wgjwhj.cn

================================================================================
来源：http://ph.nszjky.cn

K. JSON 与序列化
来源：http://xw.bookmarksfly.cn

================================================================================
来源：http://ef.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://rd.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hg.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sb.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://ru.521024.cn

TS:   JSON.stringify(obj)
来源：http://fa.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://av.521024.cn

Go:   json.Marshal(obj)
来源：http://ne.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vl.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ap.huanxung.cn

[K02] JSON 字符串转对象
来源：http://js.chemitech.net.cn

Py:   json.loads(s)
来源：http://ww.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cf.nicolike.cn

JS:   JSON.parse(s)
来源：http://xh.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://cl.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mc.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://si.huanxung.cn

Ruby: JSON.parse(s)
来源：http://vg.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://te.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://wv.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dw.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mk.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kw.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fc.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iq.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ea.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wz.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gm.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://om.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wb.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vs.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iu.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ka.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pc.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tf.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bg.newstarts.cn

[K05] 深拷贝对象
来源：http://oe.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://md.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://xq.9csxet.cn

JS:   structuredClone(obj)
来源：http://xc.szsharing.cn

TS:   structuredClone(obj)
来源：http://ut.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://id.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pj.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gd.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mm.9csxet.cn

[K06] 解析 URL 查询串
来源：http://qj.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ky.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ao.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nf.asd995.cn


<!-- 参考信息 -->