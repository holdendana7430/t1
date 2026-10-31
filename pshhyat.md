代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ie.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://af.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wy.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://dz.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wf.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ol.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ra.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yd.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yx.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zt.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iv.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cd.huanxung.cn

[H03] 主动抛出异常
来源：http://fm.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://rb.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ed.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://ch.colortex.cn

TS:   throw new Error("错误信息");
来源：http://mr.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nq.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lf.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hq.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dw.colortex.cn

[H04] 自定义异常类型
来源：http://bx.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://uk.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ot.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://fl.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://am.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://dw.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sy.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://ei.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://nd.shxzukj.cn

[H05] 捕获特定类型
来源：http://jk.bjjhwx.cn

Py:   except ValueError as e:
来源：http://um.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mr.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://yu.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://iv.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://eb.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bo.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://cu.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xy.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://it.nicolike.cn

Py:   value = d.get("k") or default
来源：http://qh.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xa.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yu.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vs.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://or.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://us.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://xr.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://dg.szxytkj.cn

[H07] 断言
来源：http://tf.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ha.newstarts.cn

PHP:  assert($x > 0);
来源：http://rq.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://co.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://wi.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://bd.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zl.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fi.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://of.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://bz.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://wf.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://np.521024.cn

JS:   e.message;  e.stack
来源：http://en.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qe.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ic.bookmarksfly.cn

Go:   err.Error()
来源：http://ev.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://sm.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://qy.9csxet.cn

[H09] 带错误码的异常
来源：http://qk.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rd.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qf.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ob.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yk.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mm.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://se.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tm.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wo.szsharing.cn

[H10] 资源自动释放
来源：http://fm.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://he.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yf.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://in.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sx.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ig.asd995.cn

Go:   defer f.Close()
来源：http://gm.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xu.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xh.chemitech.net.cn

================================================================================
来源：http://gp.521024.cn

I. 正则表达式
来源：http://is.szsharing.cn

================================================================================
来源：http://rm.521024.cn

[I01] 判断是否匹配
来源：http://sd.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://io.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fb.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://lv.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://sd.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://io.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hv.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://ur.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jw.panjiajie.cn

[I02] 提取所有匹配
来源：http://mn.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://io.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://id.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xr.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://bk.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://od.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mh.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://kt.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rg.hnjuh.cn

[I03] 提取捕获分组
来源：http://al.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hi.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xy.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ze.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pt.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kv.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jq.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dg.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ad.haigaiapp.cn

[I04] 正则替换
来源：http://dv.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lb.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fp.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jz.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cd.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jo.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sg.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xs.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://go.jctech888.com.cn

[I05] 按正则拆分
来源：http://ry.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qq.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ec.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://yz.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://fe.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://el.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dx.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vl.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zb.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ft.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qy.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rp.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qh.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ih.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lc.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dx.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uu.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://au.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://wr.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zo.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wg.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bo.huanxung.cn

TS:   /error/gim
来源：http://di.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oh.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cu.asd995.cn

Ruby: s.scan(/error/i)
来源：http://oq.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vi.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ie.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://od.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mp.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://df.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sb.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ju.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eq.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ma.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://up.jctech888.com.cn

================================================================================
来源：http://ya.chemitech.net.cn

J. 日期与时间
来源：http://fk.nszjky.cn

================================================================================
来源：http://zu.shxzukj.cn

[J01] 获取当前时间
来源：http://uf.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ci.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ar.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://on.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ks.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fr.bjjhwx.cn

Go:   time.Now()
来源：http://nz.yuntaijiaju.cn

Ruby: Time.now
来源：http://ar.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://se.jctech888.com.cn

[J02] 格式化输出
来源：http://rb.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gh.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bh.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uw.chemitech.net.cn

TS:   d.toISOString()
来源：http://sa.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ms.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ua.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qw.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yk.colortex.cn

[J03] 字符串解析为日期
来源：http://do.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ab.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mh.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://pq.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://ga.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ra.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vu.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://fu.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mz.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://wl.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tj.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vk.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oc.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pl.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yq.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rd.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jx.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://if.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://zi.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://yd.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cg.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tz.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bu.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ty.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pm.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://tz.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ya.hnjuh.cn

[J06] 计算两时间之差
来源：http://bv.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://lj.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://fp.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zf.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oj.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xf.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://fu.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://jx.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://qr.huixiangedu.cn

[J07] 比较两个日期
来源：http://mh.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ss.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pf.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rw.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ob.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nz.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kk.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yc.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://hw.hnjuh.cn

[J08] 提取年月日与星期
来源：http://xj.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pz.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://io.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://db.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qn.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tv.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wr.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hx.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tq.szxytkj.cn

[J09] 时区处理
来源：http://vr.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yd.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pf.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nx.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kt.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://si.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://go.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bc.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://qa.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mn.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bb.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zu.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rz.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qp.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mr.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sp.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yf.newstarts.cn

================================================================================
来源：http://lj.hnjuh.cn

K. JSON 与序列化
来源：http://eb.huixinmuqiang.cn

================================================================================
来源：http://ef.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://kf.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yx.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tj.colortex.cn

JS:   JSON.stringify(obj)
来源：http://fp.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://pd.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lq.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://jo.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ku.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cn.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://tz.huixiangedu.cn

Py:   json.loads(s)
来源：http://nq.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vc.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://rb.shxzukj.cn

TS:   JSON.parse(s)
来源：http://yi.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://li.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://it.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ou.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://js.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ri.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ns.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ff.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xt.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pc.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oh.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lk.9csxet.cn

[K04] 读取 JSON 文件
来源：http://vg.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ws.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sv.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kb.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://db.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://km.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fl.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nw.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zx.nicolike.cn

[K05] 深拷贝对象
来源：http://ug.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://ef.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://du.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://jo.nicolike.cn

TS:   structuredClone(obj)
来源：http://mc.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mc.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gh.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xg.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qe.hahajie.cn


<!-- 参考信息 -->