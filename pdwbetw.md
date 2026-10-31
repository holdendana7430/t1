代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xs.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vm.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://am.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iw.nicolike.cn

================================================================================
来源：http://cj.hnjuh.cn

G. 面向对象
来源：http://zp.bjjhwx.cn

================================================================================
来源：http://zl.szsharing.cn

[G01] 定义类
来源：http://hy.huixiangedu.cn

Py:   class User: pass
来源：http://vt.muxihuayi.cn

PHP:  class User {}
来源：http://xb.huixiangedu.cn

JS:   class User {}
来源：http://sk.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://sk.colortex.cn

Java: class User {}
来源：http://wu.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://oc.haigaiapp.cn

Ruby: class User; end
来源：http://ui.huixiangedu.cn

C#:   class User {}
来源：http://nr.nicolike.cn

[G02] 构造函数
来源：http://cv.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://rh.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ic.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://js.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://lj.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://nb.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://il.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ls.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://xc.shxzskj.cn

[G03] 实例属性
来源：http://ct.jctech888.com.cn

Py:   self.name = "x"
来源：http://az.asd995.cn

PHP:  public string $name = "x";
来源：http://ql.panjiajie.cn

JS:   this.name = "x";
来源：http://sm.hnjuh.cn

TS:   name: string = "x";
来源：http://ux.colortex.cn

Java: private String name;
来源：http://xo.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ci.gzmigu.cn

Ruby: @name = "x"
来源：http://ar.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ul.huixiangedu.cn

[G04] 定义方法
来源：http://ht.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://dx.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bn.asd995.cn

JS:   greet() { return this.name; }
来源：http://du.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://nq.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://qo.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xl.szsharing.cn

Ruby: def greet; @name; end
来源：http://ur.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://bn.shtwfgs.cn

[G05] 继承
来源：http://ob.asd995.cn

Py:   class Admin(User): pass
来源：http://kk.521024.cn

PHP:  class Admin extends User {}
来源：http://vb.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://tc.newstarts.cn

TS:   class Admin extends User {}
来源：http://ux.huanxung.cn

Java: class Admin extends User {}
来源：http://za.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uz.huanxung.cn

Ruby: class Admin < User; end
来源：http://ir.9csxet.cn

C#:   class Admin : User {}
来源：http://nu.nszjky.cn

[G06] 重写方法
来源：http://sv.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://cu.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kd.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://kc.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://gh.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://wj.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mo.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://qy.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://yr.yuexingan06.cn

[G07] 调用父类方法
来源：http://pz.bookmarksfly.cn

Py:   super().greet()
来源：http://wp.colortex.cn

PHP:  parent::greet();
来源：http://mm.hahajie.cn

JS:   super.greet();
来源：http://go.nszjky.cn

TS:   super.greet();
来源：http://rd.jctech888.com.cn

Java: super.greet();
来源：http://hv.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nb.shxzskj.cn

Ruby: super
来源：http://zl.hahajie.cn

C#:   base.Greet();
来源：http://qv.bjjhwx.cn

[G08] 静态方法与属性
来源：http://wh.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lh.yuexingan06.cn

PHP:  public static function f() {}
来源：http://ie.asd995.cn

JS:   static f() {}
来源：http://qu.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://jt.yuntaijiaju.cn

Java: static void f() {}
来源：http://pq.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pk.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://zj.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://lh.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://ce.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://bo.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://io.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jt.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://lv.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://dn.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ku.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ug.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://to.yuexingan06.cn

[G10] 访问控制
来源：http://wl.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://ft.huixiangedu.cn

PHP:  public / protected / private
来源：http://ub.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://nr.wgjwhj.cn

TS:   public / protected / private
来源：http://fy.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://jl.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rt.panjiajie.cn

Ruby: public / protected / private
来源：http://au.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://xj.shtwfgs.cn

[G11] getter / setter
来源：http://fi.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://tp.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uh.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://ro.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://cl.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://ko.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://il.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://oy.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://fm.521024.cn

[G12] 对象转字符串
来源：http://cj.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://xs.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wo.colortex.cn

JS:   toString() { return this.name; }
来源：http://fg.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ge.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://zb.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cf.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://hy.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://vy.wgjwhj.cn

[G13] 判断对象类型
来源：http://zc.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://dz.szsharing.cn

PHP:  $u instanceof User
来源：http://jn.newstarts.cn

JS:   u instanceof User
来源：http://fj.gzmigu.cn

TS:   u instanceof User
来源：http://pw.gzmigu.cn

Java: u instanceof User
来源：http://ih.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mz.szsharing.cn

Ruby: u.is_a?(User)
来源：http://uw.huixinmuqiang.cn

C#:   u is User
来源：http://hu.haigaiapp.cn

[G14] 数据类 / record
来源：http://bc.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bk.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ii.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pq.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://cj.nszjky.cn

Java: record User(String name, int age) {}
来源：http://at.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://oi.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tm.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://ee.chemitech.net.cn

[G15] 枚举
来源：http://bb.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qq.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kf.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ht.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vc.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://om.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mj.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://bq.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eg.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://sa.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tn.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://mc.colortex.cn

JS:   Object.entries(obj)
来源：http://wj.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://sg.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ua.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zv.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://kf.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://um.shxzskj.cn

================================================================================
来源：http://wm.huixinmuqiang.cn

H. 异常与错误处理
来源：http://yx.hahajie.cn

================================================================================
来源：http://ob.nicolike.cn

[H01] try / catch 基础
来源：http://ir.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ye.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rd.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nx.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ub.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ig.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uv.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fo.newstarts.cn

[H02] finally / ensure 收尾
来源：http://fh.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iw.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ak.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nj.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yp.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vb.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vc.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tj.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sn.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://ye.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://rl.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pu.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://wy.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://jr.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://am.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ck.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://du.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tb.haigaiapp.cn

[H04] 自定义异常类型
来源：http://fv.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://vx.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jx.szsharing.cn

JS:   class MyError extends Error {}
来源：http://wo.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://zi.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://dv.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://au.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://cz.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://uj.shtwfgs.cn

[H05] 捕获特定类型
来源：http://yn.hahajie.cn

Py:   except ValueError as e:
来源：http://ry.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://id.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://fo.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://lx.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://hr.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ef.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://wv.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uz.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://qm.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://nr.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fa.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fd.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cw.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jr.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oo.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://wa.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://vc.muxihuayi.cn

[H07] 断言
来源：http://td.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ov.shxzskj.cn

PHP:  assert($x > 0);
来源：http://li.szsharing.cn

JS:   console.assert(x > 0);
来源：http://in.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://kq.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://zo.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qe.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ga.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://vi.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://zg.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://it.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jz.szsharing.cn

JS:   e.message;  e.stack
来源：http://qb.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xc.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ib.lnxyls.cn

Go:   err.Error()
来源：http://sa.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://nj.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://mi.bjjhwx.cn

[H09] 带错误码的异常
来源：http://yx.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iz.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tb.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fy.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rz.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kh.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fl.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://he.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vw.nicolike.cn

[H10] 资源自动释放
来源：http://jg.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://li.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rs.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eb.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cv.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tf.bjjhwx.cn

Go:   defer f.Close()
来源：http://cx.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bm.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mi.bjjhwx.cn

================================================================================
来源：http://xy.muxihuayi.cn

I. 正则表达式
来源：http://ut.yuexingan06.cn

================================================================================
来源：http://bc.jctech888.com.cn

[I01] 判断是否匹配
来源：http://hd.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pz.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://or.asd995.cn

JS:   /\d+/.test(s)
来源：http://lk.szsharing.cn

TS:   /\d+/.test(s)
来源：http://nl.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hd.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sr.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://yh.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bb.521024.cn

[I02] 提取所有匹配
来源：http://by.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://qj.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ih.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zn.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://je.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ce.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bk.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://jc.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tz.szxytkj.cn

[I03] 提取捕获分组
来源：http://tn.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vb.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://od.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sz.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ax.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ge.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xp.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tr.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ef.521024.cn

[I04] 正则替换
来源：http://bg.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zu.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hg.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jz.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://po.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ci.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qr.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://js.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fb.hahajie.cn

[I05] 按正则拆分
来源：http://dm.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://le.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ve.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://ss.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ln.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://gy.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hg.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ll.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sj.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jr.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rn.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uq.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sm.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jk.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mj.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qb.9csxet.cn


<!-- 参考信息 -->