代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://ng.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aq.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hm.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ed.muxihuayi.cn

[H03] 主动抛出异常
来源：http://ws.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://pz.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uo.521024.cn

JS:   throw new Error("错误信息");
来源：http://ii.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://yt.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ki.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jl.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xb.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lb.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://kd.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://oh.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fz.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://id.colortex.cn

TS:   class MyError extends Error {}
来源：http://ng.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://fz.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xs.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://zy.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://dw.shxzskj.cn

[H05] 捕获特定类型
来源：http://zg.chemitech.net.cn

Py:   except ValueError as e:
来源：http://hk.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cy.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://fw.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://lc.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://gj.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yv.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://sz.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mv.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://bh.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://mq.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gg.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gy.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nf.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bz.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mw.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://at.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://ks.panjiajie.cn

[H07] 断言
来源：http://uc.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://dt.szsharing.cn

PHP:  assert($x > 0);
来源：http://xo.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ig.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://fq.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://nz.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://na.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xr.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ml.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://em.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://ir.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aw.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://lc.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ek.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ei.huixinmuqiang.cn

Go:   err.Error()
来源：http://tz.521024.cn

Ruby: e.message;  e.backtrace
来源：http://cd.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://co.szsharing.cn

[H09] 带错误码的异常
来源：http://lp.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wf.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lc.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hi.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ov.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yz.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bp.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vm.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wo.nicolike.cn

[H10] 资源自动释放
来源：http://lp.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pq.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sa.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://at.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ew.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ic.hnjuh.cn

Go:   defer f.Close()
来源：http://vv.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bt.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ac.szsharing.cn

================================================================================
来源：http://sz.huixinmuqiang.cn

I. 正则表达式
来源：http://xi.bjjhwx.cn

================================================================================
来源：http://om.huanxung.cn

[I01] 判断是否匹配
来源：http://pz.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qy.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ey.hahajie.cn

JS:   /\d+/.test(s)
来源：http://pz.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://xb.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mx.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pp.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://qu.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fn.lnxyls.cn

[I02] 提取所有匹配
来源：http://nh.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://io.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xp.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qe.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://qf.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rf.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pu.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://pl.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ii.newstarts.cn

[I03] 提取捕获分组
来源：http://an.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lh.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dr.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://po.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vc.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pn.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://en.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xc.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ht.huixinmuqiang.cn

[I04] 正则替换
来源：http://wk.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ln.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oo.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://er.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xs.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bv.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pj.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nm.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gd.szsharing.cn

[I05] 按正则拆分
来源：http://nn.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fr.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fb.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://le.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://op.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://cb.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eq.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wu.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jf.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ok.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ox.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cr.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nf.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qm.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sk.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kz.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ar.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ej.521024.cn

[I07] 忽略大小写与多行模式
来源：http://hq.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xg.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nr.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jp.shxzukj.cn

TS:   /error/gim
来源：http://ls.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dt.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lh.asd995.cn

Ruby: s.scan(/error/i)
来源：http://an.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bb.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://sz.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hu.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ht.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zy.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://as.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://se.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sv.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gx.yuexingan06.cn

================================================================================
来源：http://ja.jctech888.com.cn

J. 日期与时间
来源：http://hw.nszjky.cn

================================================================================
来源：http://bq.szsharing.cn

[J01] 获取当前时间
来源：http://xd.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zx.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://na.colortex.cn

JS:   new Date();  Date.now()
来源：http://sm.huanxung.cn

TS:   new Date();  Date.now()
来源：http://sg.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uh.lnxyls.cn

Go:   time.Now()
来源：http://xb.asd995.cn

Ruby: Time.now
来源：http://kv.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://he.bjjhwx.cn

[J02] 格式化输出
来源：http://ru.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qv.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fx.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hc.szsharing.cn

TS:   d.toISOString()
来源：http://rh.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zd.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ye.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uu.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qy.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://du.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ws.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wq.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://we.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://tm.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gk.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ps.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ph.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oi.asd995.cn

[J04] 时间戳与日期互转
来源：http://ml.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oo.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kx.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tl.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bq.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://is.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://at.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rw.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wi.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://un.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://nr.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nu.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ja.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ej.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ih.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uv.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://cn.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sn.nszjky.cn

[J06] 计算两时间之差
来源：http://ua.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://cn.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://zt.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bh.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rx.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ji.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://xw.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ix.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://wb.newstarts.cn

[J07] 比较两个日期
来源：http://uf.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vq.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oy.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kq.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oz.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kp.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pc.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://of.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://bh.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jx.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qv.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tp.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yr.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ur.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rs.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qn.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qz.jianghongdianzi.cn

[J09] 时区处理
来源：http://xo.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pt.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vb.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qh.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yd.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lu.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gs.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://po.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://rl.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ru.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ep.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lq.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xy.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hf.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vb.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bb.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sq.jianghongdianzi.cn

================================================================================
来源：http://ib.hnjuh.cn

K. JSON 与序列化
来源：http://ni.haigaiapp.cn

================================================================================
来源：http://ai.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://gb.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fq.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cx.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ud.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://uc.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nu.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://oo.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://te.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yh.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://rv.gzmigu.cn

Py:   json.loads(s)
来源：http://kz.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pv.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ln.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://gi.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qx.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://rl.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://rv.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rx.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bx.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ra.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pc.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vh.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sg.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qv.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://je.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yt.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://my.colortex.cn

[K04] 读取 JSON 文件
来源：http://ga.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qh.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pp.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jf.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xd.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zl.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://po.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kh.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ia.panjiajie.cn

[K05] 深拷贝对象
来源：http://yl.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://ks.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://tk.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://mx.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://kp.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cz.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gr.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qx.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rg.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://uw.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ls.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://es.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vc.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pd.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wb.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yz.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gl.wgjwhj.cn


<!-- 参考信息 -->