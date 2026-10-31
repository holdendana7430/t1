代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://qy.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kr.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wg.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://px.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oq.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fz.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bd.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bz.hnjuh.cn

[H03] 主动抛出异常
来源：http://oe.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://oa.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xe.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://qh.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://bd.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zw.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mh.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bk.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jn.9csxet.cn

[H04] 自定义异常类型
来源：http://do.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://jm.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vp.521024.cn

JS:   class MyError extends Error {}
来源：http://kv.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://eo.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://wa.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lv.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://gu.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://if.newstarts.cn

[H05] 捕获特定类型
来源：http://sn.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://tn.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://he.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://qd.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://jl.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://gp.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qv.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ut.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rf.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://kv.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://or.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://og.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ga.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fq.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lh.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wg.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://xz.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://zk.jctech888.com.cn

[H07] 断言
来源：http://tl.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://cg.shxzskj.cn

PHP:  assert($x > 0);
来源：http://ge.szsharing.cn

JS:   console.assert(x > 0);
来源：http://iy.colortex.cn

TS:   console.assert(x > 0);
来源：http://xw.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://ja.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xs.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vf.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://og.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://kn.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://em.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://do.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mr.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wx.lnxyls.cn

Go:   err.Error()
来源：http://vv.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://zn.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://bk.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ur.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pw.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xd.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zw.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://md.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://av.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fe.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bd.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ik.szxytkj.cn

[H10] 资源自动释放
来源：http://uu.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rx.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mn.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://is.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ih.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lt.hahajie.cn

Go:   defer f.Close()
来源：http://yr.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kn.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oz.hnjuh.cn

================================================================================
来源：http://ul.shtwfgs.cn

I. 正则表达式
来源：http://dr.szsharing.cn

================================================================================
来源：http://ac.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://tw.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vz.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mx.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://vh.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://fd.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://my.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lv.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://iq.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iz.panjiajie.cn

[I02] 提取所有匹配
来源：http://xb.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://hf.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nj.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tb.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://sc.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yz.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xd.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://nv.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fp.hnjuh.cn

[I03] 提取捕获分组
来源：http://rj.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ar.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oo.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nh.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lr.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nw.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ef.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rf.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fe.gzmigu.cn

[I04] 正则替换
来源：http://eu.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yn.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ek.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kv.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wq.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dz.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nl.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ka.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nk.jctech888.com.cn

[I05] 按正则拆分
来源：http://xv.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dj.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xc.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://ya.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://gz.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://mf.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://he.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://la.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eh.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ca.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qw.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wg.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pe.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mu.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vi.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qf.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ss.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aa.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://ya.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ye.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tv.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iz.yuntaijiaju.cn

TS:   /error/gim
来源：http://cj.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fd.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://js.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://gf.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ei.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://sp.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ls.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ov.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jc.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ta.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qo.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://od.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://he.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gn.muxihuayi.cn

================================================================================
来源：http://yo.9csxet.cn

J. 日期与时间
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://so.hahajie.cn

[J01] 获取当前时间
来源：http://qt.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ya.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jk.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://fu.huanxung.cn

TS:   new Date();  Date.now()
来源：http://qw.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zl.jianghongdianzi.cn

Go:   time.Now()
来源：http://op.muxihuayi.cn

Ruby: Time.now
来源：http://mi.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nq.colortex.cn

[J02] 格式化输出
来源：http://vl.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dy.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lq.huixiangedu.cn

TS:   d.toISOString()
来源：http://co.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fe.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fu.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vh.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tw.shxzskj.cn

[J03] 字符串解析为日期
来源：http://ce.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vk.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hs.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://kn.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ok.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xr.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yb.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://zx.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ek.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://ng.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ao.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fd.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bl.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kc.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mn.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oa.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gc.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dq.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://hg.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ca.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wr.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jy.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://lw.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://se.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://yl.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ak.nicolike.cn

[J06] 计算两时间之差
来源：http://pz.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://kd.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://fh.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cw.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sa.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gp.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ia.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://oo.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://sm.huixiangedu.cn

[J07] 比较两个日期
来源：http://ms.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://ph.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pn.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ho.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tw.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xy.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yv.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pe.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://es.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ph.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zr.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uj.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jk.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gc.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nl.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cd.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yy.jctech888.com.cn

[J09] 时区处理
来源：http://yu.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fm.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qq.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ip.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://al.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eb.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zv.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lj.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://hd.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hv.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yh.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tu.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ut.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yw.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zw.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vj.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jy.521024.cn

================================================================================
来源：http://hb.shxzskj.cn

K. JSON 与序列化
来源：http://vv.yuexingan06.cn

================================================================================
来源：http://js.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://sw.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://un.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pk.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://el.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://al.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dl.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://bh.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kc.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ow.newstarts.cn

[K02] JSON 字符串转对象
来源：http://sm.shxzskj.cn

Py:   json.loads(s)
来源：http://tv.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pz.hnjuh.cn

JS:   JSON.parse(s)
来源：http://bx.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://nq.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wf.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://dv.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://cw.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xs.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://yr.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mv.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eg.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cg.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ua.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hb.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wb.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nv.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hk.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://te.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xn.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wp.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mv.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oo.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nt.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kx.nicolike.cn

[K05] 深拷贝对象
来源：http://rz.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://fv.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ag.521024.cn

JS:   structuredClone(obj)
来源：http://ns.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://ko.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cx.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ps.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pn.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dp.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://og.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bc.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xr.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://px.nicolike.cn


<!-- 参考信息 -->