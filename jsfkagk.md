代发 wailian999

JS:   super.greet();
来源：http://ll.muxihuayi.cn

TS:   super.greet();
来源：http://cr.wgjwhj.cn

Java: super.greet();
来源：http://ro.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ye.muxihuayi.cn

Ruby: super
来源：http://ur.shxzukj.cn

C#:   base.Greet();
来源：http://pr.asd995.cn

[G08] 静态方法与属性
来源：http://nm.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yc.hahajie.cn

PHP:  public static function f() {}
来源：http://um.lnxyls.cn

JS:   static f() {}
来源：http://md.shtwfgs.cn

TS:   static f(): void {}
来源：http://xj.newstarts.cn

Java: static void f() {}
来源：http://be.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yd.szsharing.cn

Ruby: def self.f; end
来源：http://zi.huanxung.cn

C#:   public static void F() {}
来源：http://kd.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://oa.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://do.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oo.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jb.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://gs.nicolike.cn

Java: interface Shape { double area(); }
来源：http://uh.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://gg.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hy.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://cx.shxzukj.cn

[G10] 访问控制
来源：http://ra.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://gw.gzmigu.cn

PHP:  public / protected / private
来源：http://jr.newstarts.cn

JS:   #private 字段；其余公开
来源：http://yy.huixiangedu.cn

TS:   public / protected / private
来源：http://da.521024.cn

Java: public / protected / private / 默认包级
来源：http://ni.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wg.asd995.cn

Ruby: public / protected / private
来源：http://uy.gzmigu.cn

C#:   public / protected / private / internal
来源：http://wn.jianghongdianzi.cn

[G11] getter / setter
来源：http://so.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://bu.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gl.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://vn.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://jf.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://xs.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://th.9csxet.cn

Ruby: attr_accessor :name
来源：http://ox.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://qj.chemitech.net.cn

[G12] 对象转字符串
来源：http://ce.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://dn.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oc.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://de.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://gv.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ju.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tg.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://st.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://if.lnxyls.cn

[G13] 判断对象类型
来源：http://af.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://lp.panjiajie.cn

PHP:  $u instanceof User
来源：http://iv.wgjwhj.cn

JS:   u instanceof User
来源：http://cw.szsharing.cn

TS:   u instanceof User
来源：http://sx.chemitech.net.cn

Java: u instanceof User
来源：http://ln.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eh.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://vt.shtwfgs.cn

C#:   u is User
来源：http://xx.colortex.cn

[G14] 数据类 / record
来源：http://ca.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vm.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://sb.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ho.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://bk.huanxung.cn

Java: record User(String name, int age) {}
来源：http://jp.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://zk.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wh.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://yx.colortex.cn

[G15] 枚举
来源：http://db.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rq.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sn.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hj.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lf.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://aw.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xx.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://mb.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://il.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://wf.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xf.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://gf.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://sg.nszjky.cn

TS:   Object.entries(obj)
来源：http://eg.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ve.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://go.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://dg.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://pv.yuntaijiaju.cn

================================================================================
来源：http://uu.9csxet.cn

H. 异常与错误处理
来源：http://bl.panjiajie.cn

================================================================================
来源：http://ma.bjjhwx.cn

[H01] try / catch 基础
来源：http://xz.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ap.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hy.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ps.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ea.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pt.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fx.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hx.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ip.hahajie.cn

[H02] finally / ensure 收尾
来源：http://es.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vw.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xs.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mf.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ud.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ax.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lf.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lr.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zt.szsharing.cn

[H03] 主动抛出异常
来源：http://vx.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://el.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pk.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://pz.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ms.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rt.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yu.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wf.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jo.chemitech.net.cn

[H04] 自定义异常类型
来源：http://oj.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://qw.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ib.nicolike.cn

JS:   class MyError extends Error {}
来源：http://kx.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://is.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://nh.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sl.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://we.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://cn.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://sg.panjiajie.cn

Py:   except ValueError as e:
来源：http://de.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tz.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://uq.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://hg.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://qc.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nu.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://jn.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ef.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://eo.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://ux.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nl.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rl.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xk.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wx.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ki.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://sc.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://ci.bookmarksfly.cn

[H07] 断言
来源：http://lu.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://yw.panjiajie.cn

PHP:  assert($x > 0);
来源：http://xx.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://bj.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://vv.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://oz.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uc.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zs.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://xe.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://zf.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://jt.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fp.gzmigu.cn

JS:   e.message;  e.stack
来源：http://tg.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ol.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qh.newstarts.cn

Go:   err.Error()
来源：http://ts.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://he.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://ei.haigaiapp.cn

[H09] 带错误码的异常
来源：http://jv.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fc.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://om.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ow.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://df.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nu.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zu.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mq.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hj.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://vt.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ci.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ho.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ga.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xt.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cx.asd995.cn

Go:   defer f.Close()
来源：http://lc.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tg.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ge.nicolike.cn

================================================================================
来源：http://bo.yuntaijiaju.cn

I. 正则表达式
来源：http://tt.asd995.cn

================================================================================
来源：http://my.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://gg.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zg.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eb.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://bn.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://vx.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qt.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://im.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://zn.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uo.shtwfgs.cn

[I02] 提取所有匹配
来源：http://xh.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://fp.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lo.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vp.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://hv.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nh.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://kc.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tp.chemitech.net.cn

[I03] 提取捕获分组
来源：http://bq.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ue.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nh.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bc.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://he.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vj.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jg.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nw.yuexingan06.cn

[I04] 正则替换
来源：http://ne.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wm.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://on.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qv.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ti.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xj.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cn.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sh.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ak.shtwfgs.cn

[I05] 按正则拆分
来源：http://hq.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jk.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zy.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://ba.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ow.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://us.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xy.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wz.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mj.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dt.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ch.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lg.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://if.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://da.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ms.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lf.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jb.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jx.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://cg.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kj.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://np.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ek.shxzskj.cn

TS:   /error/gim
来源：http://si.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nd.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xg.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://wc.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wu.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://xe.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xp.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hg.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zr.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pt.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ri.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xi.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dk.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ne.hnjuh.cn

================================================================================
来源：http://ju.nicolike.cn

J. 日期与时间
来源：http://hw.colortex.cn

================================================================================
来源：http://rl.shxzskj.cn

[J01] 获取当前时间
来源：http://wg.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zi.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://if.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://cw.huanxung.cn

TS:   new Date();  Date.now()
来源：http://ud.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yy.nicolike.cn

Go:   time.Now()
来源：http://vv.bookmarksfly.cn

Ruby: Time.now
来源：http://qu.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fn.haigaiapp.cn

[J02] 格式化输出
来源：http://hh.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://et.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kv.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jp.szxytkj.cn

TS:   d.toISOString()
来源：http://aq.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tc.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oi.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vz.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ul.9csxet.cn

[J03] 字符串解析为日期
来源：http://pg.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dv.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dt.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://ua.521024.cn

TS:   new Date("2024-01-02")
来源：http://ew.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kc.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dy.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://ca.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gc.hahajie.cn

[J04] 时间戳与日期互转
来源：http://gw.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gd.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qz.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qo.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fq.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bx.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gi.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yr.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tv.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://lw.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://kv.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wy.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wz.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wu.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://yd.nicolike.cn


<!-- 参考信息 -->