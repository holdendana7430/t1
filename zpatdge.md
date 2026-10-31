代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://bf.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ga.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vp.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qv.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ur.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://us.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hj.521024.cn

JS:   throw new Error("错误信息");
来源：http://dz.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://nv.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jz.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tx.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mx.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hd.521024.cn

[H04] 自定义异常类型
来源：http://dq.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://id.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://he.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://us.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://nt.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://hi.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://db.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://mm.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://eq.gzmigu.cn

[H05] 捕获特定类型
来源：http://eb.shxzskj.cn

Py:   except ValueError as e:
来源：http://tm.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ly.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ze.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://zf.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://cv.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oc.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://mb.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://px.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://ea.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://lr.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://no.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eb.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://an.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zl.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nh.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://he.521024.cn

C#:   obj?.A?.B ?? default
来源：http://qk.chemitech.net.cn

[H07] 断言
来源：http://ve.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://he.shxzukj.cn

PHP:  assert($x > 0);
来源：http://pi.colortex.cn

JS:   console.assert(x > 0);
来源：http://ad.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://nh.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://xm.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rj.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qh.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://az.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://bb.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://bw.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://an.lnxyls.cn

JS:   e.message;  e.stack
来源：http://dv.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ya.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iz.huixiangedu.cn

Go:   err.Error()
来源：http://bi.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://of.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://wr.bjjhwx.cn

[H09] 带错误码的异常
来源：http://hy.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nr.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uq.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://np.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://df.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xk.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gi.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://os.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yc.nszjky.cn

[H10] 资源自动释放
来源：http://px.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cw.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://up.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yk.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ov.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iv.szxytkj.cn

Go:   defer f.Close()
来源：http://fb.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hj.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yq.szsharing.cn

================================================================================
来源：http://yr.shxzukj.cn

I. 正则表达式
来源：http://nz.jianghongdianzi.cn

================================================================================
来源：http://cj.colortex.cn

[I01] 判断是否匹配
来源：http://tb.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hr.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jh.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ej.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://za.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dj.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://li.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://bw.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://px.szsharing.cn

[I02] 提取所有匹配
来源：http://vs.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://ra.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rn.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qz.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ns.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oi.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wr.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://rz.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wa.hahajie.cn

[I03] 提取捕获分组
来源：http://in.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iz.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ix.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kx.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jm.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vi.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rk.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vv.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qh.haigaiapp.cn

[I04] 正则替换
来源：http://km.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hc.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ua.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gj.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rz.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ep.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ak.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://of.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bp.9csxet.cn

[I05] 按正则拆分
来源：http://wr.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qv.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mr.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://zu.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://zn.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://ff.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gv.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jr.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ey.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://st.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://on.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mr.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zp.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ih.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jx.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bc.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tg.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cx.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://rn.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pu.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nl.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tj.hnjuh.cn

TS:   /error/gim
来源：http://cl.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ir.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vq.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://fi.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://al.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://yj.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jz.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cd.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lz.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bi.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aq.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jr.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bo.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ha.521024.cn

================================================================================
来源：http://ja.huixinmuqiang.cn

J. 日期与时间
来源：http://ry.shtwfgs.cn

================================================================================
来源：http://lj.shtwfgs.cn

[J01] 获取当前时间
来源：http://yf.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uw.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xf.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://ty.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://xm.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://po.lnxyls.cn

Go:   time.Now()
来源：http://hv.bjjhwx.cn

Ruby: Time.now
来源：http://bd.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ne.shxzukj.cn

[J02] 格式化输出
来源：http://ce.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://es.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://md.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gj.shxzskj.cn

TS:   d.toISOString()
来源：http://pw.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://st.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zf.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bo.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://dh.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://id.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pu.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://gv.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://lx.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pm.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dl.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://px.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://id.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://lw.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cu.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ds.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gz.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jy.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tg.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ye.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mh.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://km.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://kr.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://eb.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fs.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ml.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jv.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ib.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vv.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://kf.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kc.panjiajie.cn

[J06] 计算两时间之差
来源：http://oj.asd995.cn

Py:   (end - start).total_seconds()
来源：http://da.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://cc.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oo.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oi.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ep.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ei.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://in.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://lm.huixiangedu.cn

[J07] 比较两个日期
来源：http://yr.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://uk.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xh.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vu.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ql.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ph.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jp.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fw.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://fv.szsharing.cn

[J08] 提取年月日与星期
来源：http://bu.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ow.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ji.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://se.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tz.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rt.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ou.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vf.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cx.muxihuayi.cn

[J09] 时区处理
来源：http://at.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://av.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lj.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nu.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ig.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wl.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gj.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rf.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ob.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://qx.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rv.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ay.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tl.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fr.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zt.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mo.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zi.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vt.newstarts.cn

================================================================================
来源：http://vg.huixinmuqiang.cn

K. JSON 与序列化
来源：http://zh.jianghongdianzi.cn

================================================================================
来源：http://eo.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://dk.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zt.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dz.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://no.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://yh.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fp.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://qr.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ak.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://km.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://lp.haigaiapp.cn

Py:   json.loads(s)
来源：http://ek.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aa.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://tx.newstarts.cn

TS:   JSON.parse(s)
来源：http://dh.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vc.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://jh.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://fl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vb.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://rh.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bd.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bu.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sl.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://us.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hv.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ep.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rb.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hm.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://va.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cb.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://je.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uk.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fh.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sk.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gm.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vp.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vs.nszjky.cn

[K05] 深拷贝对象
来源：http://aj.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://bz.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://pw.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://kl.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://fi.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zg.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pt.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ia.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qk.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://mb.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uj.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pn.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zq.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fj.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zw.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rr.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tq.huixinmuqiang.cn


<!-- 参考信息 -->