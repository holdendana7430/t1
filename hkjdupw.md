代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://es.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wj.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://st.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ec.muxihuayi.cn

[H03] 主动抛出异常
来源：http://fd.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://vy.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://uh.colortex.cn

TS:   throw new Error("错误信息");
来源：http://bg.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ge.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ua.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xm.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fr.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://mi.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://hn.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sb.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://fz.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://cj.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://ts.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ch.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ix.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://ur.hahajie.cn

[H05] 捕获特定类型
来源：http://ct.haigaiapp.cn

Py:   except ValueError as e:
来源：http://nq.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://np.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ov.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://jf.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://in.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tp.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://dm.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yo.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://cl.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://hh.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://as.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xz.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qc.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ek.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ay.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ib.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://vf.bookmarksfly.cn

[H07] 断言
来源：http://yi.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://sd.521024.cn

PHP:  assert($x > 0);
来源：http://cl.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://ei.asd995.cn

TS:   console.assert(x > 0);
来源：http://kf.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://fy.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yf.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sj.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://mm.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://qt.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://bo.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tx.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://dd.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pc.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mz.521024.cn

Go:   err.Error()
来源：http://ea.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://iu.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://ks.nicolike.cn

[H09] 带错误码的异常
来源：http://lw.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ib.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ui.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gz.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mc.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hd.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ts.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bd.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vw.nicolike.cn

[H10] 资源自动释放
来源：http://ps.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xk.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yy.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oc.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hw.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sa.shxzskj.cn

Go:   defer f.Close()
来源：http://wf.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zs.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eu.9csxet.cn

================================================================================
来源：http://gc.asd995.cn

I. 正则表达式
来源：http://ne.9csxet.cn

================================================================================
来源：http://re.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ii.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yl.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wr.newstarts.cn

JS:   /\d+/.test(s)
来源：http://gu.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://su.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eo.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nv.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://pc.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zh.hnjuh.cn

[I02] 提取所有匹配
来源：http://ud.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ah.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bb.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fk.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://oc.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jb.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rb.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://tf.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vk.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sj.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tz.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nh.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://so.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bg.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wa.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mn.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ao.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gm.huanxung.cn

[I04] 正则替换
来源：http://tq.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://be.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mm.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mx.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://un.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gg.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jw.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://va.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bz.yuexingan06.cn

[I05] 按正则拆分
来源：http://jj.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hc.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://di.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://mw.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://dg.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ee.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gu.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dj.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dz.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gs.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ar.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nb.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dd.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fp.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iq.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ia.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://os.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://et.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://gq.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ro.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uj.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sw.jianghongdianzi.cn

TS:   /error/gim
来源：http://ac.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pt.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sq.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://hy.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hb.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://uw.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xr.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cn.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bv.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fu.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zh.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://do.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://my.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ge.521024.cn

================================================================================
来源：http://tj.9csxet.cn

J. 日期与时间
来源：http://ci.huanxung.cn

================================================================================
来源：http://uq.huixiangedu.cn

[J01] 获取当前时间
来源：http://da.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bb.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yf.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://vd.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://vy.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bm.bjjhwx.cn

Go:   time.Now()
来源：http://zy.lnxyls.cn

Ruby: Time.now
来源：http://yb.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cw.newstarts.cn

[J02] 格式化输出
来源：http://na.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ud.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gh.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hx.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://si.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rw.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ev.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vs.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uc.hahajie.cn

[J03] 字符串解析为日期
来源：http://vq.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fg.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ws.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://af.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://yx.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cr.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://al.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://pl.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sl.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://fm.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dd.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cz.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sh.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rj.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fe.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mu.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ve.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iz.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://jw.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://tf.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vt.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ec.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ln.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fh.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://js.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://an.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kh.9csxet.cn

[J06] 计算两时间之差
来源：http://eg.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://zv.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://rc.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oc.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ts.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vr.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://xl.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://xr.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://wj.yuexingan06.cn

[J07] 比较两个日期
来源：http://rq.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://iu.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wu.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yf.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mv.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ak.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jy.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zv.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://il.colortex.cn

[J08] 提取年月日与星期
来源：http://xx.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wk.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ud.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nr.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yy.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yc.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ed.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bc.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pw.hahajie.cn

[J09] 时区处理
来源：http://wi.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nk.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qp.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dg.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yu.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://le.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ib.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mm.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iq.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://xu.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ub.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pm.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lc.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lb.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uf.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wq.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bh.shtwfgs.cn

================================================================================
来源：http://rv.colortex.cn

K. JSON 与序列化
来源：http://qt.shxzukj.cn

================================================================================
来源：http://so.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://br.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jo.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ks.colortex.cn

JS:   JSON.stringify(obj)
来源：http://mf.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://jz.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yh.9csxet.cn

Go:   json.Marshal(obj)
来源：http://qs.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yh.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ix.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ix.shxzukj.cn

Py:   json.loads(s)
来源：http://nx.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vj.nicolike.cn

JS:   JSON.parse(s)
来源：http://ls.szxytkj.cn

TS:   JSON.parse(s)
来源：http://rr.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://td.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://cy.nicolike.cn

Ruby: JSON.parse(s)
来源：http://re.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ut.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://qo.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dc.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://en.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ye.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pl.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yb.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nd.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ct.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ql.szsharing.cn

[K04] 读取 JSON 文件
来源：http://vt.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rh.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zn.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ku.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tt.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tg.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jd.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uu.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hk.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://zh.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://yu.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://rf.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://ew.gzmigu.cn

TS:   structuredClone(obj)
来源：http://dr.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://su.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rc.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ip.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qp.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://uo.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://do.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ps.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yc.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tj.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://is.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.newstarts.cn


<!-- 参考信息 -->