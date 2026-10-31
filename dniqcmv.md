代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://wq.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ix.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://ra.asd995.cn

================================================================================
来源：http://fp.lnxyls.cn

H. 异常与错误处理
来源：http://fz.shxzukj.cn

================================================================================
来源：http://qs.jctech888.com.cn

[H01] try / catch 基础
来源：http://fu.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://se.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xp.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hf.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aq.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tz.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xi.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fq.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qc.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://lt.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://co.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gi.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qr.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cz.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wc.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dp.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fy.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bd.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://mo.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://el.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rb.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://fv.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ju.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fw.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mm.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hu.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ue.szxytkj.cn

[H04] 自定义异常类型
来源：http://tu.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://vu.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ik.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://rz.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ib.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://dz.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cg.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://xp.szsharing.cn

C#:   class MyException : Exception {}
来源：http://jm.muxihuayi.cn

[H05] 捕获特定类型
来源：http://tu.gzmigu.cn

Py:   except ValueError as e:
来源：http://ap.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qy.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://oq.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://el.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://mn.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://au.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://hu.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ms.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://bt.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://xn.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nt.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://or.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://id.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bw.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ct.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://yv.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://mb.newstarts.cn

[H07] 断言
来源：http://mi.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://dx.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://fo.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://xj.nszjky.cn

TS:   console.assert(x > 0);
来源：http://vp.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://my.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zj.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kh.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://nf.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://ad.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ll.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hg.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://jd.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oh.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bk.bookmarksfly.cn

Go:   err.Error()
来源：http://dt.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://zf.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://mp.521024.cn

[H09] 带错误码的异常
来源：http://qo.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uy.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cd.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lc.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://su.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://la.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pe.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hx.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zm.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://qs.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xj.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pw.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jo.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qc.hnjuh.cn

Go:   defer f.Close()
来源：http://xa.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rc.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dj.huixinmuqiang.cn

================================================================================
来源：http://pw.wgjwhj.cn

I. 正则表达式
来源：http://tv.muxihuayi.cn

================================================================================
来源：http://xw.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://mc.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://px.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oe.nszjky.cn

JS:   /\d+/.test(s)
来源：http://qm.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://vk.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ld.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wz.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ko.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ve.szxytkj.cn

[I02] 提取所有匹配
来源：http://uv.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://aq.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tq.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xr.521024.cn

TS:   s.match(/\d+/g)
来源：http://eu.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ey.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://yi.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lz.bjjhwx.cn

[I03] 提取捕获分组
来源：http://uo.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zi.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ga.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uw.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sy.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://av.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dq.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ng.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nw.panjiajie.cn

[I04] 正则替换
来源：http://lx.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wi.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bh.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rz.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bt.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tf.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qx.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ar.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cb.asd995.cn

[I05] 按正则拆分
来源：http://lv.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uy.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rm.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://uw.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kt.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://ms.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vm.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ep.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qd.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://al.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yd.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dr.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bo.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://he.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bm.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hr.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fj.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zn.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://qr.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ic.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hv.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qd.hahajie.cn

TS:   /error/gim
来源：http://kl.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vf.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ep.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ta.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oz.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://uo.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zk.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://be.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bi.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zb.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ba.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hq.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ie.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ev.hnjuh.cn

================================================================================
来源：http://ky.panjiajie.cn

J. 日期与时间
来源：http://qc.szxytkj.cn

================================================================================
来源：http://oh.panjiajie.cn

[J01] 获取当前时间
来源：http://li.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pg.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kb.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://cj.521024.cn

TS:   new Date();  Date.now()
来源：http://wr.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jb.szsharing.cn

Go:   time.Now()
来源：http://un.hnjuh.cn

Ruby: Time.now
来源：http://ik.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ti.nszjky.cn

[J02] 格式化输出
来源：http://xd.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lf.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xf.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rs.nicolike.cn

TS:   d.toISOString()
来源：http://tw.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xl.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qj.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qp.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bc.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://we.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yp.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dj.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://hq.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://oa.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gz.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jd.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://io.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fj.hahajie.cn

[J04] 时间戳与日期互转
来源：http://wr.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eu.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://or.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fw.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ow.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ow.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cl.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kb.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yh.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://ta.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://vr.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uc.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sd.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://so.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://in.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mz.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://tk.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ej.muxihuayi.cn

[J06] 计算两时间之差
来源：http://tu.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://up.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://xu.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wk.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jw.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ua.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://cj.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://sb.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://cv.9csxet.cn

[J07] 比较两个日期
来源：http://rr.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://ht.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mv.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ra.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nt.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tn.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hd.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://em.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://lb.colortex.cn

[J08] 提取年月日与星期
来源：http://lw.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sv.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jo.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mn.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gz.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hf.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bl.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jx.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hr.9csxet.cn

[J09] 时区处理
来源：http://hi.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zc.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://go.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vd.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wg.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mp.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://og.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fs.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dz.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ug.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mi.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pv.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://em.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ob.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gl.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dp.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tl.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lh.bookmarksfly.cn

================================================================================
来源：http://ck.huanxung.cn

K. JSON 与序列化
来源：http://me.yuexingan06.cn

================================================================================
来源：http://yk.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://bz.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lc.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kf.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://qm.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://ky.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ri.nszjky.cn

Go:   json.Marshal(obj)
来源：http://sd.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://it.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eq.asd995.cn

[K02] JSON 字符串转对象
来源：http://ki.panjiajie.cn

Py:   json.loads(s)
来源：http://bt.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yw.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://ne.9csxet.cn

TS:   JSON.parse(s)
来源：http://dz.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ol.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://kc.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://ap.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ct.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://zr.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://al.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xa.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ih.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zb.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tt.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://la.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qm.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tj.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://tq.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yq.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cv.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kg.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://of.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mv.asd995.cn


<!-- 参考信息 -->