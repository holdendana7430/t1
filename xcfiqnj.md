代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://xf.nicolike.cn

Ruby: def to_s; @name; end
来源：http://ft.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://md.nszjky.cn

[G13] 判断对象类型
来源：http://dr.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://qk.shtwfgs.cn

PHP:  $u instanceof User
来源：http://hv.bjjhwx.cn

JS:   u instanceof User
来源：http://zv.lnxyls.cn

TS:   u instanceof User
来源：http://ou.shxzukj.cn

Java: u instanceof User
来源：http://ci.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fx.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://qz.panjiajie.cn

C#:   u is User
来源：http://xl.szxytkj.cn

[G14] 数据类 / record
来源：http://jw.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ja.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://oj.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hs.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://zi.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://ms.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://ts.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rv.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://xg.bjjhwx.cn

[G15] 枚举
来源：http://vq.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dl.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dg.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wc.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wz.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://my.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ia.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://en.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fr.521024.cn

[G16] 对象转数组 / 字典
来源：http://xg.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wz.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://is.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://zl.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://cf.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ck.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wq.shxzskj.cn

Ruby: obj.instance_variables
来源：http://qo.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://sy.hnjuh.cn

================================================================================
来源：http://rv.muxihuayi.cn

H. 异常与错误处理
来源：http://jv.9csxet.cn

================================================================================
来源：http://wo.9csxet.cn

[H01] try / catch 基础
来源：http://bj.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://of.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tp.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dw.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cj.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hi.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jb.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hy.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ny.huanxung.cn

[H02] finally / ensure 收尾
来源：http://wz.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ef.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ma.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bf.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wh.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://po.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://if.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://id.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nf.panjiajie.cn

[H03] 主动抛出异常
来源：http://em.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://vt.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://as.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://or.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://yc.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gk.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pt.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gx.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qk.newstarts.cn

[H04] 自定义异常类型
来源：http://ku.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://kh.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fd.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://qq.szsharing.cn

TS:   class MyError extends Error {}
来源：http://yy.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://hr.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vq.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://ne.asd995.cn

C#:   class MyException : Exception {}
来源：http://lg.newstarts.cn

[H05] 捕获特定类型
来源：http://nz.521024.cn

Py:   except ValueError as e:
来源：http://an.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wl.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://aj.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://rb.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://nm.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gp.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hq.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gw.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ke.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://ex.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jp.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://as.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sq.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hw.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qe.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://dv.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://wj.szsharing.cn

[H07] 断言
来源：http://fm.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://uf.newstarts.cn

PHP:  assert($x > 0);
来源：http://zh.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://yl.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://cn.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://bz.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nq.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cw.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://vs.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://bc.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://vc.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ro.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ow.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ue.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ss.yuntaijiaju.cn

Go:   err.Error()
来源：http://eb.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://xq.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://un.wgjwhj.cn

[H09] 带错误码的异常
来源：http://en.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fx.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ox.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ft.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xa.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ll.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yf.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gq.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jb.newstarts.cn

[H10] 资源自动释放
来源：http://bv.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kf.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tm.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gv.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://by.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jc.szsharing.cn

Go:   defer f.Close()
来源：http://xa.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qx.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zh.lnxyls.cn

================================================================================
来源：http://nt.wgjwhj.cn

I. 正则表达式
来源：http://ke.jctech888.com.cn

================================================================================
来源：http://ms.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://mm.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ib.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bx.huanxung.cn

JS:   /\d+/.test(s)
来源：http://te.huanxung.cn

TS:   /\d+/.test(s)
来源：http://uq.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ko.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vw.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://pd.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fu.shxzskj.cn

[I02] 提取所有匹配
来源：http://ri.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://de.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zi.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bv.521024.cn

TS:   s.match(/\d+/g)
来源：http://op.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hl.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vg.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://uu.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oj.newstarts.cn

[I03] 提取捕获分组
来源：http://cw.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gw.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oy.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://za.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hn.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zr.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jr.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qx.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dk.hahajie.cn

[I04] 正则替换
来源：http://kt.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ee.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://id.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wz.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pv.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xo.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rq.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jp.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://so.chemitech.net.cn

[I05] 按正则拆分
来源：http://wc.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uh.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eq.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://kx.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ta.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://wi.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ob.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jw.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://re.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zj.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xj.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qt.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uv.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fw.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jm.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zo.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kw.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mz.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://kt.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xy.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tb.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mp.huixinmuqiang.cn

TS:   /error/gim
来源：http://zz.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ou.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ob.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://hg.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ny.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://yk.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qh.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://on.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pl.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mg.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xw.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qz.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jx.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vw.yuntaijiaju.cn

================================================================================
来源：http://hl.bjjhwx.cn

J. 日期与时间
来源：http://vr.yuexingan06.cn

================================================================================
来源：http://ae.panjiajie.cn

[J01] 获取当前时间
来源：http://cx.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://co.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gd.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://un.asd995.cn

TS:   new Date();  Date.now()
来源：http://xo.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tz.bjjhwx.cn

Go:   time.Now()
来源：http://st.yuexingan06.cn

Ruby: Time.now
来源：http://qu.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mc.newstarts.cn

[J02] 格式化输出
来源：http://ra.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mw.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pe.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rj.szsharing.cn

TS:   d.toISOString()
来源：http://ps.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zj.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cp.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://du.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kb.gzmigu.cn

[J03] 字符串解析为日期
来源：http://bt.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oz.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ed.asd995.cn

JS:   new Date("2024-01-02")
来源：http://vp.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://dp.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://db.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uv.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://it.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sj.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ra.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bk.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qe.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kd.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yz.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jy.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tw.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fh.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xa.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://nh.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://qn.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jv.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mt.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tq.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://yk.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://le.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://vy.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jg.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://lb.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://xd.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://op.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wx.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tc.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bf.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://nb.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://pm.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://va.nszjky.cn

[J07] 比较两个日期
来源：http://nj.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://or.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gn.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qy.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hy.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xe.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bl.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qh.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://jw.9csxet.cn

[J08] 提取年月日与星期
来源：http://ez.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cv.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fn.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jr.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mz.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://as.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vf.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dv.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vr.lnxyls.cn

[J09] 时区处理
来源：http://bf.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kp.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ir.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tz.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lg.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://es.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rw.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://my.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tl.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://gr.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mk.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://um.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hf.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ug.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bp.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pj.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oa.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ew.9csxet.cn


<!-- 参考信息 -->