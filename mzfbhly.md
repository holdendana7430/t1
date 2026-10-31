代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://be.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ps.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vm.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://mo.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xv.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qx.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ly.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nl.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ls.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://db.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ji.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://og.huanxung.cn

[H03] 主动抛出异常
来源：http://pf.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://dl.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ik.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://wz.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://ae.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://up.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ju.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ht.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mw.nszjky.cn

[H04] 自定义异常类型
来源：http://hq.asd995.cn

Py:   class MyError(Exception): pass
来源：http://cz.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oo.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://je.nicolike.cn

TS:   class MyError extends Error {}
来源：http://zv.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://ny.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oa.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://vn.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://iz.huixiangedu.cn

[H05] 捕获特定类型
来源：http://qm.colortex.cn

Py:   except ValueError as e:
来源：http://ya.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ga.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://uv.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://qv.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://gu.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mk.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://nb.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zv.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://sw.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://yc.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://et.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wa.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ia.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wb.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zi.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://kk.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://dp.bookmarksfly.cn

[H07] 断言
来源：http://xp.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://tj.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://su.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ox.szsharing.cn

TS:   console.assert(x > 0);
来源：http://pq.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://lq.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xz.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ol.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://wf.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://vo.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://de.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tj.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://om.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://is.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://io.hnjuh.cn

Go:   err.Error()
来源：http://ke.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://gb.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://wk.hnjuh.cn

[H09] 带错误码的异常
来源：http://pj.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pn.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dx.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gj.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://av.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gb.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ol.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sv.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fv.shxzukj.cn

[H10] 资源自动释放
来源：http://nn.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dc.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sb.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jw.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xf.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dv.shxzskj.cn

Go:   defer f.Close()
来源：http://ch.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jj.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rn.szxytkj.cn

================================================================================
来源：http://ju.newstarts.cn

I. 正则表达式
来源：http://xl.szxytkj.cn

================================================================================
来源：http://gb.chemitech.net.cn

[I01] 判断是否匹配
来源：http://an.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gc.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zu.nszjky.cn

JS:   /\d+/.test(s)
来源：http://sz.nszjky.cn

TS:   /\d+/.test(s)
来源：http://nk.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wt.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bl.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://tq.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gs.chemitech.net.cn

[I02] 提取所有匹配
来源：http://qn.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://zi.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hn.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ax.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://nm.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vi.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pr.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://ld.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fx.huanxung.cn

[I03] 提取捕获分组
来源：http://ec.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rw.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xf.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zn.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ot.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cu.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wo.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zv.muxihuayi.cn

[I04] 正则替换
来源：http://ri.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yf.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ro.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ih.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tl.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dw.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ku.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://go.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vl.521024.cn

[I05] 按正则拆分
来源：http://vr.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yw.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sw.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nz.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://le.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://yb.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dt.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yr.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vh.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hv.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mx.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sd.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mi.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fs.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ru.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cd.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fm.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pj.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://ap.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://at.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ws.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zf.szxytkj.cn

TS:   /error/gim
来源：http://xv.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ka.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tu.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://cg.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fo.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://hg.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sa.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zn.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wd.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vq.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ll.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rm.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yj.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ty.wgjwhj.cn

================================================================================
来源：http://tc.hahajie.cn

J. 日期与时间
来源：http://ow.asd995.cn

================================================================================
来源：http://uy.muxihuayi.cn

[J01] 获取当前时间
来源：http://zf.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hk.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cn.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://lw.colortex.cn

TS:   new Date();  Date.now()
来源：http://ge.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ts.szxytkj.cn

Go:   time.Now()
来源：http://ra.huixiangedu.cn

Ruby: Time.now
来源：http://ti.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pe.hahajie.cn

[J02] 格式化输出
来源：http://jb.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hx.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uk.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nq.muxihuayi.cn

TS:   d.toISOString()
来源：http://uq.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nn.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wj.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iq.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sd.szxytkj.cn

[J03] 字符串解析为日期
来源：http://kn.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://is.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xp.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://nb.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://fz.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bv.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hk.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://tm.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ad.colortex.cn

[J04] 时间戳与日期互转
来源：http://wo.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gm.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zo.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://km.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yp.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ho.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uq.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ij.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nv.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://gc.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://fj.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qj.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ni.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vu.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://zw.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yd.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://re.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ib.huixiangedu.cn

[J06] 计算两时间之差
来源：http://vs.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://oi.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ox.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zp.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sw.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ei.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://pb.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://cy.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://dr.wgjwhj.cn

[J07] 比较两个日期
来源：http://kk.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://it.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ej.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ak.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lv.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qw.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bh.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nz.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://qz.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://al.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://me.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jg.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tf.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yt.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zp.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://es.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dw.9csxet.cn

[J09] 时区处理
来源：http://nc.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://na.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://np.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bc.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wc.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pn.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ox.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yz.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xk.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://hw.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://js.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tp.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qv.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jk.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hy.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nq.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ez.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xw.huixiangedu.cn

================================================================================
来源：http://dh.hnjuh.cn

K. JSON 与序列化
来源：http://jk.jianghongdianzi.cn

================================================================================
来源：http://vk.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://sa.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yp.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pf.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://mf.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://je.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mc.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://rd.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rp.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pj.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://mn.huanxung.cn

Py:   json.loads(s)
来源：http://qx.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lf.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://on.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://kn.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://po.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ln.newstarts.cn

Ruby: JSON.parse(s)
来源：http://kg.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ic.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://gp.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qx.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nr.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ev.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tz.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fn.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ft.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iu.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ah.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://wi.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wo.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zy.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wm.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rw.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wn.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cv.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zs.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rp.muxihuayi.cn

[K05] 深拷贝对象
来源：http://mi.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://vn.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://uw.newstarts.cn

JS:   structuredClone(obj)
来源：http://wr.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://uv.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zm.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bf.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bt.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yp.lnxyls.cn


<!-- 参考信息 -->