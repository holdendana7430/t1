代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://gz.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://xi.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pm.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tx.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bt.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://nr.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yg.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kp.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tq.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lm.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://md.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://it.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ml.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://he.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cl.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sf.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ob.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wx.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bd.huixiangedu.cn

[F12] CSV 读写
来源：http://vk.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://on.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rw.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hr.colortex.cn

TS:   // 同上
来源：http://tc.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qt.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ik.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zc.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ya.521024.cn

================================================================================
来源：http://va.huanxung.cn

G. 面向对象
来源：http://bj.muxihuayi.cn

================================================================================
来源：http://uj.bjjhwx.cn

[G01] 定义类
来源：http://ts.lnxyls.cn

Py:   class User: pass
来源：http://ez.shxzukj.cn

PHP:  class User {}
来源：http://nq.gzmigu.cn

JS:   class User {}
来源：http://tk.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://qy.jctech888.com.cn

Java: class User {}
来源：http://wy.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://it.nicolike.cn

Ruby: class User; end
来源：http://jc.szxytkj.cn

C#:   class User {}
来源：http://nd.muxihuayi.cn

[G02] 构造函数
来源：http://gv.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://dm.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fw.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://js.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ly.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://mz.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vz.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://qa.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://hg.jianghongdianzi.cn

[G03] 实例属性
来源：http://or.gzmigu.cn

Py:   self.name = "x"
来源：http://oa.shxzukj.cn

PHP:  public string $name = "x";
来源：http://av.muxihuayi.cn

JS:   this.name = "x";
来源：http://rg.hnjuh.cn

TS:   name: string = "x";
来源：http://op.shxzukj.cn

Java: private String name;
来源：http://na.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yf.newstarts.cn

Ruby: @name = "x"
来源：http://uc.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://ha.bookmarksfly.cn

[G04] 定义方法
来源：http://km.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://rj.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://we.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://bi.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://au.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ra.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dd.nszjky.cn

Ruby: def greet; @name; end
来源：http://cz.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://sf.muxihuayi.cn

[G05] 继承
来源：http://db.asd995.cn

Py:   class Admin(User): pass
来源：http://xd.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://hs.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://vo.nicolike.cn

TS:   class Admin extends User {}
来源：http://dj.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://vv.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mx.szsharing.cn

Ruby: class Admin < User; end
来源：http://sn.shxzukj.cn

C#:   class Admin : User {}
来源：http://zv.hahajie.cn

[G06] 重写方法
来源：http://ql.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://vc.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://od.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://sf.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://mr.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://uv.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hd.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://tk.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://ig.hnjuh.cn

[G07] 调用父类方法
来源：http://zq.wgjwhj.cn

Py:   super().greet()
来源：http://lu.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://yd.hahajie.cn

JS:   super.greet();
来源：http://kq.huixinmuqiang.cn

TS:   super.greet();
来源：http://hg.521024.cn

Java: super.greet();
来源：http://od.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mx.nszjky.cn

Ruby: super
来源：http://zm.muxihuayi.cn

C#:   base.Greet();
来源：http://fo.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://aa.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hx.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://dj.huixiangedu.cn

JS:   static f() {}
来源：http://qn.shtwfgs.cn

TS:   static f(): void {}
来源：http://zy.shtwfgs.cn

Java: static void f() {}
来源：http://kv.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xl.bjjhwx.cn

Ruby: def self.f; end
来源：http://vj.asd995.cn

C#:   public static void F() {}
来源：http://qz.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://ig.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://jz.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tg.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wa.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://oe.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://cy.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://jb.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lv.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://tk.shxzukj.cn

[G10] 访问控制
来源：http://ig.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://rh.haigaiapp.cn

PHP:  public / protected / private
来源：http://fq.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://tl.wgjwhj.cn

TS:   public / protected / private
来源：http://ih.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://cw.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xn.asd995.cn

Ruby: public / protected / private
来源：http://ih.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://ga.521024.cn

[G11] getter / setter
来源：http://wx.colortex.cn

Py:   @property 与 @x.setter
来源：http://ck.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fg.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://bz.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://qw.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://xl.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wv.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://fu.newstarts.cn

C#:   public string Name { get; set; }
来源：http://xw.muxihuayi.cn

[G12] 对象转字符串
来源：http://vp.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://ba.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ia.asd995.cn

JS:   toString() { return this.name; }
来源：http://dg.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://fo.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://sb.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ar.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://ii.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://jc.asd995.cn

[G13] 判断对象类型
来源：http://td.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://is.colortex.cn

PHP:  $u instanceof User
来源：http://ls.haigaiapp.cn

JS:   u instanceof User
来源：http://ls.asd995.cn

TS:   u instanceof User
来源：http://ee.colortex.cn

Java: u instanceof User
来源：http://zu.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rx.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://yv.nszjky.cn

C#:   u is User
来源：http://rs.huanxung.cn

[G14] 数据类 / record
来源：http://hz.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ev.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://uf.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rb.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://uk.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://jq.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://hm.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qz.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://dd.huixinmuqiang.cn

[G15] 枚举
来源：http://hf.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bh.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mi.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hh.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uv.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://io.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oa.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://mi.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ql.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://nr.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zj.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://et.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ht.szxytkj.cn

TS:   Object.entries(obj)
来源：http://cx.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dj.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://is.colortex.cn

Ruby: obj.instance_variables
来源：http://nv.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pc.newstarts.cn

================================================================================
来源：http://hd.hnjuh.cn

H. 异常与错误处理
来源：http://uv.huanxung.cn

================================================================================
来源：http://eu.bjjhwx.cn

[H01] try / catch 基础
来源：http://le.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zq.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kp.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xr.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gw.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ha.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hv.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ek.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ig.hahajie.cn

[H02] finally / ensure 收尾
来源：http://kk.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sv.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ve.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fq.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oc.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uc.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://db.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pr.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hk.colortex.cn

[H03] 主动抛出异常
来源：http://km.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://mc.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://et.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://la.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://nx.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fw.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://il.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qy.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rf.newstarts.cn

[H04] 自定义异常类型
来源：http://ri.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ps.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dz.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://on.521024.cn

TS:   class MyError extends Error {}
来源：http://xz.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://hm.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fn.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://lj.hahajie.cn

C#:   class MyException : Exception {}
来源：http://kz.yuexingan06.cn

[H05] 捕获特定类型
来源：http://nb.muxihuayi.cn

Py:   except ValueError as e:
来源：http://kv.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vd.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://jj.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://eh.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ec.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ig.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://fc.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ft.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://th.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://qt.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pa.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vf.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qn.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tl.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ws.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://wz.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://yy.chemitech.net.cn

[H07] 断言
来源：http://yo.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://km.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://mq.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ga.nicolike.cn

TS:   console.assert(x > 0);
来源：http://tp.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://wu.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jc.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://he.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://hk.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ld.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://iv.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ig.9csxet.cn

JS:   e.message;  e.stack
来源：http://jz.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ly.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ew.bookmarksfly.cn

Go:   err.Error()
来源：http://lz.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://fs.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ul.szxytkj.cn

[H09] 带错误码的异常
来源：http://dr.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rr.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cq.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zl.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://og.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vm.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xi.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ht.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yq.9csxet.cn

[H10] 资源自动释放
来源：http://ep.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ni.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vq.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lh.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rk.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lv.asd995.cn

Go:   defer f.Close()
来源：http://rq.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pc.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gs.lnxyls.cn

================================================================================
来源：http://hg.chemitech.net.cn

I. 正则表达式
来源：http://ik.shtwfgs.cn

================================================================================
来源：http://ao.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://za.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jo.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jl.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://td.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ax.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://by.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uj.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://sb.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://al.521024.cn

[I02] 提取所有匹配
来源：http://zw.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://uk.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sl.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bw.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://fv.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sh.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ww.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://zr.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hf.gzmigu.cn

[I03] 提取捕获分组
来源：http://op.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mi.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fi.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yx.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://go.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lm.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pa.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jj.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rh.hnjuh.cn

[I04] 正则替换
来源：http://zq.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ig.nicolike.cn


<!-- 参考信息 -->