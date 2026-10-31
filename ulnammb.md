代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nn.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ye.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jj.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://xy.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jr.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cy.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lb.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ol.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jc.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://db.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pg.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qz.lnxyls.cn

[H03] 主动抛出异常
来源：http://fj.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://bk.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://px.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://zw.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://zj.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qd.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pr.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xy.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cx.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://oo.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://qt.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nh.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ys.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://el.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://yw.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rw.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://uh.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://nc.muxihuayi.cn

[H05] 捕获特定类型
来源：http://ns.jctech888.com.cn

Py:   except ValueError as e:
来源：http://nw.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lb.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://nf.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://oi.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://pb.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://es.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://bt.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ly.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://fc.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://wy.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yk.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ou.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hn.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gh.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rf.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://fu.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://bv.lnxyls.cn

[H07] 断言
来源：http://ob.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://sv.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://gg.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://ln.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://du.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://jt.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qc.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ql.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://yh.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://vo.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://fd.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wm.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://yc.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xe.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ye.jctech888.com.cn

Go:   err.Error()
来源：http://cp.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://nw.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://fq.panjiajie.cn

[H09] 带错误码的异常
来源：http://hn.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xh.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ew.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ry.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uw.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bt.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wg.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zz.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yb.haigaiapp.cn

[H10] 资源自动释放
来源：http://en.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fi.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fd.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ce.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ua.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vd.szxytkj.cn

Go:   defer f.Close()
来源：http://gz.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yw.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://um.9csxet.cn

================================================================================
来源：http://pr.bookmarksfly.cn

I. 正则表达式
来源：http://xz.521024.cn

================================================================================
来源：http://df.jctech888.com.cn

[I01] 判断是否匹配
来源：http://fr.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pe.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ry.nicolike.cn

JS:   /\d+/.test(s)
来源：http://na.9csxet.cn

TS:   /\d+/.test(s)
来源：http://so.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://un.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ql.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fa.gzmigu.cn

[I02] 提取所有匹配
来源：http://zx.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://bn.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hw.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://gt.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gr.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zz.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://xp.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lf.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ei.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jd.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qt.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wk.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wi.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ei.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ua.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fc.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dc.shxzskj.cn

[I04] 正则替换
来源：http://bi.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cz.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ou.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zz.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lf.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tz.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uq.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fe.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vy.shxzukj.cn

[I05] 按正则拆分
来源：http://ug.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mb.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tq.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://is.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://js.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://ey.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wz.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://im.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gw.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ql.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vx.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sl.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ut.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qd.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bw.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pc.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://et.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ys.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://kd.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://md.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lj.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mo.shxzukj.cn

TS:   /error/gim
来源：http://nk.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qi.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sv.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://jz.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ho.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://vk.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ce.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yd.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jw.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://re.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lv.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jo.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lz.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nd.yuntaijiaju.cn

================================================================================
来源：http://up.szxytkj.cn

J. 日期与时间
来源：http://ia.lnxyls.cn

================================================================================
来源：http://bp.colortex.cn

[J01] 获取当前时间
来源：http://ie.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dx.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iu.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://rh.nicolike.cn

TS:   new Date();  Date.now()
来源：http://cy.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qa.jianghongdianzi.cn

Go:   time.Now()
来源：http://av.shxzukj.cn

Ruby: Time.now
来源：http://jb.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sy.huixiangedu.cn

[J02] 格式化输出
来源：http://bi.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sh.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ky.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zf.wgjwhj.cn

TS:   d.toISOString()
来源：http://vi.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://um.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pl.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ht.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sn.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://dj.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hu.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iz.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://mw.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://oj.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mr.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nk.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://sr.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gq.szsharing.cn

[J04] 时间戳与日期互转
来源：http://cu.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vu.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zu.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://si.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qg.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dp.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mg.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pp.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://ky.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://wa.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bm.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hs.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ea.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ng.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lk.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://po.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pf.shtwfgs.cn

[J06] 计算两时间之差
来源：http://be.521024.cn

Py:   (end - start).total_seconds()
来源：http://xa.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://uw.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mz.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fk.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hu.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://pn.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://ye.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://sk.hnjuh.cn

[J07] 比较两个日期
来源：http://vl.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ij.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://db.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cz.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hq.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zz.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qb.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cp.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://kr.colortex.cn

[J08] 提取年月日与星期
来源：http://bo.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oa.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ld.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ry.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mw.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qz.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://in.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ei.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vx.bjjhwx.cn

[J09] 时区处理
来源：http://hz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cy.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jy.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wj.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uj.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jz.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ns.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://av.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://vp.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vr.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yh.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fs.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vx.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ox.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wi.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://az.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lf.huixinmuqiang.cn

================================================================================
来源：http://th.nszjky.cn

K. JSON 与序列化
来源：http://kf.bookmarksfly.cn

================================================================================
来源：http://nr.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://we.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kl.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rn.colortex.cn

JS:   JSON.stringify(obj)
来源：http://uz.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://jv.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bu.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://wq.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://st.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qx.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ts.wgjwhj.cn

Py:   json.loads(s)
来源：http://yc.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://io.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://fc.huanxung.cn

TS:   JSON.parse(s)
来源：http://dk.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://np.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://er.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://jp.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sa.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://qo.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ja.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kw.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pc.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xt.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ia.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ty.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jq.nicolike.cn

[K04] 读取 JSON 文件
来源：http://kl.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ob.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ch.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zu.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ll.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ww.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ua.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mh.shxzskj.cn

[K05] 深拷贝对象
来源：http://ma.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://mp.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://rc.asd995.cn

JS:   structuredClone(obj)
来源：http://xg.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://cy.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kz.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://th.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vl.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iy.huanxung.cn


<!-- 参考信息 -->