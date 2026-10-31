代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://xi.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dk.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sb.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fo.shxzskj.cn

[H03] 主动抛出异常
来源：http://mj.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://qu.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ob.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://dt.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://yd.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wx.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bq.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://is.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://af.yuexingan06.cn

[H04] 自定义异常类型
来源：http://wy.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://dw.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sk.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://nf.hahajie.cn

TS:   class MyError extends Error {}
来源：http://ql.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://bp.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yf.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://jr.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://yx.szsharing.cn

[H05] 捕获特定类型
来源：http://ss.haigaiapp.cn

Py:   except ValueError as e:
来源：http://jp.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jb.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://qg.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://hj.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://uk.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dj.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://vm.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uw.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://rs.521024.cn

Py:   value = d.get("k") or default
来源：http://bi.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qc.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qn.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zz.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://np.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ce.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://yj.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://gt.huixinmuqiang.cn

[H07] 断言
来源：http://xv.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://fl.szxytkj.cn

PHP:  assert($x > 0);
来源：http://hx.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://rp.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://sx.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://xt.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cl.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://er.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://el.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://vt.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://qx.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://co.szsharing.cn

JS:   e.message;  e.stack
来源：http://oo.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gn.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fo.shtwfgs.cn

Go:   err.Error()
来源：http://ze.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ae.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://zk.haigaiapp.cn

[H09] 带错误码的异常
来源：http://br.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uu.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tx.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://na.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ud.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eq.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hf.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gd.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ax.shtwfgs.cn

[H10] 资源自动释放
来源：http://ay.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lq.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://td.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nt.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://av.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pp.9csxet.cn

Go:   defer f.Close()
来源：http://je.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nd.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bh.bjjhwx.cn

================================================================================
来源：http://fh.jianghongdianzi.cn

I. 正则表达式
来源：http://ym.hahajie.cn

================================================================================
来源：http://bi.hahajie.cn

[I01] 判断是否匹配
来源：http://bq.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gr.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hv.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://sq.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://eg.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jx.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fj.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://qz.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nv.newstarts.cn

[I02] 提取所有匹配
来源：http://xr.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://lt.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hs.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sk.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ys.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gb.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vw.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://fl.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pn.nszjky.cn

[I03] 提取捕获分组
来源：http://kj.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ky.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ao.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nj.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xz.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nf.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ni.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cc.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pn.gzmigu.cn

[I04] 正则替换
来源：http://nv.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fp.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hv.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rc.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mv.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gj.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mp.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uu.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jz.colortex.cn

[I05] 按正则拆分
来源：http://bp.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rk.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lu.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://qk.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gt.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://hy.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dg.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://az.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ej.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hl.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lq.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kq.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fk.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yz.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yb.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rq.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kg.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://th.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xa.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kq.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ha.jctech888.com.cn

TS:   /error/gim
来源：http://ez.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zt.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kf.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ka.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rg.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://za.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uc.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pi.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qo.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ey.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gy.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sr.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tx.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tb.szsharing.cn

================================================================================
来源：http://fn.nszjky.cn

J. 日期与时间
来源：http://de.lnxyls.cn

================================================================================
来源：http://to.asd995.cn

[J01] 获取当前时间
来源：http://mm.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pf.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bf.521024.cn

JS:   new Date();  Date.now()
来源：http://fm.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://st.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yo.huixinmuqiang.cn

Go:   time.Now()
来源：http://rk.chemitech.net.cn

Ruby: Time.now
来源：http://ct.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wa.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ur.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lj.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tz.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ye.huixiangedu.cn

TS:   d.toISOString()
来源：http://km.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cm.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ud.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xy.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hk.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://lh.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vm.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ph.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://vs.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://qi.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jn.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dj.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://mn.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qr.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://jd.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ec.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sj.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kp.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ci.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fx.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rc.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ep.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nz.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://vb.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://yt.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pt.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ni.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xt.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://cs.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yq.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ov.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://st.lnxyls.cn

[J06] 计算两时间之差
来源：http://ei.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://wm.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://re.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://of.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ak.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://za.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ld.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://py.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://ld.huixiangedu.cn

[J07] 比较两个日期
来源：http://tx.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://bj.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kp.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jc.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ml.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vi.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yf.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eu.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://uq.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://qv.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qp.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xg.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qp.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pm.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xv.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pf.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iu.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ez.gzmigu.cn

[J09] 时区处理
来源：http://wi.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vo.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ri.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ia.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kc.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nh.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fg.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dc.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mi.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://vb.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://os.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hx.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ve.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qh.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nt.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eh.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gh.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yw.szxytkj.cn

================================================================================
来源：http://wy.szxytkj.cn

K. JSON 与序列化
来源：http://or.colortex.cn

================================================================================
来源：http://ov.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://df.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qk.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mu.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://rc.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://su.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bt.szsharing.cn

Go:   json.Marshal(obj)
来源：http://wt.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ua.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vb.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://dn.nszjky.cn

Py:   json.loads(s)
来源：http://bo.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qm.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://rz.szxytkj.cn

TS:   JSON.parse(s)
来源：http://ng.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://az.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://jg.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://vx.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ng.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://gy.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://br.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aw.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://td.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://np.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iq.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sl.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ig.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pa.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://nv.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yt.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://po.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mn.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wh.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dm.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kd.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zg.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jm.bjjhwx.cn

[K05] 深拷贝对象
来源：http://hm.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://eo.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ka.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ky.panjiajie.cn

TS:   structuredClone(obj)
来源：http://wu.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ly.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hf.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tq.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xw.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://ru.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rc.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jd.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ji.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hc.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ta.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ub.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lo.newstarts.cn


<!-- 参考信息 -->