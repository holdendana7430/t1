代发 wailian999

[H03] 主动抛出异常
来源：http://qx.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://oj.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wl.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://dq.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://xf.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ws.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wm.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uw.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qq.lnxyls.cn

[H04] 自定义异常类型
来源：http://dl.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://ui.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zm.szsharing.cn

JS:   class MyError extends Error {}
来源：http://gs.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://cu.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://jd.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hx.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://zy.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://im.asd995.cn

[H05] 捕获特定类型
来源：http://rj.colortex.cn

Py:   except ValueError as e:
来源：http://nq.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://px.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ti.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ys.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://dm.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bu.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://vs.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xa.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://os.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://xc.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oz.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gn.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://op.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://te.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tk.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://kx.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://bb.yuexingan06.cn

[H07] 断言
来源：http://sh.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://lb.colortex.cn

PHP:  assert($x > 0);
来源：http://su.szsharing.cn

JS:   console.assert(x > 0);
来源：http://yo.nicolike.cn

TS:   console.assert(x > 0);
来源：http://pl.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://jb.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cd.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rl.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://bx.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://cg.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://rc.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kz.hnjuh.cn

JS:   e.message;  e.stack
来源：http://ae.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hy.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://on.szsharing.cn

Go:   err.Error()
来源：http://hx.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://wh.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://me.hnjuh.cn

[H09] 带错误码的异常
来源：http://br.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yn.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ir.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cd.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ol.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pp.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yy.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://br.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lw.nicolike.cn

[H10] 资源自动释放
来源：http://hk.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rx.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nw.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xu.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iy.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wm.521024.cn

Go:   defer f.Close()
来源：http://cl.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ru.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xq.newstarts.cn

================================================================================
来源：http://gu.huixinmuqiang.cn

I. 正则表达式
来源：http://nb.nszjky.cn

================================================================================
来源：http://qi.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://lo.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ne.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fp.huanxung.cn

JS:   /\d+/.test(s)
来源：http://dt.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://bh.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sq.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cs.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://cp.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wk.shxzskj.cn

[I02] 提取所有匹配
来源：http://iz.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://dl.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cj.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pu.521024.cn

TS:   s.match(/\d+/g)
来源：http://yv.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zw.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ug.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://js.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zy.bjjhwx.cn

[I03] 提取捕获分组
来源：http://xv.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://la.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cc.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gx.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mp.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mm.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kv.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ur.bjjhwx.cn

[I04] 正则替换
来源：http://zz.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://as.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pc.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jo.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ac.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ax.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mn.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tj.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lp.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://xb.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nt.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cp.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qp.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://xi.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://tm.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qc.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nm.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dw.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pv.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nz.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fr.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ii.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dn.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://it.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aa.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cd.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://li.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pb.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ag.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kc.wgjwhj.cn

TS:   /error/gim
来源：http://sl.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jk.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pa.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://yn.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jv.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://pn.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rr.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yx.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nq.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nr.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qi.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rn.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tp.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rg.521024.cn

================================================================================
来源：http://sk.yuntaijiaju.cn

J. 日期与时间
来源：http://vd.jctech888.com.cn

================================================================================
来源：http://de.hnjuh.cn

[J01] 获取当前时间
来源：http://dt.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zh.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eh.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://rc.hahajie.cn

TS:   new Date();  Date.now()
来源：http://vk.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rs.hahajie.cn

Go:   time.Now()
来源：http://ic.newstarts.cn

Ruby: Time.now
来源：http://ew.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tk.wgjwhj.cn

[J02] 格式化输出
来源：http://mw.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vb.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mw.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qr.bookmarksfly.cn

TS:   d.toISOString()
来源：http://xl.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hf.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eu.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xd.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ej.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://cw.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vd.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mo.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://vu.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://jm.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lt.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gt.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://nk.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ei.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://do.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://os.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lg.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ye.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fd.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xg.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wz.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rj.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dn.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://bb.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://qw.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jr.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xc.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ps.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://qy.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://su.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ww.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pm.hahajie.cn

[J06] 计算两时间之差
来源：http://hx.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://lx.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://tb.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hs.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://za.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wu.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://rw.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://uz.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://wr.nszjky.cn

[J07] 比较两个日期
来源：http://aj.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://uj.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xu.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mi.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kd.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qw.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://na.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zl.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://vs.hnjuh.cn

[J08] 提取年月日与星期
来源：http://jn.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lp.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://th.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ms.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wq.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ek.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bm.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hy.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wp.colortex.cn

[J09] 时区处理
来源：http://kg.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gr.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cx.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eq.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tq.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gc.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ih.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://km.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rh.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://zs.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nc.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cc.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yj.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zm.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ck.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vd.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ax.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fy.wgjwhj.cn

================================================================================
来源：http://li.chemitech.net.cn

K. JSON 与序列化
来源：http://xr.chemitech.net.cn

================================================================================
来源：http://uc.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://mm.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nm.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vm.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://bc.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://qm.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kr.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://gl.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gq.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vm.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://zy.huixiangedu.cn

Py:   json.loads(s)
来源：http://nl.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gc.newstarts.cn

JS:   JSON.parse(s)
来源：http://ii.nicolike.cn

TS:   JSON.parse(s)
来源：http://ou.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ve.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://xy.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://kn.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tm.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://af.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ax.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oh.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ss.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qk.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xe.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qu.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yk.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oa.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ca.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wm.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vg.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zn.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hu.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ti.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tl.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://or.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iq.huanxung.cn

[K05] 深拷贝对象
来源：http://ec.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ov.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://uw.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ow.nszjky.cn

TS:   structuredClone(obj)
来源：http://bb.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gg.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://be.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zh.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tv.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://ex.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pd.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gx.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rs.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lf.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tk.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bg.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gh.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wj.lnxyls.cn

[K07] 进制转换
来源：http://ud.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xv.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wt.521024.cn


<!-- 参考信息 -->