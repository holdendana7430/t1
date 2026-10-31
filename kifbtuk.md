代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ps.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://or.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rx.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ed.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ri.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dk.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bv.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lo.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fi.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://am.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ym.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uc.9csxet.cn

[H03] 主动抛出异常
来源：http://cd.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://si.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ig.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://ud.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://kh.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vm.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dj.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wy.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ng.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://qz.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://el.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gz.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ns.hahajie.cn

TS:   class MyError extends Error {}
来源：http://ra.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://bj.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://il.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://sw.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://qa.szsharing.cn

[H05] 捕获特定类型
来源：http://im.9csxet.cn

Py:   except ValueError as e:
来源：http://ly.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sc.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://sf.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://em.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ss.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ht.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qx.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ph.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://xv.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mt.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ua.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aw.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ci.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kv.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://hf.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://zp.huixiangedu.cn

[H07] 断言
来源：http://kt.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://qc.asd995.cn

PHP:  assert($x > 0);
来源：http://ms.nszjky.cn

JS:   console.assert(x > 0);
来源：http://nb.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://hj.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://gb.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gh.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dv.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://af.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://tt.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://se.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ud.lnxyls.cn

JS:   e.message;  e.stack
来源：http://cr.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vh.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hp.huixiangedu.cn

Go:   err.Error()
来源：http://ki.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://md.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://kl.shtwfgs.cn

[H09] 带错误码的异常
来源：http://kr.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vg.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mn.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tc.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fd.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://au.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uk.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mi.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dk.szsharing.cn

[H10] 资源自动释放
来源：http://oi.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zk.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jx.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ve.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://li.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xh.huanxung.cn

Go:   defer f.Close()
来源：http://et.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vr.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lj.wgjwhj.cn

================================================================================
来源：http://lv.jianghongdianzi.cn

I. 正则表达式
来源：http://ta.chemitech.net.cn

================================================================================
来源：http://fw.hnjuh.cn

[I01] 判断是否匹配
来源：http://zb.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lj.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wp.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://cr.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://an.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dl.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kk.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://sb.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fy.gzmigu.cn

[I02] 提取所有匹配
来源：http://oq.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://pt.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hw.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rm.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://zu.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oy.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mu.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://ug.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://el.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://zf.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lu.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fd.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zz.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ux.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sj.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://es.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vn.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://th.asd995.cn

[I04] 正则替换
来源：http://ev.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://er.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nr.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gs.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kq.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nf.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kk.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ca.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tl.haigaiapp.cn

[I05] 按正则拆分
来源：http://xi.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wk.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ro.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://io.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://hu.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://os.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qw.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vd.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gn.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ws.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ua.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tu.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://to.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://va.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qu.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dn.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ql.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://na.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://em.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oy.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ct.chemitech.net.cn

TS:   /error/gim
来源：http://uq.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ig.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zr.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://iq.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://je.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://jm.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wt.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gh.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mg.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fr.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xn.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xi.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xe.shxzskj.cn

================================================================================
来源：http://uc.9csxet.cn

J. 日期与时间
来源：http://lw.521024.cn

================================================================================
来源：http://qx.szsharing.cn

[J01] 获取当前时间
来源：http://xi.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ic.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jq.colortex.cn

JS:   new Date();  Date.now()
来源：http://tj.nicolike.cn

TS:   new Date();  Date.now()
来源：http://yw.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xa.colortex.cn

Go:   time.Now()
来源：http://zu.yuntaijiaju.cn

Ruby: Time.now
来源：http://qn.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gw.yuexingan06.cn

[J02] 格式化输出
来源：http://tm.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qw.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ff.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://je.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pr.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wp.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jj.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ej.szxytkj.cn

[J03] 字符串解析为日期
来源：http://cg.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zw.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hy.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://vv.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://pg.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zs.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lq.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://kc.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zc.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://rk.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ql.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lk.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ey.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bu.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kf.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sn.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hj.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jr.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://zg.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ue.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vh.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gl.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eq.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://km.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://av.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://dg.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xm.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://yy.colortex.cn

Py:   (end - start).total_seconds()
来源：http://dl.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://kf.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rk.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xv.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qe.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://bh.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ge.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://gx.shxzukj.cn

[J07] 比较两个日期
来源：http://er.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zr.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yr.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nv.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tw.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yt.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hr.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kp.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://bo.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://oz.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gw.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uc.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nd.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pt.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hj.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fr.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lp.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qr.haigaiapp.cn

[J09] 时区处理
来源：http://ap.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xx.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ak.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nf.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vf.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lb.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ma.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oi.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ur.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://pu.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vp.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ha.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kw.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hq.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zu.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gu.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nk.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.wgjwhj.cn

================================================================================
来源：http://sf.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ew.gzmigu.cn

================================================================================
来源：http://pu.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://yi.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://np.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qe.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://jx.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://ge.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rp.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://fd.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nw.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vm.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://av.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://gw.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cj.colortex.cn

JS:   JSON.parse(s)
来源：http://uu.nszjky.cn

TS:   JSON.parse(s)
来源：http://qt.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oi.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://xr.huanxung.cn

Ruby: JSON.parse(s)
来源：http://ga.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qq.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://wp.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dd.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fq.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kj.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hi.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ja.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qy.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mw.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ng.nicolike.cn

[K04] 读取 JSON 文件
来源：http://nv.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hr.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cg.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ns.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pl.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://id.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ar.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yk.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://vx.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://uh.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://fu.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://po.newstarts.cn

TS:   structuredClone(obj)
来源：http://ax.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zz.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kr.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yd.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nz.hnjuh.cn


<!-- 参考信息 -->