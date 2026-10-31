代发 wailian999

H. 异常与错误处理
来源：http://fk.shtwfgs.cn

================================================================================
来源：http://sw.lnxyls.cn

[H01] try / catch 基础
来源：http://oy.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ap.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bv.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hu.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://me.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yi.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gd.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://me.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kd.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://fm.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gf.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uv.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cu.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ka.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zp.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bl.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uk.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pr.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://rr.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://oi.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://di.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://cr.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://ht.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fv.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mf.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mu.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yo.jctech888.com.cn

[H04] 自定义异常类型
来源：http://iw.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://sa.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ye.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://tz.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://zv.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://gb.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nz.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://dy.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://jn.wgjwhj.cn

[H05] 捕获特定类型
来源：http://qq.shxzskj.cn

Py:   except ValueError as e:
来源：http://uo.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nl.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://rg.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://aq.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://yi.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ki.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://ii.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://js.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://js.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://kc.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jc.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uw.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kj.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wc.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pn.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ez.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ea.shxzskj.cn

[H07] 断言
来源：http://sa.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://qa.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://hq.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://nt.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://mv.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://oo.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lv.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rd.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ht.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://tr.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://bv.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dm.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://hh.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ns.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ji.nicolike.cn

Go:   err.Error()
来源：http://iy.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://xe.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://ho.szxytkj.cn

[H09] 带错误码的异常
来源：http://fb.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gb.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kg.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sx.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hq.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hs.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nj.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sz.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zl.shxzukj.cn

[H10] 资源自动释放
来源：http://yi.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xo.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hk.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lu.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mi.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bz.haigaiapp.cn

Go:   defer f.Close()
来源：http://yz.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tk.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qu.shtwfgs.cn

================================================================================
来源：http://vb.szsharing.cn

I. 正则表达式
来源：http://dd.huanxung.cn

================================================================================
来源：http://cq.huanxung.cn

[I01] 判断是否匹配
来源：http://tq.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mw.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ol.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://xx.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://pz.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mt.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dr.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://hf.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xj.panjiajie.cn

[I02] 提取所有匹配
来源：http://lm.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ky.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xc.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xt.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://rk.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tn.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kk.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://yh.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wj.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ig.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pi.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ou.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vc.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qu.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yz.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sq.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ry.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vn.newstarts.cn

[I04] 正则替换
来源：http://go.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ja.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pb.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://er.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cx.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nc.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ts.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://en.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wo.521024.cn

[I05] 按正则拆分
来源：http://ep.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zs.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://if.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://qc.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://jt.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://eb.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tt.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pv.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hj.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bc.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bx.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qy.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qc.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://px.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ri.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ll.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bn.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://jp.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yj.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tp.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zx.huanxung.cn

TS:   /error/gim
来源：http://go.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qi.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jn.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://bs.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xh.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://am.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://af.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wy.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ml.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ix.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uw.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iq.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ep.huanxung.cn

================================================================================
来源：http://qx.shxzukj.cn

J. 日期与时间
来源：http://et.nicolike.cn

================================================================================
来源：http://ju.shxzukj.cn

[J01] 获取当前时间
来源：http://xb.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kg.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fl.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://gm.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://bv.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wh.bookmarksfly.cn

Go:   time.Now()
来源：http://it.shxzskj.cn

Ruby: Time.now
来源：http://wg.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xy.nicolike.cn

[J02] 格式化输出
来源：http://yg.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://le.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wf.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.shtwfgs.cn

TS:   d.toISOString()
来源：http://co.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ya.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nl.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vf.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cm.9csxet.cn

[J03] 字符串解析为日期
来源：http://ar.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sq.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ml.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://xu.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://jc.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fh.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lj.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://dc.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://so.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://us.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ha.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qo.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jz.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wy.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gu.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yj.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ve.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://de.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://gs.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://mb.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ut.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zd.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dj.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://qt.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://th.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://it.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gb.muxihuayi.cn

[J06] 计算两时间之差
来源：http://qh.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://uc.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://vy.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pv.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fm.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dr.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://vd.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://ks.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ki.chemitech.net.cn

[J07] 比较两个日期
来源：http://ul.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ba.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pn.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://is.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mo.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nq.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pw.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xu.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://pi.nszjky.cn

[J08] 提取年月日与星期
来源：http://fo.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ci.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ml.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oz.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zt.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ei.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nv.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zv.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://py.chemitech.net.cn

[J09] 时区处理
来源：http://wb.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gp.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jp.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dz.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xf.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://va.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vo.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ca.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pp.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://un.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sb.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dg.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rt.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ty.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vt.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://el.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nw.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uz.hahajie.cn

================================================================================
来源：http://ni.newstarts.cn

K. JSON 与序列化
来源：http://bg.lnxyls.cn

================================================================================
来源：http://ll.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://st.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yc.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aa.colortex.cn

JS:   JSON.stringify(obj)
来源：http://xs.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://mk.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oc.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://wi.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vg.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ub.nicolike.cn

[K02] JSON 字符串转对象
来源：http://ab.hahajie.cn

Py:   json.loads(s)
来源：http://zr.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jq.hnjuh.cn

JS:   JSON.parse(s)
来源：http://yl.gzmigu.cn

TS:   JSON.parse(s)
来源：http://qn.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jg.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://vy.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://fn.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zl.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://ld.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vi.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yd.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rn.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://im.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://or.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zs.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://da.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uz.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://hd.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ma.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uo.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xv.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rk.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ei.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ub.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://in.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cn.muxihuayi.cn

[K05] 深拷贝对象
来源：http://kb.lnxyls.cn


<!-- 参考信息 -->