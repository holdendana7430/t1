代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dx.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ol.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hw.huanxung.cn

[H02] finally / ensure 收尾
来源：http://hm.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gk.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cm.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://af.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ui.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cl.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oc.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ry.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oz.asd995.cn

[H03] 主动抛出异常
来源：http://et.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://ai.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ck.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://hf.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://nu.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ji.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ya.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ya.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ty.bjjhwx.cn

[H04] 自定义异常类型
来源：http://kf.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://of.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mp.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://yy.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://cs.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://fw.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ue.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://sh.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://dm.newstarts.cn

[H05] 捕获特定类型
来源：http://mo.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://qn.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://we.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://vk.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://px.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://wb.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dc.521024.cn

Ruby: rescue ArgumentError => e
来源：http://ob.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bq.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://bo.huanxung.cn

Py:   value = d.get("k") or default
来源：http://af.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bl.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://in.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rm.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://by.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fm.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://eg.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://er.hahajie.cn

[H07] 断言
来源：http://ho.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://pm.shxzskj.cn

PHP:  assert($x > 0);
来源：http://re.nicolike.cn

JS:   console.assert(x > 0);
来源：http://oh.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://vg.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://lj.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nl.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ht.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://cm.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://eq.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://yk.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tr.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://cd.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mk.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ld.chemitech.net.cn

Go:   err.Error()
来源：http://lk.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://gt.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://ko.9csxet.cn

[H09] 带错误码的异常
来源：http://xh.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://je.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qp.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ua.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jk.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yc.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lk.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nl.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gw.huanxung.cn

[H10] 资源自动释放
来源：http://tj.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ei.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qx.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ye.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qf.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://se.shxzskj.cn

Go:   defer f.Close()
来源：http://ue.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ez.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vc.szsharing.cn

================================================================================
来源：http://dt.panjiajie.cn

I. 正则表达式
来源：http://zv.nicolike.cn

================================================================================
来源：http://bx.colortex.cn

[I01] 判断是否匹配
来源：http://vg.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ls.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://on.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ou.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://vb.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lq.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xg.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://hj.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fb.521024.cn

[I02] 提取所有匹配
来源：http://rb.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://in.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ky.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vz.521024.cn

TS:   s.match(/\d+/g)
来源：http://er.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tz.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fh.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://xy.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dn.hnjuh.cn

[I03] 提取捕获分组
来源：http://mh.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ps.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ey.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ro.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gj.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rt.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hw.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://az.szsharing.cn

[I04] 正则替换
来源：http://nd.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://im.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zo.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nx.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yx.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xn.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uh.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wy.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sb.521024.cn

[I05] 按正则拆分
来源：http://du.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yz.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cv.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://jl.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://iq.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://dp.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tj.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bq.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vw.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://in.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fe.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qr.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qg.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yg.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xt.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nk.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rn.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://id.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://ox.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jp.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vg.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fa.panjiajie.cn

TS:   /error/gim
来源：http://xq.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wm.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ro.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://te.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vl.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://uq.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vk.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fv.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ot.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mx.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dq.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ts.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gj.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://by.szxytkj.cn

================================================================================
来源：http://st.bookmarksfly.cn

J. 日期与时间
来源：http://oq.szsharing.cn

================================================================================
来源：http://hj.newstarts.cn

[J01] 获取当前时间
来源：http://mr.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ip.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iw.hahajie.cn

JS:   new Date();  Date.now()
来源：http://tb.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://au.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vv.huixiangedu.cn

Go:   time.Now()
来源：http://ej.shtwfgs.cn

Ruby: Time.now
来源：http://xx.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://va.haigaiapp.cn

[J02] 格式化输出
来源：http://ly.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tn.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wv.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fn.9csxet.cn

TS:   d.toISOString()
来源：http://lu.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kl.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jv.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yj.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qn.9csxet.cn

[J03] 字符串解析为日期
来源：http://qx.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fa.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nq.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://pe.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://xl.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ia.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ce.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://fy.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qw.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://jl.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xi.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jj.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gu.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lm.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hm.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rb.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zr.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iy.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://jp.colortex.cn

Py:   now + timedelta(days=7)
来源：http://iy.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rx.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lq.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zk.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://zk.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://np.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ai.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ik.chemitech.net.cn

[J06] 计算两时间之差
来源：http://ij.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://id.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://qs.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://io.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ux.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pl.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://qx.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://wc.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://jk.haigaiapp.cn

[J07] 比较两个日期
来源：http://zs.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://te.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pr.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://na.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gy.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ll.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cz.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bq.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://ag.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://qg.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://es.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xm.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://no.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eq.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lx.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://db.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yw.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ir.jctech888.com.cn

[J09] 时区处理
来源：http://ke.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qj.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yu.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aq.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ak.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lv.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kz.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lh.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fy.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://wv.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ej.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://co.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pd.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ch.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vc.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sb.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fy.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nv.9csxet.cn

================================================================================
来源：http://zh.nicolike.cn

K. JSON 与序列化
来源：http://xm.bjjhwx.cn

================================================================================
来源：http://ja.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://sf.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gu.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://or.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ar.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://db.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nz.colortex.cn

Go:   json.Marshal(obj)
来源：http://ch.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xo.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dy.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://el.yuexingan06.cn

Py:   json.loads(s)
来源：http://qd.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yr.lnxyls.cn

JS:   JSON.parse(s)
来源：http://if.hnjuh.cn

TS:   JSON.parse(s)
来源：http://op.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qe.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://xb.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ry.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cw.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://wd.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nf.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ic.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wv.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cm.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ax.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dh.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gh.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vf.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://aa.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fh.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pg.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rn.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xc.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lk.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://br.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yn.huanxung.cn

[K05] 深拷贝对象
来源：http://er.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://je.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://tj.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://ku.shxzskj.cn

TS:   structuredClone(obj)
来源：http://ed.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wg.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qp.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hc.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cm.huanxung.cn


<!-- 参考信息 -->