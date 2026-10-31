代发 wailian999

[H03] 主动抛出异常
来源：http://zc.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://jr.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nd.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://co.asd995.cn

TS:   throw new Error("错误信息");
来源：http://ls.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fy.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ol.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jo.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fj.colortex.cn

[H04] 自定义异常类型
来源：http://ft.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://pu.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fm.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://td.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://cu.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://si.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mg.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ut.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://rk.521024.cn

[H05] 捕获特定类型
来源：http://fv.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://xr.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yz.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://pi.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://vl.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://py.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mg.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://ua.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://xe.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ua.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ls.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dh.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oq.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kq.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gl.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://pn.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://ma.wgjwhj.cn

[H07] 断言
来源：http://xn.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://mi.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://mh.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://fn.szsharing.cn

TS:   console.assert(x > 0);
来源：http://th.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://yp.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nc.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ga.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://zd.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://wq.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ke.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tz.shxzskj.cn

JS:   e.message;  e.stack
来源：http://cb.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yr.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dn.colortex.cn

Go:   err.Error()
来源：http://ou.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://dh.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://cw.asd995.cn

[H09] 带错误码的异常
来源：http://ry.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xt.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gj.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gs.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ti.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://me.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gh.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yr.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bw.bjjhwx.cn

[H10] 资源自动释放
来源：http://ka.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://we.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vb.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://go.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ow.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nc.newstarts.cn

Go:   defer f.Close()
来源：http://av.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nd.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zy.nicolike.cn

================================================================================
来源：http://is.hahajie.cn

I. 正则表达式
来源：http://nt.wgjwhj.cn

================================================================================
来源：http://mv.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://vb.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sn.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kx.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://sg.9csxet.cn

TS:   /\d+/.test(s)
来源：http://yy.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kw.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://us.521024.cn

Ruby: s.match?(/\d+/)
来源：http://on.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lp.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ph.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://rf.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dv.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hf.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://iv.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ec.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bu.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://su.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hi.haigaiapp.cn

[I03] 提取捕获分组
来源：http://tx.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wx.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rz.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jh.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yi.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ux.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wv.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mc.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ia.szsharing.cn

[I04] 正则替换
来源：http://mb.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ax.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gi.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sx.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yj.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ai.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ti.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ip.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yp.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://jy.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kg.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jp.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ia.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://dn.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://ir.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wt.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yi.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tl.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tk.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rh.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jy.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tq.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://au.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yh.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://su.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ef.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uj.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://ip.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bs.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xn.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bk.colortex.cn

TS:   /error/gim
来源：http://uf.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bv.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ic.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://li.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ly.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://uv.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ml.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://th.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zn.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fh.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xr.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kp.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lt.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wj.hnjuh.cn

================================================================================
来源：http://ch.szsharing.cn

J. 日期与时间
来源：http://zn.bookmarksfly.cn

================================================================================
来源：http://ec.shxzukj.cn

[J01] 获取当前时间
来源：http://vk.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ya.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://by.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://hl.nicolike.cn

TS:   new Date();  Date.now()
来源：http://pa.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ww.yuexingan06.cn

Go:   time.Now()
来源：http://rv.gzmigu.cn

Ruby: Time.now
来源：http://fb.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ya.jctech888.com.cn

[J02] 格式化输出
来源：http://xy.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nf.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vd.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pj.chemitech.net.cn

TS:   d.toISOString()
来源：http://zr.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gu.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wt.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bk.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ip.szsharing.cn

[J03] 字符串解析为日期
来源：http://dn.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gv.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wt.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ox.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://bo.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hp.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tk.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ao.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zj.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://kt.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cq.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ts.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dq.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kj.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wt.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pk.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://no.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sr.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://qq.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://ub.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://da.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ru.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://to.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://zs.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://va.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://pw.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sz.huanxung.cn

[J06] 计算两时间之差
来源：http://jx.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://la.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://fa.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xc.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hc.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hk.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://ex.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://sn.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://vf.asd995.cn

[J07] 比较两个日期
来源：http://zy.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://fb.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qv.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tb.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://re.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ff.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fr.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ue.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zb.newstarts.cn

[J08] 提取年月日与星期
来源：http://tw.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qp.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ne.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hp.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xq.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ke.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tg.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xm.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pi.huixiangedu.cn

[J09] 时区处理
来源：http://fw.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zq.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zl.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://la.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tv.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fa.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fe.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://of.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rx.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://so.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lh.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://na.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tb.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fo.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ym.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://al.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qn.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aj.lnxyls.cn

================================================================================
来源：http://uw.nicolike.cn

K. JSON 与序列化
来源：http://rj.bookmarksfly.cn

================================================================================
来源：http://ui.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://bu.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vw.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lw.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://dt.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://et.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rs.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://jb.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xi.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cb.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://rh.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://bk.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nj.hnjuh.cn

JS:   JSON.parse(s)
来源：http://nq.newstarts.cn

TS:   JSON.parse(s)
来源：http://yh.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ul.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://rq.521024.cn

Ruby: JSON.parse(s)
来源：http://ag.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ug.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://tc.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ur.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yp.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://az.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ci.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yw.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hl.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xo.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mh.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ea.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gz.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fx.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cj.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rh.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iu.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nc.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oo.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://if.lnxyls.cn

[K05] 深拷贝对象
来源：http://vu.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://jw.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://jr.asd995.cn

JS:   structuredClone(obj)
来源：http://fl.huanxung.cn

TS:   structuredClone(obj)
来源：http://un.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ov.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://je.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wd.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mc.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://rw.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qu.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://in.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zf.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vy.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vb.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kf.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://af.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://id.chemitech.net.cn

[K07] 进制转换
来源：http://lv.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gy.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ko.9csxet.cn


<!-- 参考信息 -->