代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zx.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fz.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gb.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://pa.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ps.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wg.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tc.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iq.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://md.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://so.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wq.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jb.shxzukj.cn

[H03] 主动抛出异常
来源：http://wu.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://da.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qx.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ez.521024.cn

TS:   throw new Error("错误信息");
来源：http://nl.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ki.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fg.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wd.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pa.bjjhwx.cn

[H04] 自定义异常类型
来源：http://do.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://xh.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fe.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://lv.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://mo.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://kn.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vw.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://px.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://od.nicolike.cn

[H05] 捕获特定类型
来源：http://tj.huixiangedu.cn

Py:   except ValueError as e:
来源：http://br.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tx.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://yu.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://vm.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ea.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ay.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://od.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qy.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://ge.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://xi.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ly.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mn.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xb.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mc.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ud.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://zp.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://re.yuntaijiaju.cn

[H07] 断言
来源：http://it.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://kr.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://ey.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://zr.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://tb.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://tl.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://to.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ce.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://jk.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://fy.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ls.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ws.szxytkj.cn

JS:   e.message;  e.stack
来源：http://yi.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vx.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zz.yuexingan06.cn

Go:   err.Error()
来源：http://xy.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://ry.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://xm.hnjuh.cn

[H09] 带错误码的异常
来源：http://zi.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vr.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://al.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gm.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://da.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ud.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sa.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vr.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kj.521024.cn

[H10] 资源自动释放
来源：http://hr.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vs.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ej.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xo.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xg.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://em.bjjhwx.cn

Go:   defer f.Close()
来源：http://gm.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://si.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vq.asd995.cn

================================================================================
来源：http://nw.yuntaijiaju.cn

I. 正则表达式
来源：http://vm.yuexingan06.cn

================================================================================
来源：http://sp.lnxyls.cn

[I01] 判断是否匹配
来源：http://ws.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ay.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://am.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://gh.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://nm.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zf.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zj.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://oe.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ub.jctech888.com.cn

[I02] 提取所有匹配
来源：http://dg.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://vg.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jm.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wq.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://he.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://im.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dt.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://pu.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://un.colortex.cn

[I03] 提取捕获分组
来源：http://kh.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jh.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jt.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vq.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sc.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dq.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rg.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mp.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uq.yuexingan06.cn

[I04] 正则替换
来源：http://vk.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xt.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fz.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sv.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dn.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rt.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://et.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sv.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cd.panjiajie.cn

[I05] 按正则拆分
来源：http://ig.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ez.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://an.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://rc.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ev.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://xp.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cu.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qj.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yv.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vd.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://on.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uy.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ya.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zc.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dp.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mf.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ty.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://zc.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bi.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zz.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://li.muxihuayi.cn

TS:   /error/gim
来源：http://ce.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yi.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xc.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://cm.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xn.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ix.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bc.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gr.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uw.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vw.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pm.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ew.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gi.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wp.szxytkj.cn

================================================================================
来源：http://du.bjjhwx.cn

J. 日期与时间
来源：http://al.9csxet.cn

================================================================================
来源：http://bd.nszjky.cn

[J01] 获取当前时间
来源：http://ls.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lz.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ch.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://eg.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://hq.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ij.shtwfgs.cn

Go:   time.Now()
来源：http://ny.newstarts.cn

Ruby: Time.now
来源：http://tw.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ow.jctech888.com.cn

[J02] 格式化输出
来源：http://ax.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kb.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sa.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dw.hahajie.cn

TS:   d.toISOString()
来源：http://oa.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yj.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yt.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://as.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wq.gzmigu.cn

[J03] 字符串解析为日期
来源：http://go.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xj.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jm.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://cf.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://hj.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fb.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qs.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://gu.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rt.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://tq.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lz.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ql.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ov.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oo.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ih.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pz.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ya.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ti.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://xc.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://hd.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dh.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dq.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rt.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://tl.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pt.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://rr.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wo.shxzskj.cn

[J06] 计算两时间之差
来源：http://ez.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://bi.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://wq.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://du.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eg.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://go.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://dj.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://cc.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ss.newstarts.cn

[J07] 比较两个日期
来源：http://mm.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hb.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ix.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mp.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sg.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pj.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ug.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cr.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yc.huanxung.cn

[J08] 提取年月日与星期
来源：http://tv.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fm.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://au.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tk.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qm.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lq.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://il.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mm.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fb.colortex.cn

[J09] 时区处理
来源：http://su.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cm.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mz.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://em.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bs.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fn.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ju.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ci.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ck.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://cy.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://za.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sl.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hn.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://se.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aa.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ma.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qd.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ci.chemitech.net.cn

================================================================================
来源：http://tv.bjjhwx.cn

K. JSON 与序列化
来源：http://vi.shtwfgs.cn

================================================================================
来源：http://ur.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://xe.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jv.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hn.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://nv.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://dt.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zd.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://fi.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ua.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://if.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://qs.jctech888.com.cn

Py:   json.loads(s)
来源：http://ys.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cw.szxytkj.cn

JS:   JSON.parse(s)
来源：http://an.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://tj.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://io.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://fz.nicolike.cn

Ruby: JSON.parse(s)
来源：http://il.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kl.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://sy.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dz.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gp.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gq.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mk.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ab.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hn.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://me.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sr.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://rr.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vs.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bx.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dt.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xh.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mc.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sz.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ga.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://si.hahajie.cn

[K05] 深拷贝对象
来源：http://iz.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://kv.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://gv.lnxyls.cn

JS:   structuredClone(obj)
来源：http://fa.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://qz.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qd.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gz.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lx.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jy.colortex.cn


<!-- 参考信息 -->