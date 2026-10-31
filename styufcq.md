代发 wailian999

[H03] 主动抛出异常
来源：http://kj.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://hx.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dq.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://yd.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://va.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xp.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oy.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vk.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xh.asd995.cn

[H04] 自定义异常类型
来源：http://aw.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://et.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bw.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://xv.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://pe.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://fk.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bv.521024.cn

Ruby: class MyError < StandardError; end
来源：http://pe.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://ou.shxzskj.cn

[H05] 捕获特定类型
来源：http://jc.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ar.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oz.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://ga.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://qq.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://zc.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bm.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://qr.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://de.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://yx.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://wl.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xu.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tf.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dj.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vx.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kj.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://dk.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ni.huanxung.cn

[H07] 断言
来源：http://mh.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://lt.lnxyls.cn

PHP:  assert($x > 0);
来源：http://zf.asd995.cn

JS:   console.assert(x > 0);
来源：http://yn.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://ao.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://tm.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ew.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zj.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://ev.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://cn.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://lw.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ln.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://gs.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ue.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://td.521024.cn

Go:   err.Error()
来源：http://iz.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://vp.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://yj.huanxung.cn

[H09] 带错误码的异常
来源：http://tn.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dm.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rn.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ui.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eh.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kj.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gd.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bk.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lq.muxihuayi.cn

[H10] 资源自动释放
来源：http://mg.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://md.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wu.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fv.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wa.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tf.shxzskj.cn

Go:   defer f.Close()
来源：http://pd.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jj.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vo.lnxyls.cn

================================================================================
来源：http://xr.nszjky.cn

I. 正则表达式
来源：http://tz.szsharing.cn

================================================================================
来源：http://en.jctech888.com.cn

[I01] 判断是否匹配
来源：http://xw.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iy.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zw.huanxung.cn

JS:   /\d+/.test(s)
来源：http://no.huanxung.cn

TS:   /\d+/.test(s)
来源：http://bo.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ez.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sg.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://gj.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gl.szxytkj.cn

[I02] 提取所有匹配
来源：http://zp.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://lw.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ih.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kn.colortex.cn

TS:   s.match(/\d+/g)
来源：http://lc.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fc.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jy.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://dm.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://in.lnxyls.cn

[I03] 提取捕获分组
来源：http://ty.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dc.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dz.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xa.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fh.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rv.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zh.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zb.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://re.muxihuayi.cn

[I04] 正则替换
来源：http://om.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ze.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://br.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qj.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://us.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://je.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jy.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uk.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tv.huanxung.cn

[I05] 按正则拆分
来源：http://vu.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ru.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sn.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://gv.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://ug.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://wh.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ig.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://up.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uv.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gw.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://va.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mi.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://en.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zx.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tq.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hw.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lt.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ko.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://pa.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://et.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uu.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjjhwx.cn

TS:   /error/gim
来源：http://vf.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pg.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jw.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://mi.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sl.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ki.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fi.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qm.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qb.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qb.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ii.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sh.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rm.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cs.haigaiapp.cn

================================================================================
来源：http://nv.szsharing.cn

J. 日期与时间
来源：http://rj.shxzskj.cn

================================================================================
来源：http://ha.colortex.cn

[J01] 获取当前时间
来源：http://aq.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kw.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zt.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://jy.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://ir.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pj.hahajie.cn

Go:   time.Now()
来源：http://vp.yuntaijiaju.cn

Ruby: Time.now
来源：http://jm.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qs.521024.cn

[J02] 格式化输出
来源：http://ot.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://md.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nr.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xh.hnjuh.cn

TS:   d.toISOString()
来源：http://sn.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kf.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xp.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lv.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ck.gzmigu.cn

[J03] 字符串解析为日期
来源：http://qm.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mr.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wo.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://zv.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ad.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fh.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oj.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://hh.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xy.colortex.cn

[J04] 时间戳与日期互转
来源：http://za.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wj.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ye.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jt.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ye.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bq.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cl.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gn.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fl.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://qn.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://iy.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ty.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fu.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ni.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://qh.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vi.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://dd.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ij.huixiangedu.cn

[J06] 计算两时间之差
来源：http://rg.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://zn.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://aa.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://up.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sq.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kz.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://gl.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://vn.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://he.hahajie.cn

[J07] 比较两个日期
来源：http://cj.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://qx.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ti.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ga.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fz.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nq.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aw.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ig.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://nk.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qs.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qj.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hv.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nd.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://da.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ke.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nx.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kq.wgjwhj.cn

[J09] 时区处理
来源：http://nl.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ba.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mz.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cd.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ev.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ld.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gk.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gk.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://px.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://cm.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ik.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://in.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ap.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ke.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ve.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ks.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tg.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rl.panjiajie.cn

================================================================================
来源：http://xz.shtwfgs.cn

K. JSON 与序列化
来源：http://wi.nszjky.cn

================================================================================
来源：http://te.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://xj.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sa.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qh.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://nc.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://fz.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vl.huanxung.cn

Go:   json.Marshal(obj)
来源：http://pg.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gd.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://le.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ej.nicolike.cn

Py:   json.loads(s)
来源：http://dj.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fg.panjiajie.cn

JS:   JSON.parse(s)
来源：http://le.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://hc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://td.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://fr.hahajie.cn

Ruby: JSON.parse(s)
来源：http://bo.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yt.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://zy.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://so.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ik.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gc.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kf.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ol.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bz.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wp.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yk.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://da.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://le.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lx.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ak.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dj.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cm.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dn.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yr.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tn.haigaiapp.cn

[K05] 深拷贝对象
来源：http://iy.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ey.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://as.nicolike.cn

JS:   structuredClone(obj)
来源：http://hm.colortex.cn

TS:   structuredClone(obj)
来源：http://na.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://md.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yk.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fs.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ba.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://ui.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fa.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pd.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://om.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dc.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zx.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pn.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nt.shtwfgs.cn

[K07] 进制转换
来源：http://yh.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nz.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xf.bookmarksfly.cn


<!-- 参考信息 -->