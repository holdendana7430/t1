代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://sw.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pa.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xa.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ke.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hq.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://es.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rw.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fi.chemitech.net.cn

[H03] 主动抛出异常
来源：http://iy.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://am.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gi.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://ft.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://ap.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qk.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nf.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rp.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oz.hnjuh.cn

[H04] 自定义异常类型
来源：http://nk.521024.cn

Py:   class MyError(Exception): pass
来源：http://pe.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://da.hahajie.cn

JS:   class MyError extends Error {}
来源：http://us.521024.cn

TS:   class MyError extends Error {}
来源：http://sj.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://ae.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cq.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://dm.9csxet.cn

C#:   class MyException : Exception {}
来源：http://cc.huanxung.cn

[H05] 捕获特定类型
来源：http://ba.jctech888.com.cn

Py:   except ValueError as e:
来源：http://dt.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kp.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://pv.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://vs.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://qd.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rk.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://jp.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://az.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://ae.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://jh.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ap.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bs.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ci.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hn.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://od.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://wh.521024.cn

C#:   obj?.A?.B ?? default
来源：http://pg.yuexingan06.cn

[H07] 断言
来源：http://in.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://lz.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://mv.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://en.nszjky.cn

TS:   console.assert(x > 0);
来源：http://po.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://sq.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://um.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://id.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ej.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://zi.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://gs.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ox.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://tv.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fr.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://en.bjjhwx.cn

Go:   err.Error()
来源：http://fz.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://xn.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://jb.gzmigu.cn

[H09] 带错误码的异常
来源：http://xk.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ex.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://be.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rh.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cq.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kq.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tu.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ts.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rx.chemitech.net.cn

[H10] 资源自动释放
来源：http://qq.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ri.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oq.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hd.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://it.9csxet.cn

Go:   defer f.Close()
来源：http://ey.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://au.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ye.haigaiapp.cn

================================================================================
来源：http://ld.szsharing.cn

I. 正则表达式
来源：http://fn.chemitech.net.cn

================================================================================
来源：http://qi.panjiajie.cn

[I01] 判断是否匹配
来源：http://an.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vk.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oj.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://zx.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://cj.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dl.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yo.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://ey.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fv.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://jz.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ok.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ze.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://kz.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nn.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fs.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://vy.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oc.szsharing.cn

[I03] 提取捕获分组
来源：http://yb.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mq.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ce.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gg.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wi.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://no.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gc.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qb.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bm.yuntaijiaju.cn

[I04] 正则替换
来源：http://us.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zz.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xv.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ad.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://to.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rr.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kb.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ff.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zj.huanxung.cn

[I05] 按正则拆分
来源：http://kv.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ux.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hx.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bc.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ky.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://jz.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fc.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://db.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cf.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rz.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://br.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iv.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qx.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yv.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mg.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uk.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ve.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lg.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://ox.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://np.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://es.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aw.szsharing.cn

TS:   /error/gim
来源：http://kf.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bc.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ms.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://bk.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bk.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://qh.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qc.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lr.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zj.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tr.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xs.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mt.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cy.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qu.wgjwhj.cn

================================================================================
来源：http://ux.asd995.cn

J. 日期与时间
来源：http://xo.shxzskj.cn

================================================================================
来源：http://iw.huanxung.cn

[J01] 获取当前时间
来源：http://ai.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qk.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ih.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://pj.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://qm.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yd.huanxung.cn

Go:   time.Now()
来源：http://ey.521024.cn

Ruby: Time.now
来源：http://us.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ge.szxytkj.cn

[J02] 格式化输出
来源：http://yf.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wl.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wv.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ea.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://pd.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cy.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://se.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hh.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uk.shxzukj.cn

[J03] 字符串解析为日期
来源：http://qk.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://to.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wo.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://zp.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://bv.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lp.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xs.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://ls.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yl.huanxung.cn

[J04] 时间戳与日期互转
来源：http://hz.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ac.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://re.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fw.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mt.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ez.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jo.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wc.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pc.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://lx.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://xx.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://be.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xu.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yu.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://eq.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bm.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://br.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ib.shxzukj.cn

[J06] 计算两时间之差
来源：http://pc.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://xu.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://sq.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fa.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gt.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://rm.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://bh.521024.cn

C#:   (end - start).TotalSeconds
来源：http://pv.asd995.cn

[J07] 比较两个日期
来源：http://oe.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://ow.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wf.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tj.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kd.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oi.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nl.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lo.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://ye.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://zk.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pu.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qh.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fu.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jf.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fi.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ew.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iw.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zb.szxytkj.cn

[J09] 时区处理
来源：http://rk.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ih.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mr.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uy.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dl.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ji.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qr.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lt.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ga.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://bg.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kv.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://il.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oi.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zc.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ke.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xy.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qk.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bw.bjjhwx.cn

================================================================================
来源：http://rv.nicolike.cn

K. JSON 与序列化
来源：http://sp.muxihuayi.cn

================================================================================
来源：http://sz.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://ev.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ai.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dp.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://sr.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://jh.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fc.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://cl.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fi.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dx.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ri.asd995.cn

Py:   json.loads(s)
来源：http://as.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://az.newstarts.cn

JS:   JSON.parse(s)
来源：http://zk.colortex.cn

TS:   JSON.parse(s)
来源：http://hg.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://di.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://zy.colortex.cn

Ruby: JSON.parse(s)
来源：http://bq.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oq.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://gf.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xz.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ql.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rk.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bc.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sk.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pt.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nu.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hq.9csxet.cn

[K04] 读取 JSON 文件
来源：http://mq.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://un.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jv.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://md.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fs.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ug.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mp.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tb.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wb.nszjky.cn

[K05] 深拷贝对象
来源：http://ft.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://aq.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://vo.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://lc.szsharing.cn

TS:   structuredClone(obj)
来源：http://mo.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xg.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qh.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cv.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wz.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://ju.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ig.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zc.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ve.chemitech.net.cn


<!-- 参考信息 -->