代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://gv.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uz.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lt.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cq.shtwfgs.cn

[H03] 主动抛出异常
来源：http://rx.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://nj.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://of.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://fe.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://bd.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ei.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mj.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lp.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oc.szxytkj.cn

[H04] 自定义异常类型
来源：http://rg.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://ha.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qw.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://cz.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://us.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://jr.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fz.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://dw.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://yp.asd995.cn

[H05] 捕获特定类型
来源：http://zq.jctech888.com.cn

Py:   except ValueError as e:
来源：http://ve.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gn.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://bq.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://bp.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://la.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oi.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://bn.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lb.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://cz.nicolike.cn

Py:   value = d.get("k") or default
来源：http://bv.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pj.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wt.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mb.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ki.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fb.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://xl.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ci.hahajie.cn

[H07] 断言
来源：http://ls.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://jq.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://fz.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://rm.521024.cn

TS:   console.assert(x > 0);
来源：http://ku.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://fo.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qw.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hr.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://jc.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://dw.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://fg.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bp.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ur.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vi.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nx.shxzskj.cn

Go:   err.Error()
来源：http://rh.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://tt.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://lo.haigaiapp.cn

[H09] 带错误码的异常
来源：http://yc.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bd.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gj.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sm.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jg.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vj.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://el.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yg.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vu.yuexingan06.cn

[H10] 资源自动释放
来源：http://uq.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zs.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ij.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lo.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jg.chemitech.net.cn

Go:   defer f.Close()
来源：http://xb.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bv.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pu.shtwfgs.cn

================================================================================
来源：http://dz.szsharing.cn

I. 正则表达式
来源：http://yb.panjiajie.cn

================================================================================
来源：http://en.szsharing.cn

[I01] 判断是否匹配
来源：http://yf.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://li.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iy.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://cn.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://za.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zy.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ni.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://vv.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ba.lnxyls.cn

[I02] 提取所有匹配
来源：http://gw.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://of.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wu.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wg.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://jc.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bj.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://tz.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yq.nicolike.cn

[I03] 提取捕获分组
来源：http://gi.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nt.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jj.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wc.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yt.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qy.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://by.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://go.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ph.9csxet.cn

[I04] 正则替换
来源：http://al.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vq.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yf.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lo.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wu.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rv.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hx.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jr.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vo.asd995.cn

[I05] 按正则拆分
来源：http://lb.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yj.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ne.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://dr.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://xl.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://uc.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ix.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bs.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yp.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wd.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fu.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sw.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://su.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://en.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gq.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ei.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ck.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pz.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://we.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oo.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mw.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ud.lnxyls.cn

TS:   /error/gim
来源：http://fa.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hu.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hy.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://jf.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ml.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://uo.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ew.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rc.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zt.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fc.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zs.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ce.huixiangedu.cn

================================================================================
来源：http://xa.panjiajie.cn

J. 日期与时间
来源：http://gg.hnjuh.cn

================================================================================
来源：http://bp.haigaiapp.cn

[J01] 获取当前时间
来源：http://ws.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ty.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dw.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://sj.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://sp.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://da.chemitech.net.cn

Go:   time.Now()
来源：http://ir.nszjky.cn

Ruby: Time.now
来源：http://rq.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ze.szxytkj.cn

[J02] 格式化输出
来源：http://pu.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wy.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jt.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fo.huixiangedu.cn

TS:   d.toISOString()
来源：http://gj.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nm.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jh.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vu.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ix.hahajie.cn

[J03] 字符串解析为日期
来源：http://il.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mf.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jy.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://hb.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://wn.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ye.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yb.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://kr.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ju.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://wj.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sd.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://as.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vo.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://el.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yp.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mq.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gn.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iz.521024.cn

[J05] 时间加减（加 7 天）
来源：http://vj.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://yv.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://to.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zl.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ad.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ob.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gk.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://vv.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yx.jctech888.com.cn

[J06] 计算两时间之差
来源：http://ii.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://eq.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ro.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fa.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hh.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fa.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://rd.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://he.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://rl.newstarts.cn

[J07] 比较两个日期
来源：http://gs.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cv.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vn.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tg.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yv.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pd.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wl.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://lj.colortex.cn

[J08] 提取年月日与星期
来源：http://on.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hc.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tt.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rs.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tg.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mc.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cj.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ne.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ev.szxytkj.cn

[J09] 时区处理
来源：http://cd.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eu.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zk.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pa.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tq.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://al.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qu.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jp.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dn.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://ls.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tz.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qr.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vf.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dy.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://km.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tg.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xz.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.nszjky.cn

================================================================================
来源：http://wh.huixiangedu.cn

K. JSON 与序列化
来源：http://vw.shtwfgs.cn

================================================================================
来源：http://tn.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://yi.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pc.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mj.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://lc.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://ii.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://az.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://fg.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ek.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qa.nicolike.cn

[K02] JSON 字符串转对象
来源：http://xb.521024.cn

Py:   json.loads(s)
来源：http://iz.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://st.shxzukj.cn

JS:   JSON.parse(s)
来源：http://uh.shxzskj.cn

TS:   JSON.parse(s)
来源：http://ae.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fs.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://qz.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://qa.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ys.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://dd.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ml.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ar.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://di.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ml.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ch.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jn.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zm.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wb.colortex.cn

[K04] 读取 JSON 文件
来源：http://hp.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hv.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tq.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dl.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ky.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://km.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nh.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://se.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aa.shxzukj.cn

[K05] 深拷贝对象
来源：http://ok.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://sj.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://ws.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://gg.nicolike.cn

TS:   structuredClone(obj)
来源：http://tn.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mm.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aw.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qv.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wp.szsharing.cn

[K06] 解析 URL 查询串
来源：http://ov.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wc.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rb.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lr.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ks.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ki.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rz.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wa.panjiajie.cn


<!-- 参考信息 -->