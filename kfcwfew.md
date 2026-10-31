代发 wailian999

[H03] 主动抛出异常
来源：http://zs.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://kq.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ff.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://gt.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://mq.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vd.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://td.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fl.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xv.muxihuayi.cn

[H04] 自定义异常类型
来源：http://hq.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://wg.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zm.szsharing.cn

JS:   class MyError extends Error {}
来源：http://ww.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://lr.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ek.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vt.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://xw.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://og.wgjwhj.cn

[H05] 捕获特定类型
来源：http://uu.shxzskj.cn

Py:   except ValueError as e:
来源：http://hc.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bk.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ma.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://zh.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://nu.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ns.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://zx.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vb.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://jh.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ho.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://du.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xq.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qs.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ud.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://io.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://fu.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://ye.jctech888.com.cn

[H07] 断言
来源：http://sc.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://pq.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://vd.nicolike.cn

JS:   console.assert(x > 0);
来源：http://bq.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://tf.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://xf.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qp.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ip.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://lu.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://fd.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://pc.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ms.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://xi.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://at.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yp.bookmarksfly.cn

Go:   err.Error()
来源：http://dk.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://vl.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yf.shtwfgs.cn

[H09] 带错误码的异常
来源：http://lm.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qa.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fy.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lk.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iv.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mx.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ze.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uu.newstarts.cn

[H10] 资源自动释放
来源：http://jg.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mb.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xv.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rw.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yq.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fr.9csxet.cn

Go:   defer f.Close()
来源：http://if.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aq.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qw.newstarts.cn

================================================================================
来源：http://mh.szsharing.cn

I. 正则表达式
来源：http://ln.bjjhwx.cn

================================================================================
来源：http://ls.huanxung.cn

[I01] 判断是否匹配
来源：http://el.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ik.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ol.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://vo.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://da.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qc.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yj.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://ql.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rr.szxytkj.cn

[I02] 提取所有匹配
来源：http://au.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://am.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ls.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gg.asd995.cn

TS:   s.match(/\d+/g)
来源：http://km.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pt.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ky.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://mq.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gk.bjjhwx.cn

[I03] 提取捕获分组
来源：http://ur.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zf.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mi.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://of.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dz.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fs.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pq.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hh.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kj.asd995.cn

[I04] 正则替换
来源：http://fx.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://co.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sp.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lf.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kt.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ph.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mc.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hs.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xs.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://tr.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ah.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dq.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://bj.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://pf.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://qg.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lh.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ma.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fc.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pl.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gt.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gs.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ui.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sj.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dw.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uf.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bt.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ma.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bw.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mm.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qn.yuexingan06.cn

TS:   /error/gim
来源：http://nu.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gt.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tk.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://dy.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fy.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://wg.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rl.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ia.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rz.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yh.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ha.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mm.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gh.huanxung.cn

================================================================================
来源：http://kh.shxzskj.cn

J. 日期与时间
来源：http://dg.9csxet.cn

================================================================================
来源：http://mv.panjiajie.cn

[J01] 获取当前时间
来源：http://dz.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ar.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vb.huanxung.cn

JS:   new Date();  Date.now()
来源：http://hb.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://ig.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zb.huanxung.cn

Go:   time.Now()
来源：http://mo.shtwfgs.cn

Ruby: Time.now
来源：http://fb.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xq.colortex.cn

[J02] 格式化输出
来源：http://ol.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jb.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wc.shtwfgs.cn

TS:   d.toISOString()
来源：http://ru.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qv.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oy.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gp.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://nc.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vn.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hu.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://wq.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://gc.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ln.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://me.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://fz.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eu.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://hi.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mg.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vd.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wk.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yj.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nl.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pn.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bq.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nm.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://lq.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://xz.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ea.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jq.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dl.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://wi.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fx.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://vq.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kr.nszjky.cn

[J06] 计算两时间之差
来源：http://qu.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://mv.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://nb.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gz.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gi.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lv.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://sm.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://zy.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://jq.wgjwhj.cn

[J07] 比较两个日期
来源：http://hu.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://ti.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qb.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eg.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ci.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ik.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ad.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xq.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://aa.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ml.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gn.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xx.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pg.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qd.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ix.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aw.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fh.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cz.bjjhwx.cn

[J09] 时区处理
来源：http://ff.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rp.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ma.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eh.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mc.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bs.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yj.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ss.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://is.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ik.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mz.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://at.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ps.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mz.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://di.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jq.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nn.muxihuayi.cn

================================================================================
来源：http://zj.huixiangedu.cn

K. JSON 与序列化
来源：http://oi.huanxung.cn

================================================================================
来源：http://jl.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://oa.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jv.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zs.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://nd.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://jw.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bv.huanxung.cn

Go:   json.Marshal(obj)
来源：http://kt.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://im.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qe.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://zw.shxzskj.cn

Py:   json.loads(s)
来源：http://js.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bx.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://mt.newstarts.cn

TS:   JSON.parse(s)
来源：http://sp.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iy.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://cf.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://pf.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vd.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://sn.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wz.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://km.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pj.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cd.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ay.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fe.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wj.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://be.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ah.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qh.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qv.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ms.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kb.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zp.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://py.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ap.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://lr.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://nn.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://go.panjiajie.cn

JS:   structuredClone(obj)
来源：http://fh.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://oo.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pf.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gb.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://su.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fp.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://kz.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ft.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vd.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fu.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vv.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yp.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xr.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rq.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zx.szxytkj.cn

[K07] 进制转换
来源：http://ho.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xt.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xg.newstarts.cn


<!-- 参考信息 -->