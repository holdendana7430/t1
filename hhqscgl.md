代发 wailian999

[H03] 主动抛出异常
来源：http://jl.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://qh.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yf.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://kg.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://fr.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yh.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fw.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yq.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oz.shxzskj.cn

[H04] 自定义异常类型
来源：http://tx.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://rx.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oo.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://kc.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://yt.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://un.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vu.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://kn.nszjky.cn

C#:   class MyException : Exception {}
来源：http://pj.shxzskj.cn

[H05] 捕获特定类型
来源：http://nf.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://rb.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ts.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://qr.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ky.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://wd.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kg.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://hm.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ky.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://dm.colortex.cn

Py:   value = d.get("k") or default
来源：http://ov.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rl.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mm.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ey.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qf.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://op.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://tc.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://kw.521024.cn

[H07] 断言
来源：http://iw.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://qb.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://bc.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://mr.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://mb.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://vp.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fz.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yt.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://vd.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://jk.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://ev.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vr.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://yi.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wo.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bf.yuntaijiaju.cn

Go:   err.Error()
来源：http://mu.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://sg.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://mf.asd995.cn

[H09] 带错误码的异常
来源：http://yr.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://is.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jt.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ie.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yx.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uk.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vf.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eg.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tg.yuexingan06.cn

[H10] 资源自动释放
来源：http://mp.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ji.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ih.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ik.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mt.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dg.wgjwhj.cn

Go:   defer f.Close()
来源：http://br.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wf.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://he.bookmarksfly.cn

================================================================================
来源：http://id.9csxet.cn

I. 正则表达式
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://bt.muxihuayi.cn

[I01] 判断是否匹配
来源：http://wq.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yv.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yu.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://cc.asd995.cn

TS:   /\d+/.test(s)
来源：http://ga.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ac.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rr.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://ge.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://of.bjjhwx.cn

[I02] 提取所有匹配
来源：http://la.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://jl.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hx.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://un.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://rn.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vp.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://io.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://ou.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ab.colortex.cn

[I03] 提取捕获分组
来源：http://cx.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vl.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ch.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ct.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mk.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ge.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pr.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xo.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tk.gzmigu.cn

[I04] 正则替换
来源：http://oi.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zr.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oy.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wf.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zy.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qa.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cj.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nu.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dd.hahajie.cn

[I05] 按正则拆分
来源：http://hv.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tv.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ve.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://yc.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mf.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://yg.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://in.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dz.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pj.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uz.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ig.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://an.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gi.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gk.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://im.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dt.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://as.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://pu.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mu.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uk.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vq.gzmigu.cn

TS:   /error/gim
来源：http://rm.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fj.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zb.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://pi.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ll.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://su.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hr.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dd.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://he.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gh.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ws.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lc.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fy.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://to.szxytkj.cn

================================================================================
来源：http://hy.hnjuh.cn

J. 日期与时间
来源：http://xe.asd995.cn

================================================================================
来源：http://qi.nicolike.cn

[J01] 获取当前时间
来源：http://mn.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nj.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mh.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://lz.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ei.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wl.szsharing.cn

Go:   time.Now()
来源：http://ps.shxzukj.cn

Ruby: Time.now
来源：http://qg.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ha.gzmigu.cn

[J02] 格式化输出
来源：http://li.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rw.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xg.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fz.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://wl.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://de.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rp.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gp.asd995.cn

[J03] 字符串解析为日期
来源：http://wi.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://up.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gy.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://az.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://lh.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pk.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gy.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://uu.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jd.nszjky.cn

[J04] 时间戳与日期互转
来源：http://do.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eq.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kv.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ao.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ue.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yf.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jr.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ju.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ri.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://an.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://pi.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rv.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uu.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bh.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://xj.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ga.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://il.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bs.jctech888.com.cn

[J06] 计算两时间之差
来源：http://yz.521024.cn

Py:   (end - start).total_seconds()
来源：http://up.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://fh.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ms.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vl.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yk.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://hd.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://om.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://sb.nszjky.cn

[J07] 比较两个日期
来源：http://fi.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://aj.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sj.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ee.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://io.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rs.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uw.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fj.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://jx.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ni.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mg.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hm.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hu.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pn.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ar.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bd.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://em.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fv.hnjuh.cn

[J09] 时区处理
来源：http://ig.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yp.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ts.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vg.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sl.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ze.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xt.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vq.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vq.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://bf.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mi.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ec.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://de.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rp.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uq.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nn.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zc.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jk.huanxung.cn

================================================================================
来源：http://pr.muxihuayi.cn

K. JSON 与序列化
来源：http://od.jianghongdianzi.cn

================================================================================
来源：http://pd.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://qi.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ff.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yc.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://tt.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://em.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rd.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://zp.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ev.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jr.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://et.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://tw.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zd.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://hy.hnjuh.cn

TS:   JSON.parse(s)
来源：http://wf.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pt.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ae.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://td.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cj.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://tv.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ec.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vh.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jo.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ik.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hf.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pl.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pr.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cg.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://as.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ul.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fe.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qj.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fp.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rl.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wt.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ku.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ld.shxzskj.cn

[K05] 深拷贝对象
来源：http://tb.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://em.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ar.newstarts.cn

TS:   structuredClone(obj)
来源：http://ye.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ui.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://it.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ah.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uq.521024.cn

[K06] 解析 URL 查询串
来源：http://kb.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mu.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fy.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qo.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mz.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://et.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tn.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bc.9csxet.cn

[K07] 进制转换
来源：http://oh.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ie.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vy.szxytkj.cn


<!-- 参考信息 -->