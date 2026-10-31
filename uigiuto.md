代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ab.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mf.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ea.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mv.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://po.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ja.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wp.chemitech.net.cn

[F12] CSV 读写
来源：http://yl.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mx.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ll.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jr.muxihuayi.cn

TS:   // 同上
来源：http://ox.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jg.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mn.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://na.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://um.shxzukj.cn

================================================================================
来源：http://bj.shxzskj.cn

G. 面向对象
来源：http://wp.yuntaijiaju.cn

================================================================================
来源：http://sb.newstarts.cn

[G01] 定义类
来源：http://zb.bookmarksfly.cn

Py:   class User: pass
来源：http://jr.shxzukj.cn

PHP:  class User {}
来源：http://kp.shtwfgs.cn

JS:   class User {}
来源：http://nw.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://tb.shxzukj.cn

Java: class User {}
来源：http://gj.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://ne.shtwfgs.cn

Ruby: class User; end
来源：http://wu.huanxung.cn

C#:   class User {}
来源：http://ox.panjiajie.cn

[G02] 构造函数
来源：http://nc.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://bi.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://ul.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://de.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://xc.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://iv.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mg.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://ow.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://aa.szsharing.cn

[G03] 实例属性
来源：http://lb.muxihuayi.cn

Py:   self.name = "x"
来源：http://ga.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://zs.shxzukj.cn

JS:   this.name = "x";
来源：http://wh.lnxyls.cn

TS:   name: string = "x";
来源：http://kl.jctech888.com.cn

Java: private String name;
来源：http://qx.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://py.asd995.cn

Ruby: @name = "x"
来源：http://gk.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zc.bookmarksfly.cn

[G04] 定义方法
来源：http://at.asd995.cn

Py:   def greet(self): return self.name
来源：http://ek.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://st.521024.cn

JS:   greet() { return this.name; }
来源：http://ey.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://yo.haigaiapp.cn

Java: String greet() { return name; }
来源：http://vh.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pc.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://tg.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://yz.huanxung.cn

[G05] 继承
来源：http://bn.panjiajie.cn

Py:   class Admin(User): pass
来源：http://ie.hahajie.cn

PHP:  class Admin extends User {}
来源：http://gx.9csxet.cn

JS:   class Admin extends User {}
来源：http://lk.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://iy.hnjuh.cn

Java: class Admin extends User {}
来源：http://qw.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://if.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://sc.nicolike.cn

C#:   class Admin : User {}
来源：http://so.huanxung.cn

[G06] 重写方法
来源：http://dg.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://tz.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gt.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://zc.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://zm.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://bq.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://et.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://qd.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://ca.lnxyls.cn

[G07] 调用父类方法
来源：http://to.shxzukj.cn

Py:   super().greet()
来源：http://di.panjiajie.cn

PHP:  parent::greet();
来源：http://ek.hahajie.cn

JS:   super.greet();
来源：http://ql.jctech888.com.cn

TS:   super.greet();
来源：http://bi.shxzukj.cn

Java: super.greet();
来源：http://tt.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xo.hnjuh.cn

Ruby: super
来源：http://kh.szxytkj.cn

C#:   base.Greet();
来源：http://ui.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://on.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ia.jctech888.com.cn

PHP:  public static function f() {}
来源：http://qn.huixinmuqiang.cn

JS:   static f() {}
来源：http://ib.521024.cn

TS:   static f(): void {}
来源：http://gz.wgjwhj.cn

Java: static void f() {}
来源：http://gj.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qd.newstarts.cn

Ruby: def self.f; end
来源：http://dv.hnjuh.cn

C#:   public static void F() {}
来源：http://cw.newstarts.cn

[G09] 接口 / 抽象类
来源：http://pa.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://jq.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ua.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://so.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://tl.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://tp.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://nr.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://za.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://bt.nszjky.cn

[G10] 访问控制
来源：http://gl.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://az.521024.cn

PHP:  public / protected / private
来源：http://ke.asd995.cn

JS:   #private 字段；其余公开
来源：http://ae.szsharing.cn

TS:   public / protected / private
来源：http://jl.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://ay.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ga.bjjhwx.cn

Ruby: public / protected / private
来源：http://ms.hahajie.cn

C#:   public / protected / private / internal
来源：http://ky.huixinmuqiang.cn

[G11] getter / setter
来源：http://al.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://pt.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qx.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://lf.521024.cn

TS:   get name(): string { return this._name; }
来源：http://sf.lnxyls.cn

Java: public String getName() { return name; }
来源：http://xc.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://us.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://ce.asd995.cn

C#:   public string Name { get; set; }
来源：http://wu.shxzukj.cn

[G12] 对象转字符串
来源：http://uf.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ci.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cr.9csxet.cn

JS:   toString() { return this.name; }
来源：http://mh.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://sy.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://bf.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://az.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://cm.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://gp.hnjuh.cn

[G13] 判断对象类型
来源：http://qs.panjiajie.cn

Py:   isinstance(u, User)
来源：http://qc.colortex.cn

PHP:  $u instanceof User
来源：http://cx.yuexingan06.cn

JS:   u instanceof User
来源：http://mp.wgjwhj.cn

TS:   u instanceof User
来源：http://qr.shtwfgs.cn

Java: u instanceof User
来源：http://pf.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sh.colortex.cn

Ruby: u.is_a?(User)
来源：http://kb.hnjuh.cn

C#:   u is User
来源：http://uw.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://ck.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rz.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://wk.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://na.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://tk.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://hj.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://mm.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kq.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://ot.wgjwhj.cn

[G15] 枚举
来源：http://ck.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://if.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bv.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vd.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gq.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://mv.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ic.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ji.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iq.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://sx.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ky.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://yh.shxzukj.cn

JS:   Object.entries(obj)
来源：http://le.asd995.cn

TS:   Object.entries(obj)
来源：http://tr.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vt.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://la.nicolike.cn

Ruby: obj.instance_variables
来源：http://si.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://hn.nicolike.cn

================================================================================
来源：http://iv.yuexingan06.cn

H. 异常与错误处理
来源：http://fd.asd995.cn

================================================================================
来源：http://re.lnxyls.cn

[H01] try / catch 基础
来源：http://jg.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ew.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://da.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ns.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kx.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uh.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zf.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ry.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qq.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://ve.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dw.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ec.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gv.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jl.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zm.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lh.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ff.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yl.newstarts.cn

[H03] 主动抛出异常
来源：http://vg.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://fk.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pd.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://in.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://ge.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ya.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ly.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qh.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xc.shtwfgs.cn

[H04] 自定义异常类型
来源：http://gu.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ar.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ly.hahajie.cn

JS:   class MyError extends Error {}
来源：http://uo.newstarts.cn

TS:   class MyError extends Error {}
来源：http://gl.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://vw.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rh.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://dm.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://xp.szxytkj.cn

[H05] 捕获特定类型
来源：http://ft.hnjuh.cn

Py:   except ValueError as e:
来源：http://vj.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ld.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://fr.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://hk.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://jf.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hi.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://de.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ud.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ux.nszjky.cn

Py:   value = d.get("k") or default
来源：http://wk.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pl.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rx.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ve.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://su.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://be.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://pi.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://hz.wgjwhj.cn

[H07] 断言
来源：http://eb.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://dt.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://bo.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://eo.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://st.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://bi.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jt.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bu.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://ic.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://bg.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ix.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wz.newstarts.cn

JS:   e.message;  e.stack
来源：http://oo.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bs.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ax.newstarts.cn

Go:   err.Error()
来源：http://zr.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://ql.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://rk.haigaiapp.cn

[H09] 带错误码的异常
来源：http://te.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ht.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://db.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tp.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ak.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rj.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xc.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tt.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uc.jctech888.com.cn

[H10] 资源自动释放
来源：http://xm.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sl.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ma.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jg.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bk.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sc.wgjwhj.cn

Go:   defer f.Close()
来源：http://rd.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vk.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gb.wgjwhj.cn

================================================================================
来源：http://rn.521024.cn

I. 正则表达式
来源：http://tq.jianghongdianzi.cn

================================================================================
来源：http://cv.wgjwhj.cn

[I01] 判断是否匹配
来源：http://ix.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jh.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yu.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://hh.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://jb.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ib.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pq.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://gq.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zr.haigaiapp.cn

[I02] 提取所有匹配
来源：http://dm.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://jw.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ig.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aw.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://ji.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ta.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gs.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://fj.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jq.9csxet.cn

[I03] 提取捕获分组
来源：http://pg.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ch.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nm.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tz.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zq.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dd.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kp.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zv.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lo.panjiajie.cn

[I04] 正则替换
来源：http://ho.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bs.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lp.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tt.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kg.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gj.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dr.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yr.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yz.asd995.cn

[I05] 按正则拆分
来源：http://ej.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ae.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ny.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://nc.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://rl.wgjwhj.cn


<!-- 参考信息 -->