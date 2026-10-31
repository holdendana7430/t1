代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ug.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kq.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://od.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ry.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ue.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xs.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://md.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://oo.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gr.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gx.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kx.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fa.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ax.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://me.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hp.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rr.nszjky.cn

[H03] 主动抛出异常
来源：http://vr.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://yk.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://to.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://jp.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://bo.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tq.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ib.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qa.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aa.shtwfgs.cn

[H04] 自定义异常类型
来源：http://mj.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://va.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nt.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://bd.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://qa.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ml.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ux.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://uz.hahajie.cn

C#:   class MyException : Exception {}
来源：http://ts.lnxyls.cn

[H05] 捕获特定类型
来源：http://sh.asd995.cn

Py:   except ValueError as e:
来源：http://ep.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mf.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://ey.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://fl.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://cl.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ks.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://dg.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://an.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ke.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://sp.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ge.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lt.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dm.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qd.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sd.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://of.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://kf.yuntaijiaju.cn

[H07] 断言
来源：http://za.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://lr.hahajie.cn

PHP:  assert($x > 0);
来源：http://tk.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://ki.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://bd.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://cc.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vr.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://le.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://fa.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://xl.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://fg.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://my.panjiajie.cn

JS:   e.message;  e.stack
来源：http://ke.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ro.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uc.jianghongdianzi.cn

Go:   err.Error()
来源：http://ax.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://qd.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://xf.chemitech.net.cn

[H09] 带错误码的异常
来源：http://nk.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ff.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qe.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://du.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pc.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ad.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eo.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xd.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ve.jctech888.com.cn

[H10] 资源自动释放
来源：http://dz.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ie.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qn.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lc.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://du.nszjky.cn

Go:   defer f.Close()
来源：http://dy.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nf.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ud.colortex.cn

================================================================================
来源：http://lb.newstarts.cn

I. 正则表达式
来源：http://de.newstarts.cn

================================================================================
来源：http://om.9csxet.cn

[I01] 判断是否匹配
来源：http://ss.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oc.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ap.hahajie.cn

JS:   /\d+/.test(s)
来源：http://vr.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://mb.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xr.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tz.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://oh.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tc.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://mt.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://zq.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vz.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tl.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://by.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lu.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kj.521024.cn

Ruby: s.scan(/\d+/)
来源：http://gq.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ei.muxihuayi.cn

[I03] 提取捕获分组
来源：http://xg.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ic.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vn.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gn.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gz.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ae.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gx.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ff.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://da.521024.cn

[I04] 正则替换
来源：http://yh.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mx.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oa.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eq.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hd.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yx.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yj.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dk.huixiangedu.cn

[I05] 按正则拆分
来源：http://ds.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hf.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eu.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://df.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ap.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://gt.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ha.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jx.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jv.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bv.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ym.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kd.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yu.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mq.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xq.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kg.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hx.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wt.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://rj.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lt.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sv.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qa.huixiangedu.cn

TS:   /error/gim
来源：http://uv.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://df.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fx.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://av.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ym.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://an.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lm.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gt.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hl.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ge.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://og.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kp.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pt.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pu.bookmarksfly.cn

================================================================================
来源：http://qa.nszjky.cn

J. 日期与时间
来源：http://zi.chemitech.net.cn

================================================================================
来源：http://mi.hahajie.cn

[J01] 获取当前时间
来源：http://hy.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dn.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tk.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://dq.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://oa.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bg.hnjuh.cn

Go:   time.Now()
来源：http://gr.gzmigu.cn

Ruby: Time.now
来源：http://ba.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ax.szsharing.cn

[J02] 格式化输出
来源：http://de.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nh.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ff.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://or.nicolike.cn

TS:   d.toISOString()
来源：http://iu.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mx.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wb.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ce.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kd.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://qx.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ak.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xv.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://hp.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://wl.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pq.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yi.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://eq.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ej.hahajie.cn

[J04] 时间戳与日期互转
来源：http://hz.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bo.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jl.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vn.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ew.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lc.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ju.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tw.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ay.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://sb.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://ip.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://do.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ma.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xy.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://lf.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cs.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://wl.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jw.szsharing.cn

[J06] 计算两时间之差
来源：http://ll.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://hq.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://cj.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ln.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ql.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ss.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ux.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ai.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ts.gzmigu.cn

[J07] 比较两个日期
来源：http://dv.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://vj.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ct.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ij.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vu.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sh.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tx.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hg.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ta.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://fk.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://to.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://js.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://co.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dy.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ta.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://em.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xl.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ha.521024.cn

[J09] 时区处理
来源：http://iv.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bk.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://to.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ds.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pp.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tn.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yn.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fl.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://va.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://ln.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vy.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vc.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dn.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qm.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://th.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rz.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gh.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ib.panjiajie.cn

================================================================================
来源：http://ar.asd995.cn

K. JSON 与序列化
来源：http://ak.bookmarksfly.cn

================================================================================
来源：http://yv.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://qo.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://si.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yq.521024.cn

JS:   JSON.stringify(obj)
来源：http://rz.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://sq.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mk.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://tl.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ki.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://my.521024.cn

[K02] JSON 字符串转对象
来源：http://il.shxzskj.cn

Py:   json.loads(s)
来源：http://id.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://th.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://sa.hnjuh.cn

TS:   JSON.parse(s)
来源：http://te.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sj.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ey.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://pm.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yf.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://dh.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uy.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ik.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dc.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://on.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vb.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ms.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qb.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pf.521024.cn

[K04] 读取 JSON 文件
来源：http://rs.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://id.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gt.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ly.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kg.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ls.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uv.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cr.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wv.szsharing.cn

[K05] 深拷贝对象
来源：http://ok.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://bh.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://qh.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://qq.newstarts.cn

TS:   structuredClone(obj)
来源：http://ez.yuexingan06.cn


<!-- 参考信息 -->