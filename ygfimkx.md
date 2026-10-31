代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://qg.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cj.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://re.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://us.huixiangedu.cn

[H03] 主动抛出异常
来源：http://ij.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://mo.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rm.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://dj.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://sf.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rl.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yh.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xi.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fl.hahajie.cn

[H04] 自定义异常类型
来源：http://mb.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://ir.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eh.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://jt.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ih.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://ur.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://az.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://gk.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://la.shxzskj.cn

[H05] 捕获特定类型
来源：http://rj.521024.cn

Py:   except ValueError as e:
来源：http://wp.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kn.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://vp.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://yy.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://gk.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sm.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://gg.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zm.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://zr.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ap.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fm.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mt.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cr.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vg.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://go.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://te.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://hz.panjiajie.cn

[H07] 断言
来源：http://ib.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://fu.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://em.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://mp.nszjky.cn

TS:   console.assert(x > 0);
来源：http://nk.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://ub.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vb.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wv.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://vp.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://cu.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ls.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pn.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://gt.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mo.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tv.szsharing.cn

Go:   err.Error()
来源：http://ax.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://zu.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://ir.nszjky.cn

[H09] 带错误码的异常
来源：http://mt.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sv.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ob.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ev.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yn.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pm.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xs.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tb.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://je.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://fj.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rc.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gu.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kg.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zg.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ze.huanxung.cn

Go:   defer f.Close()
来源：http://pc.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ot.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xs.huixinmuqiang.cn

================================================================================
来源：http://cj.huixiangedu.cn

I. 正则表达式
来源：http://nu.asd995.cn

================================================================================
来源：http://fd.muxihuayi.cn

[I01] 判断是否匹配
来源：http://yh.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qe.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wa.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://nk.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://dj.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ps.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pk.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://hl.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aq.colortex.cn

[I02] 提取所有匹配
来源：http://ze.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://ym.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fx.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kk.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://up.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pj.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://do.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://ps.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ly.chemitech.net.cn

[I03] 提取捕获分组
来源：http://ve.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xx.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mj.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tc.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jz.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yj.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ec.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mq.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gt.jctech888.com.cn

[I04] 正则替换
来源：http://cf.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xi.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bu.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://be.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ay.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ky.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aj.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ng.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ao.hnjuh.cn

[I05] 按正则拆分
来源：http://ec.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://io.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gb.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://qa.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://zg.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://sc.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oq.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uv.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://db.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ra.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rp.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wn.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zn.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ty.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ro.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rc.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nb.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cb.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://gl.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://py.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bd.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qo.jctech888.com.cn

TS:   /error/gim
来源：http://dh.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ac.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jy.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://dg.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ql.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://qp.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://my.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ck.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cq.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://et.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wf.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ba.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cp.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://of.muxihuayi.cn

================================================================================
来源：http://cn.wgjwhj.cn

J. 日期与时间
来源：http://xt.szsharing.cn

================================================================================
来源：http://dn.huixiangedu.cn

[J01] 获取当前时间
来源：http://fn.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nw.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ap.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://iu.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://do.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pd.bjjhwx.cn

Go:   time.Now()
来源：http://pk.huixinmuqiang.cn

Ruby: Time.now
来源：http://eo.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jx.gzmigu.cn

[J02] 格式化输出
来源：http://xm.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ej.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zl.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yu.lnxyls.cn

TS:   d.toISOString()
来源：http://af.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gs.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://es.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ne.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xt.newstarts.cn

[J03] 字符串解析为日期
来源：http://ph.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://so.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://im.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://xx.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://dx.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ei.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fi.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ps.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ig.nszjky.cn

[J04] 时间戳与日期互转
来源：http://ig.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cr.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gr.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yz.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gn.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ck.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zi.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lg.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jb.521024.cn

[J05] 时间加减（加 7 天）
来源：http://zq.521024.cn

Py:   now + timedelta(days=7)
来源：http://ex.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pn.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fy.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ho.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ub.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://af.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://xf.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sv.haigaiapp.cn

[J06] 计算两时间之差
来源：http://np.521024.cn

Py:   (end - start).total_seconds()
来源：http://np.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://im.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lf.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ki.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vp.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://lx.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://im.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://st.newstarts.cn

[J07] 比较两个日期
来源：http://yk.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://vs.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vm.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://it.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gu.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kc.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ol.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ut.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://vv.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://zz.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ko.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wc.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ib.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sy.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qd.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cn.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gg.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gm.newstarts.cn

[J09] 时区处理
来源：http://sv.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rt.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oy.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://je.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mh.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qi.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ff.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cf.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nm.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://yf.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ax.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xh.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jy.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mo.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dt.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ls.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fq.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wx.panjiajie.cn

================================================================================
来源：http://ql.szxytkj.cn

K. JSON 与序列化
来源：http://dd.asd995.cn

================================================================================
来源：http://yp.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ao.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xf.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://um.521024.cn

JS:   JSON.stringify(obj)
来源：http://zg.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://yp.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rh.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://zk.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hp.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bw.colortex.cn

[K02] JSON 字符串转对象
来源：http://ik.hnjuh.cn

Py:   json.loads(s)
来源：http://og.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kr.szsharing.cn

JS:   JSON.parse(s)
来源：http://sy.asd995.cn

TS:   JSON.parse(s)
来源：http://pw.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zi.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://zu.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://uc.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qx.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://eb.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dp.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://al.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://az.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gr.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ig.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://py.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ba.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://un.hahajie.cn

[K04] 读取 JSON 文件
来源：http://wc.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vl.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://js.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tv.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jv.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ss.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lz.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://di.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zk.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://fv.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://hr.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://hp.gzmigu.cn

JS:   structuredClone(obj)
来源：http://fd.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://no.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tw.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uw.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hk.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://re.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://wu.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yn.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hq.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jj.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://on.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ta.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ka.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wx.muxihuayi.cn


<!-- 参考信息 -->