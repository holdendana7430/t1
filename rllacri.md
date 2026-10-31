代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ul.asd995.cn

Ruby: obj.instance_variables
来源：http://oy.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://ob.chemitech.net.cn

================================================================================
来源：http://kd.shxzskj.cn

H. 异常与错误处理
来源：http://sw.wgjwhj.cn

================================================================================
来源：http://il.muxihuayi.cn

[H01] try / catch 基础
来源：http://ay.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vw.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://og.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://op.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wd.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qn.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://el.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kt.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pg.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://wz.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://by.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xd.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mo.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ny.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mz.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bl.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uu.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://va.hnjuh.cn

[H03] 主动抛出异常
来源：http://ap.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://ue.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jp.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://pn.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://ol.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fe.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kp.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oi.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://al.nicolike.cn

[H04] 自定义异常类型
来源：http://gg.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://ms.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mm.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://xf.colortex.cn

TS:   class MyError extends Error {}
来源：http://en.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://pn.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kb.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://kt.521024.cn

C#:   class MyException : Exception {}
来源：http://qa.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://uk.panjiajie.cn

Py:   except ValueError as e:
来源：http://ap.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zd.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://qb.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://pn.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://ey.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wz.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://xm.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ru.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ll.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cv.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ag.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bg.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jo.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://op.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://xp.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://me.jianghongdianzi.cn

[H07] 断言
来源：http://sn.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ti.shxzskj.cn

PHP:  assert($x > 0);
来源：http://ns.huanxung.cn

JS:   console.assert(x > 0);
来源：http://vw.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://zr.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://oz.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ay.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://am.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://ti.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://oe.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://fx.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tq.shxzukj.cn

JS:   e.message;  e.stack
来源：http://nf.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oq.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fk.huanxung.cn

Go:   err.Error()
来源：http://ry.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://cw.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://uq.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://xz.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mc.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dv.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vv.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gn.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nh.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iv.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tg.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hd.521024.cn

[H10] 资源自动释放
来源：http://vh.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://es.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nb.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hd.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cd.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hh.szsharing.cn

Go:   defer f.Close()
来源：http://dw.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tc.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rn.colortex.cn

================================================================================
来源：http://dv.huixinmuqiang.cn

I. 正则表达式
来源：http://kw.9csxet.cn

================================================================================
来源：http://lt.asd995.cn

[I01] 判断是否匹配
来源：http://du.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xd.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zk.nicolike.cn

JS:   /\d+/.test(s)
来源：http://wt.hahajie.cn

TS:   /\d+/.test(s)
来源：http://pm.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://or.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gh.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://gk.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wg.gzmigu.cn

[I02] 提取所有匹配
来源：http://en.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://uk.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wf.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ht.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://nw.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sw.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sn.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://qa.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gh.521024.cn

[I03] 提取捕获分组
来源：http://fi.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oq.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wk.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fp.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pf.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ru.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hj.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yr.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gp.bjjhwx.cn

[I04] 正则替换
来源：http://ve.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://de.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gm.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ap.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fn.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xy.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uq.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://il.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fu.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://cg.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uk.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pf.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://pe.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://nh.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ot.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sw.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xy.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pu.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://or.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://en.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iw.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://at.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://re.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kn.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qs.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://um.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qt.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://it.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bl.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sv.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bk.shxzskj.cn

TS:   /error/gim
来源：http://ra.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sk.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xv.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://nr.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ev.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://sz.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ds.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nr.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vn.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tg.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ce.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ww.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hc.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uk.newstarts.cn

================================================================================
来源：http://au.nszjky.cn

J. 日期与时间
来源：http://gq.szxytkj.cn

================================================================================
来源：http://iq.bookmarksfly.cn

[J01] 获取当前时间
来源：http://bs.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xi.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://by.asd995.cn

TS:   new Date();  Date.now()
来源：http://vh.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gc.chemitech.net.cn

Go:   time.Now()
来源：http://te.huixinmuqiang.cn

Ruby: Time.now
来源：http://zb.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://en.hnjuh.cn

[J02] 格式化输出
来源：http://ur.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rs.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wi.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://td.huixiangedu.cn

TS:   d.toISOString()
来源：http://pw.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lm.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ex.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ab.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gu.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://sf.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cf.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hl.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://ud.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://qk.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rm.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yd.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://hw.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zt.nicolike.cn

[J04] 时间戳与日期互转
来源：http://vp.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://od.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zd.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ub.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qo.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oh.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fb.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cu.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ib.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://xf.colortex.cn

Py:   now + timedelta(days=7)
来源：http://se.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vh.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tj.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uz.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://yf.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wq.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://zj.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kh.nszjky.cn

[J06] 计算两时间之差
来源：http://up.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://py.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://nq.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uq.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ev.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ee.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://qj.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://lk.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://st.shxzukj.cn

[J07] 比较两个日期
来源：http://tr.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://qy.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tq.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://li.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fn.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sk.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qa.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mp.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://kg.9csxet.cn

[J08] 提取年月日与星期
来源：http://cc.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ej.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qc.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://as.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gt.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ae.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nc.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aj.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ba.muxihuayi.cn

[J09] 时区处理
来源：http://hp.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tr.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://la.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hh.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ok.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uw.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vg.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tw.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ve.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://yo.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fx.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ov.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tr.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yg.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oz.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://be.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zd.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hx.huixiangedu.cn

================================================================================
来源：http://on.jctech888.com.cn

K. JSON 与序列化
来源：http://oi.shxzskj.cn

================================================================================
来源：http://mv.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://ws.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zh.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://te.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ez.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://mc.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tg.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://gn.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fa.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dh.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://vz.shtwfgs.cn

Py:   json.loads(s)
来源：http://es.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fk.lnxyls.cn

JS:   JSON.parse(s)
来源：http://gx.newstarts.cn

TS:   JSON.parse(s)
来源：http://ng.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://os.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ob.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hp.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://pn.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://en.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fz.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qp.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kx.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uq.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ud.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yu.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wp.nszjky.cn

[K04] 读取 JSON 文件
来源：http://xh.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vn.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://be.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zp.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fv.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eq.jctech888.com.cn


<!-- 参考信息 -->