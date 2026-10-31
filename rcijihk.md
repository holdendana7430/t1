代发 wailian999

Ruby: File.delete("a.txt")
来源：http://rh.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://lt.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://tm.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tx.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cc.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ip.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://no.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://an.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://op.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bx.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://up.yuexingan06.cn

[F08] 遍历目录
来源：http://eb.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://af.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ao.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://tq.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://hu.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gy.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ws.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://tp.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://up.wgjwhj.cn

[F09] 获取文件大小
来源：http://wj.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://bb.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://hb.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://bz.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ku.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ox.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qo.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://zh.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://fn.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://am.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gr.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wj.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wr.nicolike.cn

TS:   path.extname("a.txt")
来源：http://gk.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tj.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ot.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yp.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sm.szxytkj.cn

[F11] 复制与移动文件
来源：http://eo.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aw.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://su.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hu.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://af.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lx.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ff.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ax.haigaiapp.cn

[F12] CSV 读写
来源：http://jo.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zg.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jt.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ms.huixinmuqiang.cn

TS:   // 同上
来源：http://kg.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rb.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://br.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dj.newstarts.cn

================================================================================
来源：http://nm.szsharing.cn

G. 面向对象
来源：http://lm.huixinmuqiang.cn

================================================================================
来源：http://hd.jianghongdianzi.cn

[G01] 定义类
来源：http://rv.nicolike.cn

Py:   class User: pass
来源：http://zv.hnjuh.cn

PHP:  class User {}
来源：http://yz.wgjwhj.cn

JS:   class User {}
来源：http://sk.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://zn.huanxung.cn

Java: class User {}
来源：http://mb.nicolike.cn

Go:   type User struct { Name string }
来源：http://qj.panjiajie.cn

Ruby: class User; end
来源：http://us.asd995.cn

C#:   class User {}
来源：http://rf.521024.cn

[G02] 构造函数
来源：http://ih.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://zi.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://av.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ny.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://ge.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://eg.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ce.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://wo.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://nk.szsharing.cn

[G03] 实例属性
来源：http://tm.bjjhwx.cn

Py:   self.name = "x"
来源：http://oh.newstarts.cn

PHP:  public string $name = "x";
来源：http://do.hahajie.cn

JS:   this.name = "x";
来源：http://jt.gzmigu.cn

TS:   name: string = "x";
来源：http://et.szxytkj.cn

Java: private String name;
来源：http://yn.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ju.hahajie.cn

Ruby: @name = "x"
来源：http://ef.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ib.huixinmuqiang.cn

[G04] 定义方法
来源：http://gd.colortex.cn

Py:   def greet(self): return self.name
来源：http://gk.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wi.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://tp.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://li.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ky.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xi.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://vo.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://gu.bjjhwx.cn

[G05] 继承
来源：http://pj.lnxyls.cn

Py:   class Admin(User): pass
来源：http://uc.huanxung.cn

PHP:  class Admin extends User {}
来源：http://hk.nicolike.cn

JS:   class Admin extends User {}
来源：http://ht.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://pu.nszjky.cn

Java: class Admin extends User {}
来源：http://pn.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zv.huanxung.cn

Ruby: class Admin < User; end
来源：http://ly.colortex.cn

C#:   class Admin : User {}
来源：http://tg.lnxyls.cn

[G06] 重写方法
来源：http://je.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://in.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://aw.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://zq.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://yp.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://gq.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ta.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://rd.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://py.shxzukj.cn

[G07] 调用父类方法
来源：http://iu.bjjhwx.cn

Py:   super().greet()
来源：http://dz.muxihuayi.cn

PHP:  parent::greet();
来源：http://ib.huixinmuqiang.cn

JS:   super.greet();
来源：http://oq.jctech888.com.cn

TS:   super.greet();
来源：http://ni.lnxyls.cn

Java: super.greet();
来源：http://qi.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fb.521024.cn

Ruby: super
来源：http://mc.yuntaijiaju.cn

C#:   base.Greet();
来源：http://oi.yuexingan06.cn

[G08] 静态方法与属性
来源：http://fn.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ze.muxihuayi.cn

PHP:  public static function f() {}
来源：http://os.gzmigu.cn

JS:   static f() {}
来源：http://jg.bookmarksfly.cn

TS:   static f(): void {}
来源：http://bm.asd995.cn

Java: static void f() {}
来源：http://ns.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vi.haigaiapp.cn

Ruby: def self.f; end
来源：http://av.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://yj.asd995.cn

[G09] 接口 / 抽象类
来源：http://js.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://yi.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kn.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://te.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://jv.huanxung.cn

Java: interface Shape { double area(); }
来源：http://dv.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://bv.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gi.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://lc.muxihuayi.cn

[G10] 访问控制
来源：http://fo.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://sf.panjiajie.cn

PHP:  public / protected / private
来源：http://ae.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://ud.gzmigu.cn

TS:   public / protected / private
来源：http://ng.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ox.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lh.521024.cn

Ruby: public / protected / private
来源：http://lr.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://fo.szsharing.cn

[G11] getter / setter
来源：http://av.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://wg.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cj.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://ut.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ju.hnjuh.cn

Java: public String getName() { return name; }
来源：http://kn.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zi.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ag.9csxet.cn

C#:   public string Name { get; set; }
来源：http://ep.hahajie.cn

[G12] 对象转字符串
来源：http://jr.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://hx.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mh.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://hg.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://fs.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://yb.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://he.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://jx.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://gt.wgjwhj.cn

[G13] 判断对象类型
来源：http://pj.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://ux.yuexingan06.cn

PHP:  $u instanceof User
来源：http://al.jctech888.com.cn

JS:   u instanceof User
来源：http://fc.521024.cn

TS:   u instanceof User
来源：http://ak.muxihuayi.cn

Java: u instanceof User
来源：http://ef.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rz.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://hw.bjjhwx.cn

C#:   u is User
来源：http://ki.asd995.cn

[G14] 数据类 / record
来源：http://le.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qa.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://kl.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://su.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ig.9csxet.cn

Java: record User(String name, int age) {}
来源：http://vn.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://mb.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hb.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ti.shtwfgs.cn

[G15] 枚举
来源：http://xk.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wc.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sw.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qw.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hc.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://bp.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lj.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://vw.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ud.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://cx.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zv.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://yn.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://go.9csxet.cn

TS:   Object.entries(obj)
来源：http://md.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vb.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kg.nszjky.cn

Ruby: obj.instance_variables
来源：http://yj.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://hc.jianghongdianzi.cn

================================================================================
来源：http://sa.muxihuayi.cn

H. 异常与错误处理
来源：http://gm.newstarts.cn

================================================================================
来源：http://dx.panjiajie.cn

[H01] try / catch 基础
来源：http://rb.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ia.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rz.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cf.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dl.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ca.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uc.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wg.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cb.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ih.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tp.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ko.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ad.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wp.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wk.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ut.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uh.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yz.muxihuayi.cn

[H03] 主动抛出异常
来源：http://de.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://zi.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bv.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://ob.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://yw.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pb.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://js.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ug.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mi.huanxung.cn

[H04] 自定义异常类型
来源：http://of.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://nz.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jo.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://jg.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://sv.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://jq.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yv.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ni.huanxung.cn

C#:   class MyException : Exception {}
来源：http://ey.hahajie.cn

[H05] 捕获特定类型
来源：http://ab.colortex.cn

Py:   except ValueError as e:
来源：http://hk.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qf.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://je.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://lm.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://lq.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zq.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://vf.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hi.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://tw.nicolike.cn

Py:   value = d.get("k") or default
来源：http://er.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hu.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bh.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://af.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gr.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qw.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://hy.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://fw.nicolike.cn

[H07] 断言
来源：http://fo.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://pe.shxzskj.cn

PHP:  assert($x > 0);
来源：http://vp.hahajie.cn

JS:   console.assert(x > 0);
来源：http://cz.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://hz.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://ag.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uh.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ns.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://xz.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ew.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ji.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pa.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://mt.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ej.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ej.szsharing.cn

Go:   err.Error()
来源：http://rb.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://jc.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://hf.colortex.cn

[H09] 带错误码的异常
来源：http://ft.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://at.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dq.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qa.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iy.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sa.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ev.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gv.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nq.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://yk.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fh.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://md.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yz.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ao.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hu.huixiangedu.cn

Go:   defer f.Close()
来源：http://ka.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gy.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sj.szxytkj.cn

================================================================================
来源：http://bg.huixiangedu.cn

I. 正则表达式
来源：http://tr.huixiangedu.cn

================================================================================
来源：http://ij.nszjky.cn

[I01] 判断是否匹配
来源：http://si.lnxyls.cn


<!-- 参考信息 -->