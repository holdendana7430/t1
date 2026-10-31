代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ea.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://de.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://gd.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://wo.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://jp.shxzskj.cn

PHP:  $u instanceof User
来源：http://to.hnjuh.cn

JS:   u instanceof User
来源：http://fu.muxihuayi.cn

TS:   u instanceof User
来源：http://pv.newstarts.cn

Java: u instanceof User
来源：http://kg.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pz.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://fx.wgjwhj.cn

C#:   u is User
来源：http://cc.wgjwhj.cn

[G14] 数据类 / record
来源：http://jy.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lt.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://oa.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ad.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://kn.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://hi.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://vc.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://th.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://mw.szxytkj.cn

[G15] 枚举
来源：http://wg.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ug.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ev.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zf.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zy.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://nn.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iw.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://am.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ir.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://gm.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uh.colortex.cn

PHP:  get_object_vars($obj);
来源：http://xt.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://nj.nszjky.cn

TS:   Object.entries(obj)
来源：http://kq.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://by.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dr.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ck.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://wy.shxzskj.cn

================================================================================
来源：http://ay.newstarts.cn

H. 异常与错误处理
来源：http://id.chemitech.net.cn

================================================================================
来源：http://wg.lnxyls.cn

[H01] try / catch 基础
来源：http://to.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zc.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ze.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pe.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://do.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yx.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qv.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uz.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gf.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://bd.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wr.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mx.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://um.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pu.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kq.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sf.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://an.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dy.lnxyls.cn

[H03] 主动抛出异常
来源：http://iw.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://ak.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://du.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://th.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ra.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dr.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://am.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vp.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ia.shxzskj.cn

[H04] 自定义异常类型
来源：http://jb.asd995.cn

Py:   class MyError(Exception): pass
来源：http://si.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tc.asd995.cn

JS:   class MyError extends Error {}
来源：http://dd.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://ld.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://cw.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nf.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://rv.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://es.lnxyls.cn

[H05] 捕获特定类型
来源：http://gx.lnxyls.cn

Py:   except ValueError as e:
来源：http://zv.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oe.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://fp.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://mf.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://md.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eo.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://aa.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oa.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://rp.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://tb.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mj.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pm.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zr.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ha.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ow.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://ia.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://lw.shxzskj.cn

[H07] 断言
来源：http://rz.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://fe.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://sl.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://it.szsharing.cn

TS:   console.assert(x > 0);
来源：http://ge.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://eb.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cx.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ww.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ye.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://om.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://ai.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gv.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://mj.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vq.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hp.yuexingan06.cn

Go:   err.Error()
来源：http://qm.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://mk.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://xr.nicolike.cn

[H09] 带错误码的异常
来源：http://dd.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ry.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fp.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://io.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vn.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uj.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://up.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://im.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zt.shxzskj.cn

[H10] 资源自动释放
来源：http://yc.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://da.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nu.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fe.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ss.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://rg.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gr.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wo.colortex.cn

================================================================================
来源：http://zc.9csxet.cn

I. 正则表达式
来源：http://kf.szsharing.cn

================================================================================
来源：http://jt.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://vq.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jz.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ts.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://xl.newstarts.cn

TS:   /\d+/.test(s)
来源：http://zp.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lw.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bl.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://jo.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cn.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ip.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://sr.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tk.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rv.colortex.cn

TS:   s.match(/\d+/g)
来源：http://wa.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://np.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wm.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://hv.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rt.yuexingan06.cn

[I03] 提取捕获分组
来源：http://kw.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rg.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lx.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pe.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dh.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wi.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bb.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xu.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ny.9csxet.cn

[I04] 正则替换
来源：http://qc.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rw.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cq.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gn.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://os.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uc.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rb.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mu.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wb.lnxyls.cn

[I05] 按正则拆分
来源：http://mj.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vd.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://si.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://qp.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://pk.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://jh.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jc.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://td.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ak.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ip.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zb.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gu.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nk.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zo.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://la.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lc.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jb.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ll.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://fp.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://up.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gy.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ai.asd995.cn

TS:   /error/gim
来源：http://tt.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nj.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vz.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://nj.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uz.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://kw.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ra.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tx.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eq.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xw.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mh.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://it.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ck.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dk.nicolike.cn

================================================================================
来源：http://ao.9csxet.cn

J. 日期与时间
来源：http://oy.muxihuayi.cn

================================================================================
来源：http://ct.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://ai.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ha.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xu.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://rz.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ro.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sx.shxzukj.cn

Go:   time.Now()
来源：http://tg.jianghongdianzi.cn

Ruby: Time.now
来源：http://vv.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ak.jctech888.com.cn

[J02] 格式化输出
来源：http://nw.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fu.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ld.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cd.asd995.cn

TS:   d.toISOString()
来源：http://gn.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yg.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vs.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pb.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tl.shxzskj.cn

[J03] 字符串解析为日期
来源：http://zq.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cn.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mf.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://jz.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://rw.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ov.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wb.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://jz.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://li.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://cu.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rr.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bn.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cp.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dm.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vy.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ci.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rm.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ud.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ap.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://db.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ui.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://is.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://cr.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xt.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://mc.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ne.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://fa.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://vf.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://em.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mx.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://re.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pz.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://tx.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://vy.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://vm.shxzukj.cn

[J07] 比较两个日期
来源：http://ej.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://op.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gq.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vn.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sx.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kl.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qi.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ha.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://lg.gzmigu.cn

[J08] 提取年月日与星期
来源：http://hh.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ru.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ir.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tc.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dq.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://em.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rg.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://py.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://um.jctech888.com.cn

[J09] 时区处理
来源：http://ga.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nl.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fp.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pz.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://je.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zc.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sp.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pl.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lg.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://vo.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kn.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zc.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xi.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oi.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xb.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dj.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pr.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zx.gzmigu.cn


<!-- 参考信息 -->