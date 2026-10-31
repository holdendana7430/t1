代发 wailian999

C#:   record User(string Name, int Age);
来源：http://tc.gzmigu.cn

[G15] 枚举
来源：http://xd.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mi.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://no.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ge.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cv.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://rm.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nu.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://ks.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://di.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://wh.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ru.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://kg.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://di.colortex.cn

TS:   Object.entries(obj)
来源：http://an.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pn.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fq.lnxyls.cn

Ruby: obj.instance_variables
来源：http://sp.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://ft.newstarts.cn

================================================================================
来源：http://op.chemitech.net.cn

H. 异常与错误处理
来源：http://zu.haigaiapp.cn

================================================================================
来源：http://jc.szxytkj.cn

[H01] try / catch 基础
来源：http://gu.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://av.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vq.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ds.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hx.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vq.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bf.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jy.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gc.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ei.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zv.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://io.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ix.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qt.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pc.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hv.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fi.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zs.521024.cn

[H03] 主动抛出异常
来源：http://se.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://yc.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mv.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://aw.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://wi.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hj.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rr.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bt.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xk.lnxyls.cn

[H04] 自定义异常类型
来源：http://zr.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://xj.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://da.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://pr.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://sg.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://qg.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pr.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://xp.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://fr.shxzukj.cn

[H05] 捕获特定类型
来源：http://ia.hnjuh.cn

Py:   except ValueError as e:
来源：http://de.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mi.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://qn.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://mt.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://lv.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cv.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://nu.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wr.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://pl.szsharing.cn

Py:   value = d.get("k") or default
来源：http://bb.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jp.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rb.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://en.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lt.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bb.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ov.521024.cn

C#:   obj?.A?.B ?? default
来源：http://hr.asd995.cn

[H07] 断言
来源：http://lo.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://wl.shxzskj.cn

PHP:  assert($x > 0);
来源：http://um.nszjky.cn

JS:   console.assert(x > 0);
来源：http://mu.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://ft.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://uw.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ir.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ij.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://oo.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://cg.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ub.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kn.panjiajie.cn

JS:   e.message;  e.stack
来源：http://vj.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vq.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xf.lnxyls.cn

Go:   err.Error()
来源：http://zi.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://sb.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://ng.newstarts.cn

[H09] 带错误码的异常
来源：http://vd.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ho.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fe.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sc.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uk.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://me.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://az.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bs.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vu.jctech888.com.cn

[H10] 资源自动释放
来源：http://ed.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oc.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pt.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kr.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nt.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xk.9csxet.cn

Go:   defer f.Close()
来源：http://gi.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xq.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jy.huixiangedu.cn

================================================================================
来源：http://lq.gzmigu.cn

I. 正则表达式
来源：http://bs.newstarts.cn

================================================================================
来源：http://ye.yuexingan06.cn

[I01] 判断是否匹配
来源：http://wm.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bb.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xk.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://vr.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ob.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://it.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ak.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ea.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fc.nszjky.cn

[I02] 提取所有匹配
来源：http://xg.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://gx.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://la.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ns.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://bh.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://du.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ml.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://tu.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bi.hnjuh.cn

[I03] 提取捕获分组
来源：http://rm.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kd.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mx.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vx.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kp.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xb.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fy.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ro.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://de.yuexingan06.cn

[I04] 正则替换
来源：http://ov.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zn.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zg.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vz.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fq.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pa.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uh.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nb.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nm.shxzskj.cn

[I05] 按正则拆分
来源：http://ii.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://le.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ec.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://yo.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://zs.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://bs.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wi.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mp.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://li.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kw.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ms.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lz.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://am.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ak.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lv.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vu.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ar.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://xn.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wr.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gs.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ex.shxzskj.cn

TS:   /error/gim
来源：http://hz.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fy.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fe.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://nr.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gh.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://cd.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sx.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vc.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ra.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ug.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vl.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sw.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sx.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dj.jianghongdianzi.cn

================================================================================
来源：http://az.nszjky.cn

J. 日期与时间
来源：http://gt.shtwfgs.cn

================================================================================
来源：http://cd.wgjwhj.cn

[J01] 获取当前时间
来源：http://dn.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ah.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xq.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://bd.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://fp.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ki.newstarts.cn

Go:   time.Now()
来源：http://xk.chemitech.net.cn

Ruby: Time.now
来源：http://si.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rr.yuntaijiaju.cn

[J02] 格式化输出
来源：http://jo.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aa.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://js.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oi.hnjuh.cn

TS:   d.toISOString()
来源：http://vm.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cp.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pt.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ta.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ay.szxytkj.cn

[J03] 字符串解析为日期
来源：http://gf.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tx.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fc.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://sq.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://zf.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ni.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dq.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://qe.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cz.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://wm.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ix.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://az.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oe.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sd.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vz.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vj.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nk.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gp.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://ul.colortex.cn

Py:   now + timedelta(days=7)
来源：http://th.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yu.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ax.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dv.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://sx.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kl.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://sh.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ha.hahajie.cn

[J06] 计算两时间之差
来源：http://dd.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://zf.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://xk.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ns.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yi.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vh.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://mb.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://nl.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://fq.shxzskj.cn

[J07] 比较两个日期
来源：http://up.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://aw.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pg.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lg.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iz.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://el.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://it.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://on.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://qo.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mw.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zg.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oc.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://js.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mq.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://do.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vg.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ke.muxihuayi.cn

[J09] 时区处理
来源：http://gp.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yb.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bl.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ma.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lo.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vn.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mb.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gv.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uk.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://jn.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://es.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ma.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nq.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bt.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qg.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zz.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nh.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ti.bjjhwx.cn

================================================================================
来源：http://ou.shxzukj.cn

K. JSON 与序列化
来源：http://ro.shxzukj.cn

================================================================================
来源：http://fz.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://wg.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ch.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rm.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://dw.521024.cn

TS:   JSON.stringify(obj)
来源：http://pr.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dy.nszjky.cn

Go:   json.Marshal(obj)
来源：http://zj.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ac.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cv.nicolike.cn

[K02] JSON 字符串转对象
来源：http://it.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://jy.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iv.szsharing.cn

JS:   JSON.parse(s)
来源：http://xs.hnjuh.cn

TS:   JSON.parse(s)
来源：http://fl.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ry.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fv.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://im.9csxet.cn


<!-- 参考信息 -->