代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://ev.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ao.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lq.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://em.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iy.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qb.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uw.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qc.shxzskj.cn

[H03] 主动抛出异常
来源：http://zm.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://lx.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hs.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://pm.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://sv.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xj.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://am.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rl.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ea.jctech888.com.cn

[H04] 自定义异常类型
来源：http://os.colortex.cn

Py:   class MyError(Exception): pass
来源：http://uh.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eo.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://or.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://jz.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://hy.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ok.521024.cn

Ruby: class MyError < StandardError; end
来源：http://tn.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://nj.haigaiapp.cn

[H05] 捕获特定类型
来源：http://wm.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://mh.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zx.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://yx.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ip.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://gb.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://my.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://cv.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zb.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://pp.colortex.cn

Py:   value = d.get("k") or default
来源：http://gc.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cb.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oc.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nu.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wp.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wd.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://dq.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://dt.huanxung.cn

[H07] 断言
来源：http://np.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://al.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://ud.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://lu.521024.cn

TS:   console.assert(x > 0);
来源：http://rz.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://bj.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bo.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uy.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://sy.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://gm.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://ey.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uz.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://le.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fu.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oc.wgjwhj.cn

Go:   err.Error()
来源：http://tl.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ne.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://mp.colortex.cn

[H09] 带错误码的异常
来源：http://mb.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pq.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dl.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kn.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sz.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kt.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hk.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fl.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yh.huanxung.cn

[H10] 资源自动释放
来源：http://wt.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lh.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://da.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://so.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cx.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yr.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://fr.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jy.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kt.shxzskj.cn

================================================================================
来源：http://ko.shxzukj.cn

I. 正则表达式
来源：http://he.huixiangedu.cn

================================================================================
来源：http://mw.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://se.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ec.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qi.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://pu.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://rb.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://db.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mh.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://qj.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hv.huanxung.cn

[I02] 提取所有匹配
来源：http://lh.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://pb.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rc.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wk.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://og.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hh.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gz.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://xn.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://di.shtwfgs.cn

[I03] 提取捕获分组
来源：http://oj.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vz.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cd.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pj.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qq.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ag.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qr.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://of.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zw.9csxet.cn

[I04] 正则替换
来源：http://nz.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oc.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fb.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://km.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://na.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://od.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ac.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://we.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oa.shxzskj.cn

[I05] 按正则拆分
来源：http://iy.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mw.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://es.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://hc.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://bm.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://hd.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mp.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sy.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xg.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ic.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://my.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mp.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://af.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rc.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bu.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pv.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ec.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ka.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://lx.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aj.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pl.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ou.9csxet.cn

TS:   /error/gim
来源：http://zo.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fj.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ln.colortex.cn

Ruby: s.scan(/error/i)
来源：http://en.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pt.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://kg.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jm.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gt.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://np.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dq.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qo.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wz.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iy.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eb.asd995.cn

================================================================================
来源：http://qo.chemitech.net.cn

J. 日期与时间
来源：http://sa.szxytkj.cn

================================================================================
来源：http://lv.muxihuayi.cn

[J01] 获取当前时间
来源：http://ts.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yj.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bk.9csxet.cn

JS:   new Date();  Date.now()
来源：http://wt.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://ne.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eh.huixinmuqiang.cn

Go:   time.Now()
来源：http://lf.chemitech.net.cn

Ruby: Time.now
来源：http://ed.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kc.9csxet.cn

[J02] 格式化输出
来源：http://ai.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zo.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://or.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.asd995.cn

TS:   d.toISOString()
来源：http://vv.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ns.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kb.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iq.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://py.hnjuh.cn

[J03] 字符串解析为日期
来源：http://mv.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bt.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ym.colortex.cn

JS:   new Date("2024-01-02")
来源：http://hp.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://wa.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tw.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zg.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://bw.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cq.szsharing.cn

[J04] 时间戳与日期互转
来源：http://xj.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sh.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sc.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ad.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ud.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sn.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ta.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eh.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ty.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://cr.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://yv.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pl.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uc.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ok.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://po.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rq.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://ik.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ru.newstarts.cn

[J06] 计算两时间之差
来源：http://go.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://sh.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://so.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ae.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fw.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://of.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://ot.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://lj.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://hb.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://sm.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://oo.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pi.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pi.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sq.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tq.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dl.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mw.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://cf.lnxyls.cn

[J08] 提取年月日与星期
来源：http://qe.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://or.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aq.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gh.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qh.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pv.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vr.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ik.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kc.szxytkj.cn

[J09] 时区处理
来源：http://ax.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cw.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ax.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mb.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oq.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bs.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jz.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xk.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fl.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://rf.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vg.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uq.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qv.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xd.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dx.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xh.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lw.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://py.muxihuayi.cn

================================================================================
来源：http://cm.haigaiapp.cn

K. JSON 与序列化
来源：http://xv.shtwfgs.cn

================================================================================
来源：http://bz.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://tt.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://re.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://st.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://zq.colortex.cn

TS:   JSON.stringify(obj)
来源：http://sl.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ah.szsharing.cn

Go:   json.Marshal(obj)
来源：http://el.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ik.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ze.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://tv.hahajie.cn

Py:   json.loads(s)
来源：http://ul.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vy.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://iy.colortex.cn

TS:   JSON.parse(s)
来源：http://oz.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://du.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://bu.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://mb.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lj.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://xq.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yp.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zk.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://my.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ku.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ph.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sh.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ja.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ec.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wo.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://et.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lq.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iw.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mk.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ug.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qy.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ga.asd995.cn

[K05] 深拷贝对象
来源：http://vf.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://ui.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://qt.huanxung.cn

JS:   structuredClone(obj)
来源：http://fd.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ak.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yj.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fx.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ri.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qw.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://ry.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://km.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kx.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jm.yuntaijiaju.cn


<!-- 参考信息 -->