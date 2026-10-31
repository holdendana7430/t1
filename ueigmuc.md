代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://kn.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pg.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bl.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mz.wgjwhj.cn

[H03] 主动抛出异常
来源：http://sj.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://av.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yr.521024.cn

JS:   throw new Error("错误信息");
来源：http://rx.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://lb.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zy.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cr.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dc.hnjuh.cn

[H04] 自定义异常类型
来源：http://be.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://jo.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ct.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ml.9csxet.cn

TS:   class MyError extends Error {}
来源：http://vv.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://vm.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gq.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://gy.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://ze.newstarts.cn

[H05] 捕获特定类型
来源：http://tg.szsharing.cn

Py:   except ValueError as e:
来源：http://vi.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cc.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://ob.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://to.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://op.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ri.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://es.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rh.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://ag.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://zz.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kl.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ae.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bc.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kl.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vs.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ld.521024.cn

C#:   obj?.A?.B ?? default
来源：http://vs.shtwfgs.cn

[H07] 断言
来源：http://xs.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ry.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://ss.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://fh.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://dm.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://fi.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wp.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cs.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://qq.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://wj.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://xs.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ax.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://qu.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mt.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://id.gzmigu.cn

Go:   err.Error()
来源：http://pz.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://qq.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://fx.haigaiapp.cn

[H09] 带错误码的异常
来源：http://nd.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kx.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ro.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://db.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fc.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uj.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rx.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gk.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zz.hnjuh.cn

[H10] 资源自动释放
来源：http://co.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pw.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iz.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qm.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wl.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dt.huixiangedu.cn

Go:   defer f.Close()
来源：http://mg.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rh.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ao.huanxung.cn

================================================================================
来源：http://yb.huixinmuqiang.cn

I. 正则表达式
来源：http://vy.hnjuh.cn

================================================================================
来源：http://cn.asd995.cn

[I01] 判断是否匹配
来源：http://co.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ti.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nc.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://gs.szsharing.cn

TS:   /\d+/.test(s)
来源：http://da.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gx.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pw.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://bp.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ka.szsharing.cn

[I02] 提取所有匹配
来源：http://ah.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://wd.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://au.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kn.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://bp.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ge.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pf.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://yo.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://se.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://qv.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bg.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yg.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qe.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ga.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wd.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rl.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rh.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kl.haigaiapp.cn

[I04] 正则替换
来源：http://pf.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jr.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sr.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bt.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ea.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bs.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ue.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ae.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vv.gzmigu.cn

[I05] 按正则拆分
来源：http://bu.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://is.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cf.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://zb.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://fm.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://fj.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sa.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pf.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://au.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fw.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hw.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nd.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://np.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uw.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ar.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ic.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jv.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hy.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://si.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://df.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zk.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mz.panjiajie.cn

TS:   /error/gim
来源：http://sn.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vr.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gc.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://kq.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vb.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://fy.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dh.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ws.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://de.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ej.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wv.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://po.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://je.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zr.szxytkj.cn

================================================================================
来源：http://rx.szsharing.cn

J. 日期与时间
来源：http://bi.shxzukj.cn

================================================================================
来源：http://fm.shxzukj.cn

[J01] 获取当前时间
来源：http://sa.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://av.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ye.hahajie.cn

JS:   new Date();  Date.now()
来源：http://pi.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://up.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ec.szsharing.cn

Go:   time.Now()
来源：http://ae.szxytkj.cn

Ruby: Time.now
来源：http://wq.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nc.haigaiapp.cn

[J02] 格式化输出
来源：http://tc.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://im.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dq.jctech888.com.cn

TS:   d.toISOString()
来源：http://st.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ch.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bx.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hm.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://um.nszjky.cn

[J03] 字符串解析为日期
来源：http://my.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tu.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tf.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://nr.521024.cn

TS:   new Date("2024-01-02")
来源：http://yy.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gc.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oa.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://in.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yj.colortex.cn

[J04] 时间戳与日期互转
来源：http://my.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ix.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tm.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fr.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vb.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qk.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dh.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rw.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pw.521024.cn

[J05] 时间加减（加 7 天）
来源：http://oj.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://dd.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ak.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lt.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qf.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://gc.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ag.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://zn.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fe.szsharing.cn

[J06] 计算两时间之差
来源：http://ha.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://rn.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ft.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wq.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qw.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vz.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://es.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://wn.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ap.panjiajie.cn

[J07] 比较两个日期
来源：http://uo.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://dw.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ud.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kg.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vk.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fj.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xe.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sl.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://pv.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://aa.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gt.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lk.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tc.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gq.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ck.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nq.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fr.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kq.szsharing.cn

[J09] 时区处理
来源：http://sk.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tu.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zf.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bg.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tl.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qx.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ni.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jh.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vg.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://bx.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vy.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://br.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dq.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ur.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qp.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nu.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ud.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xg.yuexingan06.cn

================================================================================
来源：http://ke.szsharing.cn

K. JSON 与序列化
来源：http://lx.nicolike.cn

================================================================================
来源：http://ha.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ur.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ip.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nb.asd995.cn

JS:   JSON.stringify(obj)
来源：http://zx.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://fv.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fy.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://tl.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mp.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lu.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://qy.nicolike.cn

Py:   json.loads(s)
来源：http://qw.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yg.shxzskj.cn

JS:   JSON.parse(s)
来源：http://jp.shxzukj.cn

TS:   JSON.parse(s)
来源：http://my.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dm.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://ya.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ry.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vd.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ja.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bd.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jv.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cq.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ln.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ve.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ir.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://om.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cw.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://mt.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hc.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://to.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rb.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cs.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fg.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://th.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uo.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://oi.521024.cn

Py:   copy.deepcopy(obj)
来源：http://oc.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ih.hahajie.cn

JS:   structuredClone(obj)
来源：http://lt.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://mc.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pa.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iy.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cx.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fj.newstarts.cn

[K06] 解析 URL 查询串
来源：http://rs.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bk.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pv.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fk.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vo.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eb.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xb.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vu.jctech888.com.cn


<!-- 参考信息 -->