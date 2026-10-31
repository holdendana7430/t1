代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://rr.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fb.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hm.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hi.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bm.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kl.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jz.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ec.newstarts.cn

[H03] 主动抛出异常
来源：http://hc.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://sc.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ga.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://nf.asd995.cn

TS:   throw new Error("错误信息");
来源：http://pi.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mq.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://go.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://or.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lb.szxytkj.cn

[H04] 自定义异常类型
来源：http://rt.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://fq.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qs.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://pg.521024.cn

TS:   class MyError extends Error {}
来源：http://mo.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://yb.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qk.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://oj.newstarts.cn

C#:   class MyException : Exception {}
来源：http://zh.szsharing.cn

[H05] 捕获特定类型
来源：http://iy.hahajie.cn

Py:   except ValueError as e:
来源：http://tl.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mx.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://vu.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://zz.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://ey.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://ot.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tw.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://sa.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://by.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yl.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pa.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kn.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gm.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sn.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://ud.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://wg.chemitech.net.cn

[H07] 断言
来源：http://lb.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://ih.asd995.cn

PHP:  assert($x > 0);
来源：http://bd.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://tk.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://oj.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://pj.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ay.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oy.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://se.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://ov.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://vn.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ng.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://hx.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ys.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hr.huanxung.cn

Go:   err.Error()
来源：http://xp.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://fh.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://vb.muxihuayi.cn

[H09] 带错误码的异常
来源：http://zs.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pl.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zp.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gu.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sr.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kn.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hm.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aa.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jf.hnjuh.cn

[H10] 资源自动释放
来源：http://ck.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pi.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ui.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ql.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uj.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://re.haigaiapp.cn

Go:   defer f.Close()
来源：http://pl.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bz.nszjky.cn

================================================================================
来源：http://bb.nicolike.cn

I. 正则表达式
来源：http://vw.yuntaijiaju.cn

================================================================================
来源：http://sj.shtwfgs.cn

[I01] 判断是否匹配
来源：http://dj.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bp.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://np.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://jb.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://lp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wy.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ph.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ls.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qh.newstarts.cn

[I02] 提取所有匹配
来源：http://ti.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://up.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ra.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://ci.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bh.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pk.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://ec.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zf.hnjuh.cn

[I03] 提取捕获分组
来源：http://yc.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tn.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vw.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ns.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yq.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bh.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ur.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bx.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lv.bjjhwx.cn

[I04] 正则替换
来源：http://gi.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zd.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ho.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eh.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rq.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rd.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iv.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uo.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://au.huanxung.cn

[I05] 按正则拆分
来源：http://dl.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nc.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jb.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://hy.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mo.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://eb.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://by.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pw.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ja.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bi.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zk.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ik.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://my.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fh.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rp.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kj.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sq.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sb.521024.cn

[I07] 忽略大小写与多行模式
来源：http://sc.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lx.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lh.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oq.shxzukj.cn

TS:   /error/gim
来源：http://xc.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ox.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kt.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://fg.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dy.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://xq.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ks.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ms.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zb.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ys.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oi.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bv.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ia.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tu.muxihuayi.cn

================================================================================
来源：http://db.bookmarksfly.cn

J. 日期与时间
来源：http://sp.huanxung.cn

================================================================================
来源：http://hy.huanxung.cn

[J01] 获取当前时间
来源：http://jn.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wg.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eo.9csxet.cn

JS:   new Date();  Date.now()
来源：http://ju.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://pp.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bt.yuexingan06.cn

Go:   time.Now()
来源：http://ti.shtwfgs.cn

Ruby: Time.now
来源：http://pj.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bh.panjiajie.cn

[J02] 格式化输出
来源：http://cx.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vi.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dg.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hq.shxzukj.cn

TS:   d.toISOString()
来源：http://mo.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nq.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yu.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cv.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sk.newstarts.cn

[J03] 字符串解析为日期
来源：http://xr.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iv.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qz.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://yz.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://fe.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hy.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ua.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://tb.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sv.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://xj.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ni.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eq.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xx.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fr.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rf.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yt.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jn.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wk.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://gs.521024.cn

Py:   now + timedelta(days=7)
来源：http://og.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://et.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lj.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://co.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nt.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://ci.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xk.szxytkj.cn

[J06] 计算两时间之差
来源：http://qd.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://fg.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://tr.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ej.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://it.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cw.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://al.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://ln.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://xh.nszjky.cn

[J07] 比较两个日期
来源：http://du.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://in.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xc.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zk.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rk.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pu.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xg.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qw.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ca.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://sa.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yv.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uo.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dm.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dj.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ty.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dt.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://he.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yl.gzmigu.cn

[J09] 时区处理
来源：http://jl.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://au.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://av.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yb.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ix.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://up.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eb.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lw.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://un.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://bn.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gu.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rz.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ey.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://si.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cz.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zh.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cf.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oz.panjiajie.cn

================================================================================
来源：http://gc.nicolike.cn

K. JSON 与序列化
来源：http://ze.szxytkj.cn

================================================================================
来源：http://lb.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://ts.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fg.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://vg.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://iz.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ky.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://jf.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ez.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pt.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://lm.huixiangedu.cn

Py:   json.loads(s)
来源：http://vf.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wu.nszjky.cn

JS:   JSON.parse(s)
来源：http://lu.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ap.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vq.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://tq.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://rl.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dz.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://jv.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bl.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gt.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://np.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ro.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://co.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://be.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ll.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cm.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://qn.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nc.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fp.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mp.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wx.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rh.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fp.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://as.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ak.hahajie.cn

[K05] 深拷贝对象
来源：http://rh.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ob.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://mv.hnjuh.cn

JS:   structuredClone(obj)
来源：http://ev.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://xv.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tp.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lo.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tx.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cw.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://ob.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yv.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oz.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jl.9csxet.cn


<!-- 参考信息 -->