代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://if.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cz.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pe.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lz.lnxyls.cn

[H03] 主动抛出异常
来源：http://ns.521024.cn

Py:   raise ValueError("错误信息")
来源：http://il.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ve.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://wl.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://ti.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rk.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://km.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qp.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ru.jctech888.com.cn

[H04] 自定义异常类型
来源：http://vc.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://vv.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gl.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://ks.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://rj.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://qe.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ms.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ub.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://xy.jctech888.com.cn

[H05] 捕获特定类型
来源：http://ny.521024.cn

Py:   except ValueError as e:
来源：http://fg.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vz.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://hp.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://le.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://kg.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fo.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://mp.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uf.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://nt.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://de.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cz.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ps.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://le.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yb.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uq.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://jq.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://ho.yuexingan06.cn

[H07] 断言
来源：http://eq.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://qj.colortex.cn

PHP:  assert($x > 0);
来源：http://sb.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://av.nicolike.cn

TS:   console.assert(x > 0);
来源：http://de.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://zl.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ki.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zx.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://nt.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://oq.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://si.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rw.shxzukj.cn

JS:   e.message;  e.stack
来源：http://dy.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ue.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tj.hahajie.cn

Go:   err.Error()
来源：http://sw.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://br.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ew.bjjhwx.cn

[H09] 带错误码的异常
来源：http://gc.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kb.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://af.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xg.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://el.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vg.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yg.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://be.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fy.shxzskj.cn

[H10] 资源自动释放
来源：http://kl.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wi.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hx.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bz.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rq.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wn.colortex.cn

Go:   defer f.Close()
来源：http://fi.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uo.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rm.bookmarksfly.cn

================================================================================
来源：http://ce.yuexingan06.cn

I. 正则表达式
来源：http://ju.huixinmuqiang.cn

================================================================================
来源：http://sd.asd995.cn

[I01] 判断是否匹配
来源：http://zj.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vv.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xy.colortex.cn

JS:   /\d+/.test(s)
来源：http://la.521024.cn

TS:   /\d+/.test(s)
来源：http://of.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ow.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bm.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://uq.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gy.huixiangedu.cn

[I02] 提取所有匹配
来源：http://fx.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://az.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kf.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://et.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://eu.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ck.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ax.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://sg.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zh.gzmigu.cn

[I03] 提取捕获分组
来源：http://bf.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lc.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://is.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ez.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cw.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bu.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jt.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qo.newstarts.cn

[I04] 正则替换
来源：http://uo.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hq.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xx.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hk.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dw.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tf.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pp.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://av.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gk.panjiajie.cn

[I05] 按正则拆分
来源：http://ff.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://px.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tr.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ac.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ii.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://xi.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cv.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zz.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://us.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vk.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kv.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hv.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ty.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oe.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yo.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sb.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://an.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fq.521024.cn

[I07] 忽略大小写与多行模式
来源：http://ee.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ts.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bm.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ar.szxytkj.cn

TS:   /error/gim
来源：http://ed.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qz.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qe.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://uv.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ky.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://bw.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vr.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rs.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tx.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://id.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dv.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gj.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lk.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uu.shxzukj.cn

================================================================================
来源：http://ss.bjjhwx.cn

J. 日期与时间
来源：http://ur.huixinmuqiang.cn

================================================================================
来源：http://kz.panjiajie.cn

[J01] 获取当前时间
来源：http://jf.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aw.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://am.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://lp.hahajie.cn

TS:   new Date();  Date.now()
来源：http://xg.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ym.nicolike.cn

Go:   time.Now()
来源：http://jg.huixinmuqiang.cn

Ruby: Time.now
来源：http://fn.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tb.haigaiapp.cn

[J02] 格式化输出
来源：http://rn.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xg.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fp.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uk.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://fz.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zl.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ll.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mg.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wd.newstarts.cn

[J03] 字符串解析为日期
来源：http://hx.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ex.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sp.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://cp.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://xl.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dc.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://il.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://hs.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ku.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ff.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qe.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://it.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uz.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dc.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ax.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tx.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tp.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dt.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://la.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://lp.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fx.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kp.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cp.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://rc.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qz.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://bm.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zn.bjjhwx.cn

[J06] 计算两时间之差
来源：http://nc.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://ow.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ge.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bs.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ta.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zt.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://fs.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ah.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ww.521024.cn

[J07] 比较两个日期
来源：http://ua.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ev.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hn.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nh.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eo.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mf.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zh.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://az.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://th.shxzskj.cn

[J08] 提取年月日与星期
来源：http://nf.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ge.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://em.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hr.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gq.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fg.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uf.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nr.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fe.shtwfgs.cn

[J09] 时区处理
来源：http://ch.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fn.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nv.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sr.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cm.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bs.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qw.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ur.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://dd.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fj.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jp.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://of.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lr.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lo.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dm.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mc.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://td.muxihuayi.cn

================================================================================
来源：http://nx.shxzskj.cn

K. JSON 与序列化
来源：http://ak.colortex.cn

================================================================================
来源：http://ty.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://si.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wb.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kh.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://sv.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://za.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dz.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://rv.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mj.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pv.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ix.nszjky.cn

Py:   json.loads(s)
来源：http://cp.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lc.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://qy.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://ke.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gq.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ag.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://db.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ql.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ld.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ho.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vy.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qq.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hn.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ml.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ak.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tj.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://yw.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fb.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eq.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yk.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jj.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yt.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jj.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ba.huanxung.cn

[K05] 深拷贝对象
来源：http://qi.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://du.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://nl.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://wf.521024.cn

TS:   structuredClone(obj)
来源：http://nm.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ps.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://to.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vn.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yg.521024.cn

[K06] 解析 URL 查询串
来源：http://wh.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tm.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vr.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yl.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ju.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rk.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vw.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jp.haigaiapp.cn


<!-- 参考信息 -->