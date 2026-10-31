代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://xm.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zl.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mv.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.muxihuayi.cn

[H03] 主动抛出异常
来源：http://mr.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://md.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://js.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://gq.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://wy.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://di.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://um.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lr.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kf.szxytkj.cn

[H04] 自定义异常类型
来源：http://rr.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://ih.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ny.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://gf.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://wh.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://su.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ep.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://rx.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://ns.bjjhwx.cn

[H05] 捕获特定类型
来源：http://ex.huanxung.cn

Py:   except ValueError as e:
来源：http://kg.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aw.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://vb.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://zp.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://yv.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oy.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://uz.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bc.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://yv.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://zl.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pg.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ho.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ww.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lx.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wl.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://xk.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://nc.yuexingan06.cn

[H07] 断言
来源：http://ai.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://du.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://rr.asd995.cn

JS:   console.assert(x > 0);
来源：http://jd.huanxung.cn

TS:   console.assert(x > 0);
来源：http://qt.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://vj.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iw.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tq.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://em.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://nr.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://dh.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kg.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://iq.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fy.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xm.szxytkj.cn

Go:   err.Error()
来源：http://ib.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://ip.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://vw.shtwfgs.cn

[H09] 带错误码的异常
来源：http://rl.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cn.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zm.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zv.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wl.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dw.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lx.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://et.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tg.nicolike.cn

[H10] 资源自动释放
来源：http://yn.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://un.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pe.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yx.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xh.jctech888.com.cn

Go:   defer f.Close()
来源：http://tv.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ml.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ea.wgjwhj.cn

================================================================================
来源：http://eo.haigaiapp.cn

I. 正则表达式
来源：http://nm.chemitech.net.cn

================================================================================
来源：http://ml.9csxet.cn

[I01] 判断是否匹配
来源：http://mp.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vr.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tr.colortex.cn

JS:   /\d+/.test(s)
来源：http://lf.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://rq.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ca.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rf.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://ro.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jd.lnxyls.cn

[I02] 提取所有匹配
来源：http://qn.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://uj.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://br.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ti.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://hw.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dl.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ix.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://gr.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ct.nicolike.cn

[I03] 提取捕获分组
来源：http://gf.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://se.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bu.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ky.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://al.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lx.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wl.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wu.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dl.gzmigu.cn

[I04] 正则替换
来源：http://ny.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jt.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tl.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ye.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uh.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vz.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://im.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://es.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sk.huanxung.cn

[I05] 按正则拆分
来源：http://gy.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cb.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yu.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://to.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://or.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://st.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://po.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tr.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sv.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dx.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bl.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ll.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fo.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cz.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://af.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bc.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sj.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mp.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://od.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ad.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://au.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jj.bookmarksfly.cn

TS:   /error/gim
来源：http://qx.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uk.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ja.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://he.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cd.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://jl.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sq.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jh.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wx.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qx.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zn.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ak.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ol.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://up.hahajie.cn

================================================================================
来源：http://wp.szxytkj.cn

J. 日期与时间
来源：http://fo.nszjky.cn

================================================================================
来源：http://qc.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://tg.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qp.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zu.newstarts.cn

JS:   new Date();  Date.now()
来源：http://fp.nicolike.cn

TS:   new Date();  Date.now()
来源：http://uo.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tv.asd995.cn

Go:   time.Now()
来源：http://an.panjiajie.cn

Ruby: Time.now
来源：http://tv.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://co.panjiajie.cn

[J02] 格式化输出
来源：http://ub.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bv.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aq.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.jctech888.com.cn

TS:   d.toISOString()
来源：http://qm.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cd.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cu.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wz.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://md.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://gh.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pe.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nt.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ed.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://fr.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://om.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://op.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://fu.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zv.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://qj.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ua.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fj.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://le.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bi.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vt.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lm.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qw.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mo.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://wn.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://ra.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zn.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bn.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://lq.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zb.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://op.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qs.521024.cn

[J06] 计算两时间之差
来源：http://ht.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://cl.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://by.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hk.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jb.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vc.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://st.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://ma.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://oi.521024.cn

[J07] 比较两个日期
来源：http://mi.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://nd.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bg.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zn.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mr.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qj.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dz.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ka.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://if.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://wx.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yz.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pm.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dl.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zs.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wv.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zs.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cq.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dr.jianghongdianzi.cn

[J09] 时区处理
来源：http://ac.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bj.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qr.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iz.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wg.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qu.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://al.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dt.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://kc.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://te.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wt.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ni.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nq.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tc.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mh.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tv.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ho.nszjky.cn

================================================================================
来源：http://em.9csxet.cn

K. JSON 与序列化
来源：http://xw.shxzskj.cn

================================================================================
来源：http://td.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://qe.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://af.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ut.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://wo.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://nr.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kc.huanxung.cn

Go:   json.Marshal(obj)
来源：http://qr.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mc.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://in.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://wn.haigaiapp.cn

Py:   json.loads(s)
来源：http://bl.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uy.521024.cn

JS:   JSON.parse(s)
来源：http://sg.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://pq.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ev.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://lo.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://gc.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gp.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://km.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vn.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xp.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gx.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nx.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qm.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://et.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xd.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bh.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://bp.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ns.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qy.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fi.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yq.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ji.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://na.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://um.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ja.jctech888.com.cn

[K05] 深拷贝对象
来源：http://zh.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://wr.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://po.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://ym.szxytkj.cn

TS:   structuredClone(obj)
来源：http://my.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mo.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ef.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ug.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lv.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://fg.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eu.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wj.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lm.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qy.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wq.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hi.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ab.haigaiapp.cn


<!-- 参考信息 -->