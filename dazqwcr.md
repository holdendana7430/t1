代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://ag.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ia.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kt.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pb.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qz.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://el.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ki.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://od.yuexingan06.cn

[H03] 主动抛出异常
来源：http://si.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://ie.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iq.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://lg.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://si.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mx.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nq.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tc.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://at.yuexingan06.cn

[H04] 自定义异常类型
来源：http://eu.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://hw.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fz.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://zn.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://nm.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://rm.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ua.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://dq.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://io.yuexingan06.cn

[H05] 捕获特定类型
来源：http://dd.panjiajie.cn

Py:   except ValueError as e:
来源：http://hp.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sq.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://af.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://wr.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://ys.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zv.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://ac.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mm.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://pt.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://wh.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lz.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yk.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nn.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ie.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lp.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://ob.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://fc.wgjwhj.cn

[H07] 断言
来源：http://di.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://ny.newstarts.cn

PHP:  assert($x > 0);
来源：http://pl.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://nx.asd995.cn

TS:   console.assert(x > 0);
来源：http://fa.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://st.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zu.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qm.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://qm.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://yy.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://et.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qh.gzmigu.cn

JS:   e.message;  e.stack
来源：http://cl.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yp.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zc.newstarts.cn

Go:   err.Error()
来源：http://mm.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://hl.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://yt.hahajie.cn

[H09] 带错误码的异常
来源：http://uu.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yg.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jn.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://po.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kh.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rc.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ga.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ju.gzmigu.cn

[H10] 资源自动释放
来源：http://ct.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uf.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://by.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uv.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xd.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ux.chemitech.net.cn

Go:   defer f.Close()
来源：http://xs.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://be.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wb.jianghongdianzi.cn

================================================================================
来源：http://ru.shxzskj.cn

I. 正则表达式
来源：http://pt.521024.cn

================================================================================
来源：http://qf.9csxet.cn

[I01] 判断是否匹配
来源：http://lj.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gn.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jv.hahajie.cn

JS:   /\d+/.test(s)
来源：http://pf.hahajie.cn

TS:   /\d+/.test(s)
来源：http://yi.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lv.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bv.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://dg.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yq.asd995.cn

[I02] 提取所有匹配
来源：http://mf.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://ul.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://no.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xs.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://xl.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bl.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bz.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://ey.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ts.jctech888.com.cn

[I03] 提取捕获分组
来源：http://rk.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zc.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ob.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jo.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ua.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mk.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ju.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://na.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ya.yuexingan06.cn

[I04] 正则替换
来源：http://ri.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://it.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rw.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mk.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mf.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xm.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://po.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ua.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pa.asd995.cn

[I05] 按正则拆分
来源：http://sy.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hv.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xs.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://vd.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://wr.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://vw.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xi.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rr.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iv.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vj.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jx.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ou.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uc.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://we.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ry.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sd.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://do.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://nb.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wc.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rw.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gt.huixinmuqiang.cn

TS:   /error/gim
来源：http://sv.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dn.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zm.asd995.cn

Ruby: s.scan(/error/i)
来源：http://uj.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://th.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://gj.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nh.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cy.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mf.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tk.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wg.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kx.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ij.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qb.nszjky.cn

================================================================================
来源：http://ct.nicolike.cn

J. 日期与时间
来源：http://pv.huanxung.cn

================================================================================
来源：http://sn.muxihuayi.cn

[J01] 获取当前时间
来源：http://ts.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ck.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qz.hahajie.cn

JS:   new Date();  Date.now()
来源：http://rw.newstarts.cn

TS:   new Date();  Date.now()
来源：http://pc.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dm.huanxung.cn

Go:   time.Now()
来源：http://hw.nicolike.cn

Ruby: Time.now
来源：http://zu.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xp.haigaiapp.cn

[J02] 格式化输出
来源：http://io.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://do.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yq.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hh.huixiangedu.cn

TS:   d.toISOString()
来源：http://ps.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dn.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yo.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fm.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://td.nicolike.cn

[J03] 字符串解析为日期
来源：http://ho.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xu.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hf.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://ao.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ay.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vo.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pm.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://vb.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dj.9csxet.cn

[J04] 时间戳与日期互转
来源：http://vk.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mk.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ce.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fs.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fx.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ew.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sj.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oi.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eu.521024.cn

[J05] 时间加减（加 7 天）
来源：http://as.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ud.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bi.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ba.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://sq.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wl.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://qa.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vs.hnjuh.cn

[J06] 计算两时间之差
来源：http://rg.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://zc.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://qf.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kf.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mk.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hk.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://oo.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://dl.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://zb.lnxyls.cn

[J07] 比较两个日期
来源：http://qe.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://he.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rx.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cs.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vp.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zx.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zt.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ck.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://kx.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ba.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://no.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eo.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sn.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vn.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mz.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ar.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nj.colortex.cn

[J09] 时区处理
来源：http://of.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wh.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vf.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uz.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oh.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hw.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kt.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wo.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xq.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://jx.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gd.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gw.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dp.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mh.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wr.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bh.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qb.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dr.jctech888.com.cn

================================================================================
来源：http://lo.yuexingan06.cn

K. JSON 与序列化
来源：http://kq.bjjhwx.cn

================================================================================
来源：http://gu.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://kq.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xs.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://rh.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://zh.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lu.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://wo.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://py.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yi.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://oc.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://ob.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qr.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://cb.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://lo.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nx.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ni.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://lt.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vj.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://cd.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mb.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wl.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hq.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ao.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sc.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qb.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qp.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gz.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://em.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vh.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://df.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xz.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kw.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://at.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qv.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fo.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zt.shxzukj.cn

[K05] 深拷贝对象
来源：http://ma.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://bt.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://ar.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://ip.lnxyls.cn

TS:   structuredClone(obj)
来源：http://jn.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ly.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hg.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://op.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vj.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://jo.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mv.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ql.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vo.521024.cn


<!-- 参考信息 -->