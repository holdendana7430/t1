代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rx.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://js.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bm.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ss.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zv.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ws.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ik.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xp.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://je.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rn.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ua.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dq.newstarts.cn

[H03] 主动抛出异常
来源：http://tr.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://iu.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fj.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://qd.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://ft.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://um.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oi.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zk.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fa.yuexingan06.cn

[H04] 自定义异常类型
来源：http://wt.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://ys.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cg.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://zx.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://qp.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://gf.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lt.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://ir.newstarts.cn

C#:   class MyException : Exception {}
来源：http://cw.521024.cn

[H05] 捕获特定类型
来源：http://up.szxytkj.cn

Py:   except ValueError as e:
来源：http://tx.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://el.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://jt.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://fw.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://zd.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jy.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://tb.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tc.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://hk.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://bi.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eu.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sk.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://an.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vb.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jf.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://wl.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://aw.9csxet.cn

[H07] 断言
来源：http://ic.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://vc.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://dv.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://fe.asd995.cn

TS:   console.assert(x > 0);
来源：http://kr.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://ra.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kv.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://jv.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://dk.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://as.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cx.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://uu.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zx.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ay.asd995.cn

Go:   err.Error()
来源：http://jr.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://cf.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://el.9csxet.cn

[H09] 带错误码的异常
来源：http://ao.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://js.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qu.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qb.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bu.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qr.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qa.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yk.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oa.newstarts.cn

[H10] 资源自动释放
来源：http://yx.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://om.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hs.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dk.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ra.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lu.yuexingan06.cn

Go:   defer f.Close()
来源：http://kw.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nt.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zs.jianghongdianzi.cn

================================================================================
来源：http://ks.gzmigu.cn

I. 正则表达式
来源：http://xe.bookmarksfly.cn

================================================================================
来源：http://hm.newstarts.cn

[I01] 判断是否匹配
来源：http://cg.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jc.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://by.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://he.nszjky.cn

TS:   /\d+/.test(s)
来源：http://wm.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kh.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ox.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://va.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://se.panjiajie.cn

[I02] 提取所有匹配
来源：http://qn.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ff.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qt.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mf.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://kj.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zk.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ed.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://sk.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wk.nszjky.cn

[I03] 提取捕获分组
来源：http://jr.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eb.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://go.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yx.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gk.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ut.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oe.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ud.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lp.szsharing.cn

[I04] 正则替换
来源：http://sb.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zs.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ka.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xk.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xm.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rt.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mj.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pv.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://du.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://hv.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vi.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oc.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://bj.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ls.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://sb.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hy.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zn.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hl.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eg.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gt.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zm.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tv.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ky.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yg.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qr.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ew.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fy.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://vk.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ro.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ku.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sj.haigaiapp.cn

TS:   /error/gim
来源：http://yz.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pq.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dg.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://cm.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lr.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://jz.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ae.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nc.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qa.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wq.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nc.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://td.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zp.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gc.muxihuayi.cn

================================================================================
来源：http://ba.yuexingan06.cn

J. 日期与时间
来源：http://sc.jctech888.com.cn

================================================================================
来源：http://au.shxzskj.cn

[J01] 获取当前时间
来源：http://ig.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fd.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://io.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://xu.nszjky.cn

TS:   new Date();  Date.now()
来源：http://fb.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eh.hnjuh.cn

Go:   time.Now()
来源：http://ln.newstarts.cn

Ruby: Time.now
来源：http://bg.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://as.huanxung.cn

[J02] 格式化输出
来源：http://dt.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://am.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wd.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eq.jctech888.com.cn

TS:   d.toISOString()
来源：http://mm.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sz.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://az.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dx.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ry.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://br.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fj.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://le.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://lk.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://kk.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://io.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xp.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://es.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kt.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://cb.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mz.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pn.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://af.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gf.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eu.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ca.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rc.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fo.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://gr.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://um.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mj.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cn.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qe.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://gt.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kq.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://cs.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tc.szxytkj.cn

[J06] 计算两时间之差
来源：http://fp.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://eq.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://pl.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tp.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ky.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tu.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://ol.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://om.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://sw.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://kg.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ir.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pb.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://np.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cd.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tp.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://va.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kh.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://oh.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://af.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qo.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tk.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eb.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nq.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ns.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qj.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rr.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bc.yuntaijiaju.cn

[J09] 时区处理
来源：http://dz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kh.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yw.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bb.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jd.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://re.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ql.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ch.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tv.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://nf.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ag.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cy.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sr.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ds.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wx.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sv.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jf.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vq.asd995.cn

================================================================================
来源：http://zg.yuexingan06.cn

K. JSON 与序列化
来源：http://hv.yuntaijiaju.cn

================================================================================
来源：http://qe.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://sy.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xc.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ka.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://jk.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://qh.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ev.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://wp.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dk.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pj.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://lv.hnjuh.cn

Py:   json.loads(s)
来源：http://cx.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://px.nicolike.cn

JS:   JSON.parse(s)
来源：http://nt.huanxung.cn

TS:   JSON.parse(s)
来源：http://ch.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lw.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://yp.szsharing.cn

Ruby: JSON.parse(s)
来源：http://tt.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ty.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://lt.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rc.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mp.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://og.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ui.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wf.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tv.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hx.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kj.colortex.cn

[K04] 读取 JSON 文件
来源：http://tl.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nm.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mo.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://be.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uf.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hv.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oo.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rm.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://yq.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://cq.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://rm.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://vl.521024.cn

TS:   structuredClone(obj)
来源：http://ua.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qn.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zd.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ai.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cf.bookmarksfly.cn


<!-- 参考信息 -->