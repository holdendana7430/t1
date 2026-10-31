代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://js.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zk.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fd.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fy.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sj.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fx.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ba.bookmarksfly.cn

[F12] CSV 读写
来源：http://cl.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mx.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mm.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pk.szxytkj.cn

TS:   // 同上
来源：http://ix.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gw.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iq.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xt.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uo.yuexingan06.cn

================================================================================
来源：http://wu.huixiangedu.cn

G. 面向对象
来源：http://rq.huixinmuqiang.cn

================================================================================
来源：http://nc.hahajie.cn

[G01] 定义类
来源：http://gq.haigaiapp.cn

Py:   class User: pass
来源：http://cb.bjjhwx.cn

PHP:  class User {}
来源：http://hy.bjjhwx.cn

JS:   class User {}
来源：http://oh.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://po.panjiajie.cn

Java: class User {}
来源：http://mr.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ob.521024.cn

Ruby: class User; end
来源：http://zg.jianghongdianzi.cn

C#:   class User {}
来源：http://wa.shtwfgs.cn

[G02] 构造函数
来源：http://as.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://jr.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ld.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://od.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://cm.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://zv.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oi.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://ud.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://rr.shtwfgs.cn

[G03] 实例属性
来源：http://lm.yuexingan06.cn

Py:   self.name = "x"
来源：http://dl.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://gz.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ih.wgjwhj.cn

TS:   name: string = "x";
来源：http://vq.muxihuayi.cn

Java: private String name;
来源：http://qf.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pl.huanxung.cn

Ruby: @name = "x"
来源：http://xm.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ms.huanxung.cn

[G04] 定义方法
来源：http://gz.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://uc.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jg.newstarts.cn

JS:   greet() { return this.name; }
来源：http://qx.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ix.hnjuh.cn

Java: String greet() { return name; }
来源：http://mu.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rr.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://my.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://ja.wgjwhj.cn

[G05] 继承
来源：http://jd.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ob.521024.cn

PHP:  class Admin extends User {}
来源：http://kv.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://cy.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://oo.shtwfgs.cn

Java: class Admin extends User {}
来源：http://qi.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pw.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://bw.chemitech.net.cn

C#:   class Admin : User {}
来源：http://gm.nicolike.cn

[G06] 重写方法
来源：http://zs.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://ic.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://he.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://ms.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://yt.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://ix.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rh.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://zk.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://ez.521024.cn

[G07] 调用父类方法
来源：http://jy.shtwfgs.cn

Py:   super().greet()
来源：http://zw.jctech888.com.cn

PHP:  parent::greet();
来源：http://nx.yuexingan06.cn

JS:   super.greet();
来源：http://au.huanxung.cn

TS:   super.greet();
来源：http://vp.jianghongdianzi.cn

Java: super.greet();
来源：http://vt.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jo.jianghongdianzi.cn

Ruby: super
来源：http://bh.asd995.cn

C#:   base.Greet();
来源：http://az.huixiangedu.cn

[G08] 静态方法与属性
来源：http://hn.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yt.huixiangedu.cn

PHP:  public static function f() {}
来源：http://qp.panjiajie.cn

JS:   static f() {}
来源：http://cz.colortex.cn

TS:   static f(): void {}
来源：http://nw.nszjky.cn

Java: static void f() {}
来源：http://vh.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pp.lnxyls.cn

Ruby: def self.f; end
来源：http://kf.9csxet.cn

C#:   public static void F() {}
来源：http://lf.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://cc.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://xf.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yt.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zi.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://bp.asd995.cn

Java: interface Shape { double area(); }
来源：http://wg.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://cp.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nh.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://yn.gzmigu.cn

[G10] 访问控制
来源：http://nb.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://bp.yuexingan06.cn

PHP:  public / protected / private
来源：http://sn.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://qx.chemitech.net.cn

TS:   public / protected / private
来源：http://vd.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://by.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hp.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://du.hahajie.cn

C#:   public / protected / private / internal
来源：http://rs.shxzskj.cn

[G11] getter / setter
来源：http://ga.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://fu.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hx.nszjky.cn

JS:   get name() { return this._name; }
来源：http://rs.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://wp.shxzskj.cn

Java: public String getName() { return name; }
来源：http://iv.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xn.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://sc.asd995.cn

C#:   public string Name { get; set; }
来源：http://bk.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://jm.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://kw.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vj.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://wl.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://bo.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://gm.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zh.huanxung.cn

Ruby: def to_s; @name; end
来源：http://dc.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ju.nicolike.cn

[G13] 判断对象类型
来源：http://kk.szxytkj.cn

Py:   isinstance(u, User)
来源：http://pw.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://jo.haigaiapp.cn

JS:   u instanceof User
来源：http://qc.lnxyls.cn

TS:   u instanceof User
来源：http://tq.newstarts.cn

Java: u instanceof User
来源：http://kb.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aj.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://sg.521024.cn

C#:   u is User
来源：http://pg.hnjuh.cn

[G14] 数据类 / record
来源：http://yd.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ul.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://br.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qm.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://ie.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://ew.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://im.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rr.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://at.haigaiapp.cn

[G15] 枚举
来源：http://nj.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://za.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ob.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zh.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ui.521024.cn

Java: enum Color { RED, GREEN }
来源：http://uk.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rv.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://ql.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hh.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://rv.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hu.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://ue.shxzukj.cn

JS:   Object.entries(obj)
来源：http://hy.szxytkj.cn

TS:   Object.entries(obj)
来源：http://xn.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yk.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zl.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://yw.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://xq.jianghongdianzi.cn

================================================================================
来源：http://au.huixinmuqiang.cn

H. 异常与错误处理
来源：http://wj.asd995.cn

================================================================================
来源：http://tb.shxzskj.cn

[H01] try / catch 基础
来源：http://qv.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zx.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ix.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qj.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vw.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yn.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dw.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pn.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xt.newstarts.cn

[H02] finally / ensure 收尾
来源：http://xe.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mc.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iy.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ih.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tk.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wx.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iu.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rw.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vb.gzmigu.cn

[H03] 主动抛出异常
来源：http://ds.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://yz.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gf.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://aa.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://kw.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gv.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ij.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://am.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xi.wgjwhj.cn

[H04] 自定义异常类型
来源：http://al.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://dl.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sf.colortex.cn

JS:   class MyError extends Error {}
来源：http://qm.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://uk.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://ic.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wy.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ar.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://bp.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://wb.nicolike.cn

Py:   except ValueError as e:
来源：http://pp.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gm.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://fh.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://wy.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ri.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zk.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://wc.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xy.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://ld.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://sq.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nc.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zw.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cj.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zo.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://os.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://ex.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://kb.huixinmuqiang.cn

[H07] 断言
来源：http://ww.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://mh.hnjuh.cn

PHP:  assert($x > 0);
来源：http://hf.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://nt.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://rs.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://oj.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://og.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zn.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://vb.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://hf.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ze.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yl.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://yy.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wj.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ir.wgjwhj.cn

Go:   err.Error()
来源：http://bc.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://zu.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://li.panjiajie.cn

[H09] 带错误码的异常
来源：http://qh.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vk.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ns.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jc.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bi.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ek.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fr.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hs.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ed.wgjwhj.cn

[H10] 资源自动释放
来源：http://cj.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cs.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sk.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://js.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ew.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ao.asd995.cn

Go:   defer f.Close()
来源：http://ib.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hc.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jr.jctech888.com.cn

================================================================================
来源：http://qu.yuexingan06.cn

I. 正则表达式
来源：http://xt.shxzskj.cn

================================================================================
来源：http://wx.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://wk.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mp.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vt.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://wc.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://jx.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cj.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uf.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://tq.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dj.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://vz.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://vd.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ox.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ct.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://hp.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fr.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ly.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://wf.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qc.szxytkj.cn

[I03] 提取捕获分组
来源：http://ji.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xq.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ud.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dq.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ez.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zn.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ew.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ha.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oj.hnjuh.cn

[I04] 正则替换
来源：http://tp.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bk.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ov.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dw.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ew.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jm.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sp.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uj.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jf.colortex.cn

[I05] 按正则拆分
来源：http://fk.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://na.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xw.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://ml.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://vd.shtwfgs.cn


<!-- 参考信息 -->