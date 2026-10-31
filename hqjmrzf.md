代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hb.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rh.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sn.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://th.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fx.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pj.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sp.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nw.9csxet.cn

[H03] 主动抛出异常
来源：http://kd.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://es.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dw.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://tu.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://uy.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://es.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://la.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hr.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uc.huanxung.cn

[H04] 自定义异常类型
来源：http://jn.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://cf.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://px.huanxung.cn

JS:   class MyError extends Error {}
来源：http://xi.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://zr.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://vh.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ef.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://rh.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://ml.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://ss.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ph.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jq.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://iv.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://fh.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://mm.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ab.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://dy.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zn.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://qt.nszjky.cn

Py:   value = d.get("k") or default
来源：http://db.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lp.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cr.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dl.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ho.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qw.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://bb.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://nx.haigaiapp.cn

[H07] 断言
来源：http://ot.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://no.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://oz.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://jc.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://hk.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://pc.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yn.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mp.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://re.521024.cn

[H08] 获取错误信息与堆栈
来源：http://la.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://ih.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qc.nicolike.cn

JS:   e.message;  e.stack
来源：http://sc.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://br.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rq.huixinmuqiang.cn

Go:   err.Error()
来源：http://bk.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://sc.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://ff.hnjuh.cn

[H09] 带错误码的异常
来源：http://ma.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ep.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ro.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ic.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nk.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fp.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zu.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://su.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lc.asd995.cn

[H10] 资源自动释放
来源：http://yi.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qz.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://si.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://di.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kv.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kf.nicolike.cn

Go:   defer f.Close()
来源：http://uh.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kc.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://om.huixinmuqiang.cn

================================================================================
来源：http://gk.9csxet.cn

I. 正则表达式
来源：http://wj.szxytkj.cn

================================================================================
来源：http://ky.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://au.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pa.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ck.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://wm.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://yp.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cm.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ol.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ry.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yb.asd995.cn

[I02] 提取所有匹配
来源：http://rk.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://pr.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xo.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dh.521024.cn

TS:   s.match(/\d+/g)
来源：http://nc.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pe.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://la.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://co.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vt.wgjwhj.cn

[I03] 提取捕获分组
来源：http://uz.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://si.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vm.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xy.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tk.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xg.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lh.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tw.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yl.szsharing.cn

[I04] 正则替换
来源：http://by.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hr.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lb.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vq.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rz.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vi.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qd.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ju.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kb.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://rb.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pq.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jv.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://tc.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://yd.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://di.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ef.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ad.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mn.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qx.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qr.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wp.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eo.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vs.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sl.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fq.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pr.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://og.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wj.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://os.jianghongdianzi.cn

TS:   /error/gim
来源：http://vl.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wq.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ib.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://kl.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pj.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ce.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jo.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sd.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rh.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ou.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tx.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uc.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pb.huixiangedu.cn

================================================================================
来源：http://gi.yuntaijiaju.cn

J. 日期与时间
来源：http://jh.gzmigu.cn

================================================================================
来源：http://hd.newstarts.cn

[J01] 获取当前时间
来源：http://yp.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pu.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ce.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://of.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://fv.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iq.huixinmuqiang.cn

Go:   time.Now()
来源：http://ke.bookmarksfly.cn

Ruby: Time.now
来源：http://hz.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zt.nicolike.cn

[J02] 格式化输出
来源：http://dj.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zg.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nx.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://us.panjiajie.cn

TS:   d.toISOString()
来源：http://kb.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xq.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hg.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jr.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ii.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://ly.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wd.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ji.asd995.cn

JS:   new Date("2024-01-02")
来源：http://mj.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ci.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dm.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://de.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://cg.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tt.521024.cn

[J04] 时间戳与日期互转
来源：http://ly.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kr.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hd.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oa.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fg.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://va.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ud.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wt.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qu.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://mk.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://oh.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lo.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lm.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tj.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ad.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kp.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://qr.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zu.yuexingan06.cn

[J06] 计算两时间之差
来源：http://fc.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://us.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://qs.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://st.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oe.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://al.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://wf.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://du.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://il.huixiangedu.cn

[J07] 比较两个日期
来源：http://dm.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://nm.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://za.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vn.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fa.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cv.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ai.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zo.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ek.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://rm.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ha.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ha.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ol.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qr.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://np.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mg.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gi.nszjky.cn

[J09] 时区处理
来源：http://fb.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://to.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pi.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lp.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yx.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://us.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zs.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ks.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yb.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://sv.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kn.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://du.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bs.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://af.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ws.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zn.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vh.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://un.newstarts.cn

================================================================================
来源：http://xr.shxzskj.cn

K. JSON 与序列化
来源：http://je.yuntaijiaju.cn

================================================================================
来源：http://iv.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ob.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://md.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qw.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://yc.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://vw.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qo.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://ci.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hz.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ij.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://op.gzmigu.cn

Py:   json.loads(s)
来源：http://vi.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xq.szsharing.cn

JS:   JSON.parse(s)
来源：http://nc.gzmigu.cn

TS:   JSON.parse(s)
来源：http://zw.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://om.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://kf.asd995.cn

Ruby: JSON.parse(s)
来源：http://bf.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fv.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://pw.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gv.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fj.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://it.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://py.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bv.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ws.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rt.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wh.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://iw.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rh.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kz.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iu.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hd.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uy.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jv.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://on.huanxung.cn

[K05] 深拷贝对象
来源：http://gc.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://iz.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://lp.newstarts.cn

JS:   structuredClone(obj)
来源：http://hk.szsharing.cn

TS:   structuredClone(obj)
来源：http://bf.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sx.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://on.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rw.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dw.huanxung.cn

[K06] 解析 URL 查询串
来源：http://md.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yo.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fn.521024.cn


<!-- 参考信息 -->