代发 wailian999

[G14] 数据类 / record
来源：http://pi.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vs.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://jl.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pb.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://ty.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://dv.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://qy.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kz.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://qy.chemitech.net.cn

[G15] 枚举
来源：http://xq.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xf.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wo.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gp.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mu.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ur.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aj.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xh.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nq.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://xp.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nj.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://zq.hahajie.cn

JS:   Object.entries(obj)
来源：http://ev.lnxyls.cn

TS:   Object.entries(obj)
来源：http://uv.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://co.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zr.panjiajie.cn

Ruby: obj.instance_variables
来源：http://xy.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://fa.521024.cn

================================================================================
来源：http://ii.hahajie.cn

H. 异常与错误处理
来源：http://fo.asd995.cn

================================================================================
来源：http://qj.asd995.cn

[H01] try / catch 基础
来源：http://ak.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hh.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://va.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xr.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tx.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vm.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ei.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bq.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eh.huanxung.cn

[H02] finally / ensure 收尾
来源：http://yj.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jt.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bz.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://no.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gg.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rj.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tp.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nu.jctech888.com.cn

[H03] 主动抛出异常
来源：http://rs.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://sf.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jm.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://tc.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://go.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qs.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aa.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jr.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ot.panjiajie.cn

[H04] 自定义异常类型
来源：http://ga.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://bp.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qa.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://mx.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://hp.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://rp.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dz.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://cl.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://ku.asd995.cn

[H05] 捕获特定类型
来源：http://ln.bjjhwx.cn

Py:   except ValueError as e:
来源：http://wu.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qf.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://fi.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://yx.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://gq.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://im.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://xj.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://se.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://er.huanxung.cn

Py:   value = d.get("k") or default
来源：http://gu.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uh.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kx.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rv.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dq.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qm.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://qc.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://xr.shxzukj.cn

[H07] 断言
来源：http://xx.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://os.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://vs.szsharing.cn

JS:   console.assert(x > 0);
来源：http://ar.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ad.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://hd.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sk.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sy.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://nd.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://km.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://lo.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://er.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://lg.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dj.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://to.shxzukj.cn

Go:   err.Error()
来源：http://fz.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://jr.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://fd.jctech888.com.cn

[H09] 带错误码的异常
来源：http://cl.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kq.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xr.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bn.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pk.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zc.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wv.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ye.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ta.newstarts.cn

[H10] 资源自动释放
来源：http://kd.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jt.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eu.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gu.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://el.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ra.huanxung.cn

Go:   defer f.Close()
来源：http://gi.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://av.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ou.huixiangedu.cn

================================================================================
来源：http://pb.nszjky.cn

I. 正则表达式
来源：http://ow.panjiajie.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://qd.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iq.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ou.newstarts.cn

JS:   /\d+/.test(s)
来源：http://lk.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://yu.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ol.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sk.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://md.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ux.shxzskj.cn

[I02] 提取所有匹配
来源：http://nz.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://ru.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://it.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mq.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://kt.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nb.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vb.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://aa.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://we.hahajie.cn

[I03] 提取捕获分组
来源：http://rx.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ol.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xy.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aq.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ft.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qe.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tf.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kh.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sr.hnjuh.cn

[I04] 正则替换
来源：http://rz.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wb.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://th.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ch.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ia.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uc.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ln.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sw.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ta.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://nj.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eh.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sl.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://xh.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://br.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://yd.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fr.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rc.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xl.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://de.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zo.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bm.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ox.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kn.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kz.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sx.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cz.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fj.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://oz.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://si.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qe.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ln.nszjky.cn

TS:   /error/gim
来源：http://zc.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oe.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://td.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://bn.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zf.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://ip.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uc.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ae.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wn.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://su.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wn.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://an.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mi.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xf.bookmarksfly.cn

================================================================================
来源：http://wq.colortex.cn

J. 日期与时间
来源：http://nq.lnxyls.cn

================================================================================
来源：http://kt.hahajie.cn

[J01] 获取当前时间
来源：http://sw.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bu.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yz.szsharing.cn

JS:   new Date();  Date.now()
来源：http://fs.521024.cn

TS:   new Date();  Date.now()
来源：http://vc.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://me.lnxyls.cn

Go:   time.Now()
来源：http://ue.chemitech.net.cn

Ruby: Time.now
来源：http://bq.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cc.hnjuh.cn

[J02] 格式化输出
来源：http://ro.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pf.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ob.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ct.lnxyls.cn

TS:   d.toISOString()
来源：http://ml.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ko.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yd.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yh.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cr.shxzukj.cn

[J03] 字符串解析为日期
来源：http://wf.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mz.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ii.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ft.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://us.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xw.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wk.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://zv.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://se.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://aa.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ms.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ro.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jh.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sz.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pf.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kc.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uj.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rv.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://sp.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://yb.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://te.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wy.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://vh.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pl.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://uc.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://il.hnjuh.cn

[J06] 计算两时间之差
来源：http://vj.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://ki.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ue.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gf.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yx.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fm.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://bk.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://og.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://jt.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://nv.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://qe.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dx.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nl.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nj.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hq.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gj.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xe.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xs.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://yq.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jw.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tu.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ch.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jq.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ho.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xb.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yq.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://je.colortex.cn

[J09] 时区处理
来源：http://vw.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sj.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ku.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ud.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cu.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pi.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sl.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ox.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gk.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://vf.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zt.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pj.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wp.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qb.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lf.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wo.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qu.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eo.wgjwhj.cn

================================================================================
来源：http://lb.szsharing.cn

K. JSON 与序列化
来源：http://fv.panjiajie.cn

================================================================================
来源：http://jc.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ec.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://li.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cb.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://tg.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://hn.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zb.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://mt.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qs.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zv.521024.cn


<!-- 参考信息 -->