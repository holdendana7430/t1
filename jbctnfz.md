代发 wailian999

[H03] 主动抛出异常
来源：http://gn.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://nd.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qg.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://hj.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://ec.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fl.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ic.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nb.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uy.9csxet.cn

[H04] 自定义异常类型
来源：http://fh.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://gx.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://me.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ie.colortex.cn

TS:   class MyError extends Error {}
来源：http://cn.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://ul.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://el.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://dr.huanxung.cn

C#:   class MyException : Exception {}
来源：http://zw.huanxung.cn

[H05] 捕获特定类型
来源：http://ir.shtwfgs.cn

Py:   except ValueError as e:
来源：http://yz.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ux.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://by.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://xx.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://ps.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pb.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://yh.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lx.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://yd.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://mp.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sy.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jb.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ed.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hs.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bh.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://lo.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://gk.nszjky.cn

[H07] 断言
来源：http://cf.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://fc.lnxyls.cn

PHP:  assert($x > 0);
来源：http://ur.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://du.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://ot.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://zp.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://it.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uv.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://os.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ol.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://pi.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xi.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://st.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tj.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qb.nszjky.cn

Go:   err.Error()
来源：http://za.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://xe.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://rj.newstarts.cn

[H09] 带错误码的异常
来源：http://ke.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qb.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qp.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xh.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rd.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://to.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ug.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ji.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wq.panjiajie.cn

[H10] 资源自动释放
来源：http://jr.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ip.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xl.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qw.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hr.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jl.huanxung.cn

Go:   defer f.Close()
来源：http://lx.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fk.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mp.bjjhwx.cn

================================================================================
来源：http://na.nicolike.cn

I. 正则表达式
来源：http://pp.bookmarksfly.cn

================================================================================
来源：http://xw.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://pu.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qv.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://nc.521024.cn

TS:   /\d+/.test(s)
来源：http://ax.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zs.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mq.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://hd.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tm.newstarts.cn

[I02] 提取所有匹配
来源：http://lh.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ul.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gv.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mf.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://fr.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yl.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sh.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://zq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ml.bjjhwx.cn

[I03] 提取捕获分组
来源：http://yc.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uy.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://go.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://up.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://za.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rp.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mr.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qk.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ya.szxytkj.cn

[I04] 正则替换
来源：http://nd.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hd.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hm.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ix.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mc.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iu.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ul.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ev.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fd.hnjuh.cn

[I05] 按正则拆分
来源：http://cv.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yy.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mt.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://il.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wq.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ti.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kv.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jw.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ys.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gz.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gq.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mt.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tt.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cj.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ox.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hq.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sd.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yw.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://ve.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lp.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lc.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ct.szsharing.cn

TS:   /error/gim
来源：http://yr.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://no.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sj.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://wp.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gd.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://by.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ei.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ce.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sp.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uz.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xu.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pu.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rl.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iz.521024.cn

================================================================================
来源：http://pd.jianghongdianzi.cn

J. 日期与时间
来源：http://al.hnjuh.cn

================================================================================
来源：http://lb.newstarts.cn

[J01] 获取当前时间
来源：http://uh.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zm.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pu.szsharing.cn

JS:   new Date();  Date.now()
来源：http://fq.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://nq.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cz.haigaiapp.cn

Go:   time.Now()
来源：http://tj.huixinmuqiang.cn

Ruby: Time.now
来源：http://kk.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qt.bjjhwx.cn

[J02] 格式化输出
来源：http://oc.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tk.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ye.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ru.newstarts.cn

TS:   d.toISOString()
来源：http://we.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jh.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bj.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vt.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ad.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://wc.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ku.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ah.asd995.cn

JS:   new Date("2024-01-02")
来源：http://xo.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://bc.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qt.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ht.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://pb.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sz.9csxet.cn

[J04] 时间戳与日期互转
来源：http://va.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ez.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tw.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kp.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://de.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pr.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ow.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cp.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aa.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://xz.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://ky.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ko.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nw.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vg.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://kc.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xw.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://eg.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lt.szsharing.cn

[J06] 计算两时间之差
来源：http://gj.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://cr.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://nw.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ax.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hu.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hh.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://ye.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hy.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://mf.nicolike.cn

[J07] 比较两个日期
来源：http://ch.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://im.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mu.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fb.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ek.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kf.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lq.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bn.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://kz.hahajie.cn

[J08] 提取年月日与星期
来源：http://wu.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fy.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ti.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zi.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ja.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://za.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bq.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://np.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ae.bookmarksfly.cn

[J09] 时区处理
来源：http://oc.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cl.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lr.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ol.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jk.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bs.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rh.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uy.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://pw.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pl.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pg.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rj.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xg.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ue.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ci.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tj.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cv.9csxet.cn

================================================================================
来源：http://dl.colortex.cn

K. JSON 与序列化
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://lj.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://vm.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eo.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mr.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://fv.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://kp.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gn.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://vw.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fm.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tv.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ei.hnjuh.cn

Py:   json.loads(s)
来源：http://lk.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gi.shxzukj.cn

JS:   JSON.parse(s)
来源：http://ab.gzmigu.cn

TS:   JSON.parse(s)
来源：http://yr.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ji.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://ov.hahajie.cn

Ruby: JSON.parse(s)
来源：http://im.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pn.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://rt.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pk.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ig.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wm.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bc.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sd.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wv.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://if.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://je.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ry.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fx.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ur.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://an.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://js.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xb.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ek.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jz.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://yu.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://sr.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://we.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ep.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://qw.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uf.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://su.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pt.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sl.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://tp.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oy.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fy.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yf.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lc.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jf.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://is.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sw.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yw.shtwfgs.cn

[K07] 进制转换
来源：http://fn.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kn.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ft.yuntaijiaju.cn


<!-- 参考信息 -->