代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://mf.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eq.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ji.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bj.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tn.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lv.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wn.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ut.chemitech.net.cn

[H03] 主动抛出异常
来源：http://sf.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://zn.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iq.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://vm.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://np.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jy.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ja.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sf.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wc.bjjhwx.cn

[H04] 自定义异常类型
来源：http://di.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://vv.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hq.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://sj.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://kd.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://mc.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://id.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://td.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://rc.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://ni.muxihuayi.cn

Py:   except ValueError as e:
来源：http://rh.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xd.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://fw.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://nj.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://tg.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ga.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://bn.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://of.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ks.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://hx.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ey.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yn.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mk.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://de.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://us.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://zb.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://ug.huixiangedu.cn

[H07] 断言
来源：http://ua.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://xw.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://bg.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://kc.hahajie.cn

TS:   console.assert(x > 0);
来源：http://ap.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://li.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ae.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xc.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://iz.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://le.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://we.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lg.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://oj.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://np.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nm.bookmarksfly.cn

Go:   err.Error()
来源：http://sh.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://vv.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://rm.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://yo.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fk.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xa.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wq.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://na.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xz.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zh.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://om.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lv.nicolike.cn

[H10] 资源自动释放
来源：http://bo.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aj.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yl.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lc.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pv.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ry.hnjuh.cn

Go:   defer f.Close()
来源：http://ci.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bc.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dr.nicolike.cn

================================================================================
来源：http://zw.hnjuh.cn

I. 正则表达式
来源：http://nx.bjjhwx.cn

================================================================================
来源：http://fy.szxytkj.cn

[I01] 判断是否匹配
来源：http://xr.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ax.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://df.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ws.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://ab.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vq.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fm.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://sp.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hi.muxihuayi.cn

[I02] 提取所有匹配
来源：http://dr.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://zw.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rz.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mw.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://ew.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gz.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fr.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://mc.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ma.hnjuh.cn

[I03] 提取捕获分组
来源：http://wm.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nt.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qh.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wa.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qw.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zo.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nu.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vc.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bs.szxytkj.cn

[I04] 正则替换
来源：http://fm.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vf.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wk.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uk.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fe.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pm.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hx.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mm.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://km.521024.cn

[I05] 按正则拆分
来源：http://vg.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rh.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ly.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://nm.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://az.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://ud.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dz.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mx.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iw.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cs.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qg.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://di.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vi.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ti.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://os.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xy.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jo.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sh.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://hd.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nn.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ji.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gb.panjiajie.cn

TS:   /error/gim
来源：http://vl.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wj.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lk.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://xx.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rv.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://os.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cn.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qf.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ci.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://si.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oy.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mq.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gx.shtwfgs.cn

================================================================================
来源：http://cc.yuexingan06.cn

J. 日期与时间
来源：http://dz.huixiangedu.cn

================================================================================
来源：http://iu.haigaiapp.cn

[J01] 获取当前时间
来源：http://ff.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://su.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://te.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://yo.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://ng.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jd.huixinmuqiang.cn

Go:   time.Now()
来源：http://nf.9csxet.cn

Ruby: Time.now
来源：http://fr.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rm.gzmigu.cn

[J02] 格式化输出
来源：http://ue.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rc.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pf.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kr.jctech888.com.cn

TS:   d.toISOString()
来源：http://pg.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wn.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kh.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ce.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sh.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://uv.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wx.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vv.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://fi.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://rz.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rx.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uh.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://ju.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aj.521024.cn

[J04] 时间戳与日期互转
来源：http://iq.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fd.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fk.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://np.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gq.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://we.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vq.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bu.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dh.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://sa.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://qj.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tk.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gu.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dn.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://rs.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rh.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://cg.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mb.wgjwhj.cn

[J06] 计算两时间之差
来源：http://mo.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://su.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ud.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pu.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lt.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ld.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://xi.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://cv.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://cl.bjjhwx.cn

[J07] 比较两个日期
来源：http://hk.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ij.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pp.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xj.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bq.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wc.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://io.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zp.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://yb.huanxung.cn

[J08] 提取年月日与星期
来源：http://wd.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ur.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ow.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tb.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fa.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://av.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vv.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ga.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wj.nicolike.cn

[J09] 时区处理
来源：http://zs.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vg.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fv.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ji.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nn.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wq.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ln.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nw.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hd.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://fu.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ou.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zf.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ui.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xc.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ei.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://az.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gn.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vv.yuexingan06.cn

================================================================================
来源：http://ty.shtwfgs.cn

K. JSON 与序列化
来源：http://vg.nicolike.cn

================================================================================
来源：http://ro.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://wd.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zp.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://em.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://dn.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ba.nszjky.cn

Go:   json.Marshal(obj)
来源：http://rg.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hn.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ua.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://sl.newstarts.cn

Py:   json.loads(s)
来源：http://kn.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ej.9csxet.cn

JS:   JSON.parse(s)
来源：http://ne.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://lx.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wb.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://ha.521024.cn

Ruby: JSON.parse(s)
来源：http://iz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://er.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://qn.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ou.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ai.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nk.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yi.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ev.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dh.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://re.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oe.nicolike.cn

[K04] 读取 JSON 文件
来源：http://vg.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nw.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vc.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zn.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wr.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ct.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nh.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://of.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zu.yuexingan06.cn

[K05] 深拷贝对象
来源：http://xe.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://db.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://ar.shxzukj.cn

JS:   structuredClone(obj)
来源：http://no.panjiajie.cn

TS:   structuredClone(obj)
来源：http://oh.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yn.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kp.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vw.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nq.huanxung.cn

[K06] 解析 URL 查询串
来源：http://qg.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hv.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ts.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qf.newstarts.cn


<!-- 参考信息 -->