代发 wailian999

JS:   this.name = "x";
来源：http://lu.newstarts.cn

TS:   name: string = "x";
来源：http://dc.asd995.cn

Java: private String name;
来源：http://va.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wl.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://et.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://gy.huanxung.cn

[G04] 定义方法
来源：http://vk.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://nu.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mr.9csxet.cn

JS:   greet() { return this.name; }
来源：http://zg.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://bz.521024.cn

Java: String greet() { return name; }
来源：http://io.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hl.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://zj.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://dx.huanxung.cn

[G05] 继承
来源：http://pl.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://yj.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://ij.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://hc.521024.cn

TS:   class Admin extends User {}
来源：http://al.huixiangedu.cn

Java: class Admin extends User {}
来源：http://lw.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lk.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://ru.colortex.cn

C#:   class Admin : User {}
来源：http://oz.yuexingan06.cn

[G06] 重写方法
来源：http://dv.colortex.cn

Py:   def greet(self): return "admin"
来源：http://ru.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qa.asd995.cn

JS:   greet() { return "admin"; }
来源：http://wi.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://tz.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://tn.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ky.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://gd.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://it.newstarts.cn

[G07] 调用父类方法
来源：http://py.yuntaijiaju.cn

Py:   super().greet()
来源：http://nu.gzmigu.cn

PHP:  parent::greet();
来源：http://xg.muxihuayi.cn

JS:   super.greet();
来源：http://bu.bookmarksfly.cn

TS:   super.greet();
来源：http://mp.huanxung.cn

Java: super.greet();
来源：http://eq.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kb.521024.cn

Ruby: super
来源：http://ck.shxzukj.cn

C#:   base.Greet();
来源：http://cl.gzmigu.cn

[G08] 静态方法与属性
来源：http://yh.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pm.huanxung.cn

PHP:  public static function f() {}
来源：http://ms.chemitech.net.cn

JS:   static f() {}
来源：http://br.yuexingan06.cn

TS:   static f(): void {}
来源：http://bz.jctech888.com.cn

Java: static void f() {}
来源：http://tz.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vd.nszjky.cn

Ruby: def self.f; end
来源：http://ne.colortex.cn

C#:   public static void F() {}
来源：http://kr.nszjky.cn

[G09] 接口 / 抽象类
来源：http://up.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://rk.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://it.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yg.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://tl.colortex.cn

Java: interface Shape { double area(); }
来源：http://wa.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://lp.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gn.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://nw.bjjhwx.cn

[G10] 访问控制
来源：http://mz.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://md.haigaiapp.cn

PHP:  public / protected / private
来源：http://rx.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://qx.shtwfgs.cn

TS:   public / protected / private
来源：http://lf.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://ub.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yy.9csxet.cn

Ruby: public / protected / private
来源：http://cu.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://qf.chemitech.net.cn

[G11] getter / setter
来源：http://br.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://bv.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dc.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://ua.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://ny.huanxung.cn

Java: public String getName() { return name; }
来源：http://al.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iy.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://vw.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://fu.szsharing.cn

[G12] 对象转字符串
来源：http://vf.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://uh.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sy.huanxung.cn

JS:   toString() { return this.name; }
来源：http://xu.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://dt.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://yz.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zo.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://zu.521024.cn

C#:   public override string ToString() => Name;
来源：http://kg.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://we.szxytkj.cn

Py:   isinstance(u, User)
来源：http://lt.521024.cn

PHP:  $u instanceof User
来源：http://zs.shxzukj.cn

JS:   u instanceof User
来源：http://yf.newstarts.cn

TS:   u instanceof User
来源：http://uh.shtwfgs.cn

Java: u instanceof User
来源：http://qs.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ub.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://wx.hahajie.cn

C#:   u is User
来源：http://tz.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://ng.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ax.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://of.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qk.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://xk.huanxung.cn

Java: record User(String name, int age) {}
来源：http://ro.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://bs.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://af.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://ih.nszjky.cn

[G15] 枚举
来源：http://jb.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uk.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jv.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qn.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ub.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://pd.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tw.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ld.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mx.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://sl.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aj.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://xc.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://pp.asd995.cn

TS:   Object.entries(obj)
来源：http://vy.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dh.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://je.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://wz.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ps.asd995.cn

================================================================================
来源：http://pb.haigaiapp.cn

H. 异常与错误处理
来源：http://fo.jianghongdianzi.cn

================================================================================
来源：http://rp.yuexingan06.cn

[H01] try / catch 基础
来源：http://bv.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fh.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qr.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oe.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zu.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wr.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tq.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nt.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gc.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://tm.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uh.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ce.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ie.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ti.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ej.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cz.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hg.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ka.muxihuayi.cn

[H03] 主动抛出异常
来源：http://ma.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://kg.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://er.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://qh.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://gj.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://np.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fa.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bd.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://mb.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://xx.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fw.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://pt.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://fe.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mw.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://uq.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://jq.szxytkj.cn

[H05] 捕获特定类型
来源：http://jq.muxihuayi.cn

Py:   except ValueError as e:
来源：http://hd.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tj.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ak.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://om.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://aa.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ho.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://aa.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://at.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://cj.nszjky.cn

Py:   value = d.get("k") or default
来源：http://gx.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mc.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kp.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eu.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hg.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cp.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://vr.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://lf.haigaiapp.cn

[H07] 断言
来源：http://gn.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ec.shxzukj.cn

PHP:  assert($x > 0);
来源：http://vu.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://fj.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://wq.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://ye.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xk.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ay.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://yp.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://wo.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://jj.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dv.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://cc.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fo.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xh.yuntaijiaju.cn

Go:   err.Error()
来源：http://vg.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://jq.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://mi.nszjky.cn

[H09] 带错误码的异常
来源：http://kd.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rp.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wd.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dd.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kk.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ta.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ub.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yd.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zs.panjiajie.cn

[H10] 资源自动释放
来源：http://mk.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qq.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wa.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ly.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ff.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hw.panjiajie.cn

Go:   defer f.Close()
来源：http://mo.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bo.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nd.nicolike.cn

================================================================================
来源：http://ti.chemitech.net.cn

I. 正则表达式
来源：http://cb.jctech888.com.cn

================================================================================
来源：http://eo.521024.cn

[I01] 判断是否匹配
来源：http://zu.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nj.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ht.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://mh.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://on.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xq.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ci.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qe.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://xd.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://kb.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lr.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uk.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://hy.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kp.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bh.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://so.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ff.asd995.cn

[I03] 提取捕获分组
来源：http://ge.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wu.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wp.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qw.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bo.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uw.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ay.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wp.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ni.asd995.cn

[I04] 正则替换
来源：http://mm.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dv.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yo.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mr.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vn.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bd.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ec.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xg.huixiangedu.cn

[I05] 按正则拆分
来源：http://kq.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://um.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ha.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://zj.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://gz.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ui.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://np.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cv.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iu.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zm.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dr.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xm.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ex.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bp.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oo.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oq.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ak.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://pt.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ys.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yh.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wy.wgjwhj.cn

TS:   /error/gim
来源：http://md.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ql.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bl.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://hf.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vl.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://kq.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hc.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vh.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bi.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nz.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://po.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zw.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wq.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://th.nszjky.cn

================================================================================
来源：http://dc.yuntaijiaju.cn

J. 日期与时间
来源：http://ue.panjiajie.cn

================================================================================
来源：http://ks.nicolike.cn

[J01] 获取当前时间
来源：http://pa.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://as.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eq.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://yz.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://ci.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wf.huanxung.cn


<!-- 参考信息 -->