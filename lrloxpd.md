代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://kk.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eo.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://km.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mv.shtwfgs.cn

[H03] 主动抛出异常
来源：http://xo.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://qw.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cv.asd995.cn

JS:   throw new Error("错误信息");
来源：http://hi.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://np.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mb.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ll.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lh.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rk.asd995.cn

[H04] 自定义异常类型
来源：http://xw.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://qm.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yh.colortex.cn

JS:   class MyError extends Error {}
来源：http://fn.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://lq.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://tr.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dy.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://uo.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://ix.521024.cn

[H05] 捕获特定类型
来源：http://ob.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://bt.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fa.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://is.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://hy.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://gb.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ji.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://oe.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ai.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ru.newstarts.cn

Py:   value = d.get("k") or default
来源：http://kv.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hm.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://md.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://em.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ed.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cz.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://gq.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://pj.newstarts.cn

[H07] 断言
来源：http://ys.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://zc.521024.cn

PHP:  assert($x > 0);
来源：http://ou.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://ah.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://zx.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://yf.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://db.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qc.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://xi.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://mz.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qr.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ga.nicolike.cn

JS:   e.message;  e.stack
来源：http://uk.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oa.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xu.asd995.cn

Go:   err.Error()
来源：http://fj.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://lr.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://wi.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://jy.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vx.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lo.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qa.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ji.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://su.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ay.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cd.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bz.panjiajie.cn

[H10] 资源自动释放
来源：http://ee.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nr.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://np.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wu.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ng.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kn.yuexingan06.cn

Go:   defer f.Close()
来源：http://cw.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xe.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lm.asd995.cn

================================================================================
来源：http://dj.shtwfgs.cn

I. 正则表达式
来源：http://fx.yuexingan06.cn

================================================================================
来源：http://er.lnxyls.cn

[I01] 判断是否匹配
来源：http://wc.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ys.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://de.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://py.newstarts.cn

TS:   /\d+/.test(s)
来源：http://jz.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mh.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hf.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://gt.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dw.nicolike.cn

[I02] 提取所有匹配
来源：http://lu.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://up.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sp.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ve.asd995.cn

TS:   s.match(/\d+/g)
来源：http://om.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mo.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://js.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://ky.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bp.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://oc.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pn.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lu.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pq.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gz.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dx.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aj.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rs.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ch.wgjwhj.cn

[I04] 正则替换
来源：http://wz.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ev.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://le.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xw.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ci.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wu.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sb.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tv.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wx.lnxyls.cn

[I05] 按正则拆分
来源：http://wc.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ru.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pm.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ij.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ly.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://wm.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lu.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tk.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ww.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kk.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fb.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vj.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pk.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tb.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iq.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mh.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://av.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://by.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://ny.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xt.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vp.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sw.bjjhwx.cn

TS:   /error/gim
来源：http://hy.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://al.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vi.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://zi.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zu.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://dh.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xy.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sy.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://di.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ni.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jv.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hu.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ky.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ii.hahajie.cn

================================================================================
来源：http://rt.haigaiapp.cn

J. 日期与时间
来源：http://cp.colortex.cn

================================================================================
来源：http://sh.bookmarksfly.cn

[J01] 获取当前时间
来源：http://rg.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://si.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ua.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://kt.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://nw.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gw.szxytkj.cn

Go:   time.Now()
来源：http://ac.jctech888.com.cn

Ruby: Time.now
来源：http://sh.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://in.szsharing.cn

[J02] 格式化输出
来源：http://qc.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cg.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sg.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wb.newstarts.cn

TS:   d.toISOString()
来源：http://dd.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ln.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fa.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nz.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wd.9csxet.cn

[J03] 字符串解析为日期
来源：http://mn.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vc.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rt.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://uc.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://gx.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yv.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pv.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://oh.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hv.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ha.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gf.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fq.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vp.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nh.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ho.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dx.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ow.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rx.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://jm.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://zw.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ln.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oj.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ru.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://bh.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ey.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://sp.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pc.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://jo.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://au.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://fe.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rc.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://se.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://do.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://yw.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://fj.chemitech.net.cn

[J07] 比较两个日期
来源：http://gx.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://oa.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yl.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cc.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eg.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://es.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wy.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cj.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://gr.hnjuh.cn

[J08] 提取年月日与星期
来源：http://yo.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ex.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://my.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://my.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lb.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sw.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hv.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vr.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://li.huanxung.cn

[J09] 时区处理
来源：http://hr.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sy.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dq.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sv.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pa.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vm.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dp.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gj.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ze.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://xt.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kx.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mr.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ts.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://la.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ec.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kz.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dz.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ck.shxzukj.cn

================================================================================
来源：http://uc.lnxyls.cn

K. JSON 与序列化
来源：http://ru.haigaiapp.cn

================================================================================
来源：http://ba.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://sp.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cu.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hf.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://cj.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ru.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xs.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://xj.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uu.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yl.nszjky.cn

[K02] JSON 字符串转对象
来源：http://xy.szxytkj.cn

Py:   json.loads(s)
来源：http://tc.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ji.panjiajie.cn

JS:   JSON.parse(s)
来源：http://pz.521024.cn

TS:   JSON.parse(s)
来源：http://bq.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kf.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://xa.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://fy.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ve.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://df.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fc.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lk.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://je.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kn.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fc.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tg.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://va.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rh.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://px.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gk.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vm.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rf.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nb.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cj.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yd.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ao.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ji.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://iz.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://uw.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://gd.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://gl.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://tb.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vq.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yy.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qv.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://be.huanxung.cn

[K06] 解析 URL 查询串
来源：http://sx.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xu.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jw.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://py.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yr.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yf.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sf.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vy.hahajie.cn


<!-- 参考信息 -->