代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hv.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ps.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nf.newstarts.cn

[H02] finally / ensure 收尾
来源：http://zk.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qd.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hb.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qk.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mv.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qg.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ix.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dw.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lt.chemitech.net.cn

[H03] 主动抛出异常
来源：http://iu.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://qk.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qb.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://ne.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://bw.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wl.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hw.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fr.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bp.bjjhwx.cn

[H04] 自定义异常类型
来源：http://hu.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://zt.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qd.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://kc.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://sd.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://ui.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cs.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://ij.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://tp.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://nz.huanxung.cn

Py:   except ValueError as e:
来源：http://zj.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oa.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://oo.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://kp.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://nn.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ml.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ig.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fw.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://hn.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://nz.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vk.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ln.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ga.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ev.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tp.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://ij.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://wj.szsharing.cn

[H07] 断言
来源：http://cs.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://ix.521024.cn

PHP:  assert($x > 0);
来源：http://mu.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://gr.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://gn.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://oq.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yp.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vd.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://un.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://wp.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://br.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pa.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://lf.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mx.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sh.yuntaijiaju.cn

Go:   err.Error()
来源：http://aa.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ei.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://bp.shxzskj.cn

[H09] 带错误码的异常
来源：http://ol.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zm.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ee.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tz.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ey.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jf.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gh.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pl.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qd.shtwfgs.cn

[H10] 资源自动释放
来源：http://xm.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uy.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nu.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ia.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qk.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ob.shxzukj.cn

Go:   defer f.Close()
来源：http://ta.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gc.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wq.muxihuayi.cn

================================================================================
来源：http://ht.huixiangedu.cn

I. 正则表达式
来源：http://xc.gzmigu.cn

================================================================================
来源：http://mv.wgjwhj.cn

[I01] 判断是否匹配
来源：http://fd.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hq.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rm.nszjky.cn

JS:   /\d+/.test(s)
来源：http://le.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://ga.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://px.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xh.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://eh.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ep.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ez.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://pf.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://os.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ob.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ns.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jx.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lz.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://hd.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wc.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ub.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lh.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qx.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ld.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sm.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cx.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sj.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vd.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bf.lnxyls.cn

[I04] 正则替换
来源：http://wz.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rm.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ae.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xc.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ii.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fq.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tj.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eg.shtwfgs.cn

[I05] 按正则拆分
来源：http://xu.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yl.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zx.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vk.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://dr.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://yi.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vf.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pi.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qd.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://li.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uo.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vl.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ny.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sc.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rn.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sc.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yf.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yq.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://qw.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wy.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ay.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fk.colortex.cn

TS:   /error/gim
来源：http://yb.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://br.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eu.colortex.cn

Ruby: s.scan(/error/i)
来源：http://gj.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oq.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://cr.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jm.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://du.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mx.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rb.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ft.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://si.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xg.nicolike.cn

================================================================================
来源：http://fw.asd995.cn

J. 日期与时间
来源：http://nc.wgjwhj.cn

================================================================================
来源：http://fr.521024.cn

[J01] 获取当前时间
来源：http://ri.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ak.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://us.nicolike.cn

JS:   new Date();  Date.now()
来源：http://ym.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://wy.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ma.shxzskj.cn

Go:   time.Now()
来源：http://bw.asd995.cn

Ruby: Time.now
来源：http://wo.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sm.nicolike.cn

[J02] 格式化输出
来源：http://ss.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://io.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wr.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ro.hahajie.cn

TS:   d.toISOString()
来源：http://jk.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tq.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nq.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zi.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dw.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ch.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dn.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kv.asd995.cn

JS:   new Date("2024-01-02")
来源：http://oe.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://nv.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fr.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ju.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://hq.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://og.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://am.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vm.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://za.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://es.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jj.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bd.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lq.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ps.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://jh.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://xb.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fh.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jt.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://md.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://dm.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fg.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://mq.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fj.wgjwhj.cn

[J06] 计算两时间之差
来源：http://un.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://yg.521024.cn

PHP:  $end->diff($start)->days;
来源：http://tt.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://he.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jx.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://si.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://ke.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hq.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://hp.521024.cn

[J07] 比较两个日期
来源：http://lk.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ze.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kw.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zl.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ov.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fb.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ys.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lr.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://vn.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ad.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mx.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oj.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ax.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qr.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lt.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rt.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ac.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vw.szsharing.cn

[J09] 时区处理
来源：http://cx.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sq.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uj.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fp.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sr.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fp.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://on.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ml.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://fb.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nf.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ew.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cy.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://un.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fq.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ow.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ha.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hj.wgjwhj.cn

================================================================================
来源：http://fs.haigaiapp.cn

K. JSON 与序列化
来源：http://wt.nicolike.cn

================================================================================
来源：http://km.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://xc.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yn.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ig.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://jb.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://nb.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://of.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://fz.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fr.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sk.huanxung.cn

[K02] JSON 字符串转对象
来源：http://wm.wgjwhj.cn

Py:   json.loads(s)
来源：http://mn.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jh.hahajie.cn

JS:   JSON.parse(s)
来源：http://vp.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://pk.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ta.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://qn.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ew.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iw.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ff.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sj.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rq.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fn.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://li.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oe.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hc.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pi.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ft.521024.cn

[K04] 读取 JSON 文件
来源：http://dr.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ky.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pc.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rh.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kt.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yr.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pc.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bu.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lv.bjjhwx.cn

[K05] 深拷贝对象
来源：http://lv.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://se.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ml.gzmigu.cn

JS:   structuredClone(obj)
来源：http://rl.panjiajie.cn

TS:   structuredClone(obj)
来源：http://il.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vd.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ai.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bl.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://il.nicolike.cn


<!-- 参考信息 -->