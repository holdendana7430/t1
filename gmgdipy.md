代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://px.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ms.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://up.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fw.muxihuayi.cn

[H03] 主动抛出异常
来源：http://im.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://rh.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://im.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://ow.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://md.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kh.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zd.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gu.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mx.hnjuh.cn

[H04] 自定义异常类型
来源：http://ad.asd995.cn

Py:   class MyError(Exception): pass
来源：http://gu.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ll.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://zs.nicolike.cn

TS:   class MyError extends Error {}
来源：http://pm.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://oz.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nm.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://jm.colortex.cn

C#:   class MyException : Exception {}
来源：http://nn.shxzskj.cn

[H05] 捕获特定类型
来源：http://tk.muxihuayi.cn

Py:   except ValueError as e:
来源：http://xh.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qj.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ws.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://iu.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://on.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zd.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://gt.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wm.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://mx.szsharing.cn

Py:   value = d.get("k") or default
来源：http://uy.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sw.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yh.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wc.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jr.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bo.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://gh.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://gb.huanxung.cn

[H07] 断言
来源：http://cb.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://nq.9csxet.cn

PHP:  assert($x > 0);
来源：http://md.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://qs.nszjky.cn

TS:   console.assert(x > 0);
来源：http://yj.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://hc.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lr.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ag.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://xr.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://jj.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://zs.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tg.huanxung.cn

JS:   e.message;  e.stack
来源：http://sh.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://li.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pj.chemitech.net.cn

Go:   err.Error()
来源：http://dx.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://eb.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://fu.szsharing.cn

[H09] 带错误码的异常
来源：http://ds.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ni.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iu.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rw.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yl.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ab.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hw.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wk.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mu.bjjhwx.cn

[H10] 资源自动释放
来源：http://ie.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ln.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sx.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sj.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nf.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://on.colortex.cn

Go:   defer f.Close()
来源：http://hi.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zm.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tl.newstarts.cn

================================================================================
来源：http://mj.yuexingan06.cn

I. 正则表达式
来源：http://tg.szsharing.cn

================================================================================
来源：http://he.wgjwhj.cn

[I01] 判断是否匹配
来源：http://mb.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pv.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yn.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://hh.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://tq.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://df.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ym.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://iq.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ks.shtwfgs.cn

[I02] 提取所有匹配
来源：http://rh.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://zf.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yv.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zu.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://st.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lb.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kc.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://fg.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mm.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://sm.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ek.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://os.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ff.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dz.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ea.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kd.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://go.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dg.nicolike.cn

[I04] 正则替换
来源：http://ac.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vn.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://je.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://db.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wj.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jw.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ol.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://co.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vh.bookmarksfly.cn

[I05] 按正则拆分
来源：http://ss.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pt.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://py.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://vi.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://hi.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://fv.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cj.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://as.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kv.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ti.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mc.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ia.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cb.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ox.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eq.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xz.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ia.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dx.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://dt.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ou.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ss.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vk.hahajie.cn

TS:   /error/gim
来源：http://bs.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aq.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yp.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://eh.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gk.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yw.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bt.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zj.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lv.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wy.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gs.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ed.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ok.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ul.gzmigu.cn

================================================================================
来源：http://jh.shxzukj.cn

J. 日期与时间
来源：http://tu.bjjhwx.cn

================================================================================
来源：http://as.9csxet.cn

[J01] 获取当前时间
来源：http://cd.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nx.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://do.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://ku.nicolike.cn

TS:   new Date();  Date.now()
来源：http://to.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jn.nszjky.cn

Go:   time.Now()
来源：http://vr.jianghongdianzi.cn

Ruby: Time.now
来源：http://gb.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fj.huixiangedu.cn

[J02] 格式化输出
来源：http://ny.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ng.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ih.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xh.yuexingan06.cn

TS:   d.toISOString()
来源：http://kp.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uz.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tw.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xy.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tt.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://io.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ck.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pk.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://mb.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://kp.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sa.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bb.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://rw.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://es.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://fd.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ap.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://es.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nz.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ns.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jo.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nr.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wf.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rj.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://tx.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://uk.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fk.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vt.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ze.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://yj.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ia.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://xf.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://so.newstarts.cn

[J06] 计算两时间之差
来源：http://bt.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://dp.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://zz.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hj.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kk.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yb.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://us.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ku.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://lq.colortex.cn

[J07] 比较两个日期
来源：http://mu.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://wa.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yp.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fd.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://du.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cv.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ra.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eg.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ef.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ey.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ec.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ap.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bu.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ne.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bh.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ns.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xl.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://av.hnjuh.cn

[J09] 时区处理
来源：http://rb.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xh.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fy.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gu.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hv.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oz.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rn.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wz.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ee.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://dw.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dk.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dg.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gk.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fi.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xq.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://df.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zq.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ui.panjiajie.cn

================================================================================
来源：http://dx.panjiajie.cn

K. JSON 与序列化
来源：http://ul.colortex.cn

================================================================================
来源：http://va.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://tz.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qk.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ps.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ld.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://gq.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lm.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ga.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aa.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fx.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ba.wgjwhj.cn

Py:   json.loads(s)
来源：http://ar.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://su.521024.cn

JS:   JSON.parse(s)
来源：http://hp.colortex.cn

TS:   JSON.parse(s)
来源：http://wc.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fn.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://qw.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://qk.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fa.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://fz.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pm.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tr.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tb.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tg.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fa.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ox.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oy.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://mm.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sd.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ol.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://an.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ic.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mt.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://et.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ok.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fd.lnxyls.cn

[K05] 深拷贝对象
来源：http://jq.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://nq.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://qc.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://as.shxzskj.cn

TS:   structuredClone(obj)
来源：http://yx.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://te.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ar.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qf.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mc.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://qr.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://on.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nh.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hf.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fk.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qo.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fw.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sa.nicolike.cn


<!-- 参考信息 -->