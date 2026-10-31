代发 wailian999

TS:   constructor(public name: string) {}
来源：http://da.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://te.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ac.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ng.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://hx.jctech888.com.cn

[G03] 实例属性
来源：http://zs.huanxung.cn

Py:   self.name = "x"
来源：http://qo.shxzukj.cn

PHP:  public string $name = "x";
来源：http://yn.jctech888.com.cn

JS:   this.name = "x";
来源：http://lj.shxzukj.cn

TS:   name: string = "x";
来源：http://li.yuexingan06.cn

Java: private String name;
来源：http://xl.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rq.chemitech.net.cn

Ruby: @name = "x"
来源：http://av.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://tb.yuntaijiaju.cn

[G04] 定义方法
来源：http://ox.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://vf.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ux.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://ru.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://qu.shtwfgs.cn

Java: String greet() { return name; }
来源：http://xn.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ki.newstarts.cn

Ruby: def greet; @name; end
来源：http://tu.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://bj.yuntaijiaju.cn

[G05] 继承
来源：http://lr.gzmigu.cn

Py:   class Admin(User): pass
来源：http://ee.hahajie.cn

PHP:  class Admin extends User {}
来源：http://fc.asd995.cn

JS:   class Admin extends User {}
来源：http://fd.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://kr.nicolike.cn

Java: class Admin extends User {}
来源：http://bt.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xs.asd995.cn

Ruby: class Admin < User; end
来源：http://vy.haigaiapp.cn

C#:   class Admin : User {}
来源：http://ec.newstarts.cn

[G06] 重写方法
来源：http://xk.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ry.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fk.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://oj.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://rt.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://nn.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uu.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://sj.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://fy.muxihuayi.cn

[G07] 调用父类方法
来源：http://sw.jctech888.com.cn

Py:   super().greet()
来源：http://ba.szxytkj.cn

PHP:  parent::greet();
来源：http://lo.bookmarksfly.cn

JS:   super.greet();
来源：http://ve.huanxung.cn

TS:   super.greet();
来源：http://td.huanxung.cn

Java: super.greet();
来源：http://lq.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ig.lnxyls.cn

Ruby: super
来源：http://qj.colortex.cn

C#:   base.Greet();
来源：http://oo.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ur.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sr.521024.cn

PHP:  public static function f() {}
来源：http://ml.muxihuayi.cn

JS:   static f() {}
来源：http://fg.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://qh.hnjuh.cn

Java: static void f() {}
来源：http://hm.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kg.9csxet.cn

Ruby: def self.f; end
来源：http://gd.colortex.cn

C#:   public static void F() {}
来源：http://sc.hahajie.cn

[G09] 接口 / 抽象类
来源：http://cv.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://lo.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xw.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eq.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://nq.asd995.cn

Java: interface Shape { double area(); }
来源：http://gh.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://jg.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dq.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://yd.yuntaijiaju.cn

[G10] 访问控制
来源：http://kv.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://jb.muxihuayi.cn

PHP:  public / protected / private
来源：http://wc.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://yb.jianghongdianzi.cn

TS:   public / protected / private
来源：http://oz.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://vf.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vh.nicolike.cn

Ruby: public / protected / private
来源：http://qv.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://qb.521024.cn

[G11] getter / setter
来源：http://ys.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://hu.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ci.521024.cn

JS:   get name() { return this._name; }
来源：http://kt.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://qy.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://vn.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bs.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ej.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://fo.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://rw.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://nv.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ib.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://sh.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://zc.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://fu.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nk.szsharing.cn

Ruby: def to_s; @name; end
来源：http://xg.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://qj.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://nr.lnxyls.cn

Py:   isinstance(u, User)
来源：http://yg.szxytkj.cn

PHP:  $u instanceof User
来源：http://tx.lnxyls.cn

JS:   u instanceof User
来源：http://at.shtwfgs.cn

TS:   u instanceof User
来源：http://sk.hnjuh.cn

Java: u instanceof User
来源：http://zg.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xy.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://tc.szxytkj.cn

C#:   u is User
来源：http://us.bookmarksfly.cn

[G14] 数据类 / record
来源：http://tp.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fu.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://at.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nk.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://vq.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://fv.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://ps.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hk.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://sb.yuntaijiaju.cn

[G15] 枚举
来源：http://by.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tm.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bt.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ke.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jf.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://gm.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xg.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://tr.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pb.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://ko.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hu.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://xz.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ph.panjiajie.cn

TS:   Object.entries(obj)
来源：http://bx.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jb.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://es.9csxet.cn

Ruby: obj.instance_variables
来源：http://cx.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ih.panjiajie.cn

================================================================================
来源：http://fu.wgjwhj.cn

H. 异常与错误处理
来源：http://lt.yuntaijiaju.cn

================================================================================
来源：http://qg.hnjuh.cn

[H01] try / catch 基础
来源：http://hl.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ns.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://au.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ah.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://as.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jd.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gk.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ee.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bi.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://cu.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ct.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zg.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qj.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://as.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xz.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zd.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mc.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zl.panjiajie.cn

[H03] 主动抛出异常
来源：http://qr.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://ul.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uw.521024.cn

JS:   throw new Error("错误信息");
来源：http://dz.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://gn.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qb.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xo.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bf.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nw.lnxyls.cn

[H04] 自定义异常类型
来源：http://tr.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://pt.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pb.huanxung.cn

JS:   class MyError extends Error {}
来源：http://pv.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://bl.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://nh.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rd.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://fl.nicolike.cn

C#:   class MyException : Exception {}
来源：http://fj.shxzukj.cn

[H05] 捕获特定类型
来源：http://wy.colortex.cn

Py:   except ValueError as e:
来源：http://ec.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://os.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://si.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://yk.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wg.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sx.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://it.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mg.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://uy.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://zb.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wd.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://af.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rk.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ze.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nj.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ef.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://jf.yuntaijiaju.cn

[H07] 断言
来源：http://tk.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://ic.shxzukj.cn

PHP:  assert($x > 0);
来源：http://he.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://st.nszjky.cn

TS:   console.assert(x > 0);
来源：http://mh.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://iq.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://al.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wg.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://up.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://ni.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://bb.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ty.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://lb.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wz.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cm.jianghongdianzi.cn

Go:   err.Error()
来源：http://nr.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ny.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://as.panjiajie.cn

[H09] 带错误码的异常
来源：http://ky.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kg.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kk.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://di.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lf.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zn.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qh.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wj.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pk.huixiangedu.cn

[H10] 资源自动释放
来源：http://il.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lm.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ms.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ar.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ks.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ah.panjiajie.cn

Go:   defer f.Close()
来源：http://wa.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iu.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yu.panjiajie.cn

================================================================================
来源：http://fw.gzmigu.cn

I. 正则表达式
来源：http://wr.asd995.cn

================================================================================
来源：http://ew.521024.cn

[I01] 判断是否匹配
来源：http://of.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gq.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ls.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://kj.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://gi.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://py.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rh.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://mo.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ie.panjiajie.cn

[I02] 提取所有匹配
来源：http://kx.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://pi.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jq.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lg.colortex.cn

TS:   s.match(/\d+/g)
来源：http://en.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uv.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xa.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://dd.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ck.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://um.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mt.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wg.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gn.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pr.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vi.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://py.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ot.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tx.szsharing.cn

[I04] 正则替换
来源：http://dg.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kk.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ls.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jc.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ci.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wj.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wj.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dp.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oe.panjiajie.cn

[I05] 按正则拆分
来源：http://ii.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yb.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jm.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://ht.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mx.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://yt.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ju.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://se.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rr.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ln.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://me.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jo.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://og.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pf.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qz.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mv.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wc.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://im.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://do.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pn.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kg.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://td.521024.cn

TS:   /error/gim
来源：http://yk.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wq.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://za.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://uq.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://af.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://wr.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bl.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cn.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iz.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bk.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wo.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ov.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://au.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mf.wgjwhj.cn

================================================================================
来源：http://fv.szxytkj.cn


<!-- 参考信息 -->