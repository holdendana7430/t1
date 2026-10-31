代发 wailian999

[H03] 主动抛出异常
来源：http://vr.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://qu.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yv.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ie.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://gu.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cw.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xh.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ib.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qo.szxytkj.cn

[H04] 自定义异常类型
来源：http://mn.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://ys.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ap.521024.cn

JS:   class MyError extends Error {}
来源：http://io.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://as.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://rd.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zd.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://bx.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://ir.jctech888.com.cn

[H05] 捕获特定类型
来源：http://eb.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://xs.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mr.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ac.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://nc.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://vv.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ra.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://tn.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qc.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://xs.nicolike.cn

Py:   value = d.get("k") or default
来源：http://as.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iv.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://st.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://go.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://us.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ic.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ha.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://iv.huixiangedu.cn

[H07] 断言
来源：http://yz.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://vx.szxytkj.cn

PHP:  assert($x > 0);
来源：http://em.asd995.cn

JS:   console.assert(x > 0);
来源：http://ek.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ey.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://eq.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kx.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cc.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://ik.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://jk.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://kh.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xo.lnxyls.cn

JS:   e.message;  e.stack
来源：http://jj.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zq.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vg.lnxyls.cn

Go:   err.Error()
来源：http://fj.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://ng.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://zb.colortex.cn

[H09] 带错误码的异常
来源：http://wg.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jk.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gs.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dk.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mn.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nj.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mb.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cj.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ag.szsharing.cn

[H10] 资源自动释放
来源：http://nu.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vl.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ek.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uw.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ji.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ml.hahajie.cn

Go:   defer f.Close()
来源：http://sw.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ro.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tj.shxzskj.cn

================================================================================
来源：http://th.yuntaijiaju.cn

I. 正则表达式
来源：http://th.newstarts.cn

================================================================================
来源：http://gi.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://vi.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vs.9csxet.cn

JS:   /\d+/.test(s)
来源：http://oq.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://qa.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vy.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fs.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://fa.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ps.shtwfgs.cn

[I02] 提取所有匹配
来源：http://vi.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://vh.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ab.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kh.asd995.cn

TS:   s.match(/\d+/g)
来源：http://wr.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jf.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://qh.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oq.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://qh.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://av.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://la.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tc.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://im.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ja.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xa.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yz.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hy.gzmigu.cn

[I04] 正则替换
来源：http://vu.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lp.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ci.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://om.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vc.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wx.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aa.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kw.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zj.bjjhwx.cn

[I05] 按正则拆分
来源：http://eh.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zi.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://zi.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://nr.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://sz.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nv.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yj.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oz.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pc.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://se.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qt.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ma.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sb.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gt.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sc.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ym.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iq.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://or.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cr.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uj.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uk.jianghongdianzi.cn

TS:   /error/gim
来源：http://qq.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ks.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bz.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://zn.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zr.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://mc.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ss.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ei.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://md.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ob.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://br.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jg.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cx.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nm.nicolike.cn

================================================================================
来源：http://gp.colortex.cn

J. 日期与时间
来源：http://kp.yuexingan06.cn

================================================================================
来源：http://ek.nicolike.cn

[J01] 获取当前时间
来源：http://bq.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pd.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dl.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://is.hahajie.cn

TS:   new Date();  Date.now()
来源：http://nu.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wj.jianghongdianzi.cn

Go:   time.Now()
来源：http://qx.nicolike.cn

Ruby: Time.now
来源：http://zx.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ni.521024.cn

[J02] 格式化输出
来源：http://oi.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tv.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dl.bookmarksfly.cn

TS:   d.toISOString()
来源：http://re.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ol.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fv.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bn.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dp.hnjuh.cn

[J03] 字符串解析为日期
来源：http://fl.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ve.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://al.asd995.cn

JS:   new Date("2024-01-02")
来源：http://nn.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://zs.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ip.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zg.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://lz.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xu.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://th.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wc.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://si.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ir.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qi.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://js.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zw.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dk.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://am.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://ff.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://xk.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yb.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ef.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gs.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ht.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wy.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://if.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ob.chemitech.net.cn

[J06] 计算两时间之差
来源：http://lj.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ep.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://ai.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nf.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rr.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nn.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://xc.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://re.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://yq.muxihuayi.cn

[J07] 比较两个日期
来源：http://oh.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://ev.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cm.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://km.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ng.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lx.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lu.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vv.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://ke.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://vq.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uv.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://br.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ps.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ts.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ju.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ib.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fl.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hd.hahajie.cn

[J09] 时区处理
来源：http://ue.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xm.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://at.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ao.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://he.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://um.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nk.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jh.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ly.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://lq.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gi.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ls.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ki.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yo.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xq.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gv.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sk.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zz.shtwfgs.cn

================================================================================
来源：http://ky.nicolike.cn

K. JSON 与序列化
来源：http://rx.szsharing.cn

================================================================================
来源：http://fj.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://vu.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qh.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zr.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://nb.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://jx.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yv.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://kn.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pf.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wi.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://av.hnjuh.cn

Py:   json.loads(s)
来源：http://xp.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vp.panjiajie.cn

JS:   JSON.parse(s)
来源：http://op.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://xh.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vm.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://jb.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://gu.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://on.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://fv.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ya.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mo.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jq.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yl.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rh.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kc.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pm.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ub.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://or.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tf.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sb.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://si.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kc.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ik.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eq.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ij.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xt.muxihuayi.cn

[K05] 深拷贝对象
来源：http://bn.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://xo.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://fn.huanxung.cn

JS:   structuredClone(obj)
来源：http://ow.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://jn.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://in.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bw.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wd.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tw.nicolike.cn

[K06] 解析 URL 查询串
来源：http://bo.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iy.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ry.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sj.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rd.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zq.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bq.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dn.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jv.gzmigu.cn

[K07] 进制转换
来源：http://lb.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://en.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wt.chemitech.net.cn


<!-- 参考信息 -->