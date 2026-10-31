代发 wailian999

C#:   File.Exists("a.txt")
来源：http://gg.szsharing.cn

[F06] 删除文件
来源：http://ae.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://se.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://gc.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cr.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ld.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kz.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://yq.asd995.cn

Ruby: File.delete("a.txt")
来源：http://la.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://qu.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://jj.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xc.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ld.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uz.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fh.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lt.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ew.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ef.asd995.cn

[F08] 遍历目录
来源：http://hi.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tg.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ml.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://gm.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://mt.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://al.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lp.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://bx.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://bv.wgjwhj.cn

[F09] 获取文件大小
来源：http://bm.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://wo.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://xk.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://bu.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://eb.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lu.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://no.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://ix.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ts.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://uk.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gy.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zv.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://on.szsharing.cn

TS:   path.extname("a.txt")
来源：http://pb.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ye.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yy.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://th.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pi.wgjwhj.cn

[F11] 复制与移动文件
来源：http://oe.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fe.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xe.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uf.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xr.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iv.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://em.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pr.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ga.newstarts.cn

[F12] CSV 读写
来源：http://jq.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ly.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ys.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ti.shxzskj.cn

TS:   // 同上
来源：http://pf.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kk.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fn.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mt.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rn.yuexingan06.cn

================================================================================
来源：http://oa.hahajie.cn

G. 面向对象
来源：http://qo.9csxet.cn

================================================================================
来源：http://gl.chemitech.net.cn

[G01] 定义类
来源：http://af.nicolike.cn

Py:   class User: pass
来源：http://rx.panjiajie.cn

PHP:  class User {}
来源：http://vp.szxytkj.cn

JS:   class User {}
来源：http://hj.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://bx.szsharing.cn

Java: class User {}
来源：http://jd.nicolike.cn

Go:   type User struct { Name string }
来源：http://ca.521024.cn

Ruby: class User; end
来源：http://cb.shxzskj.cn

C#:   class User {}
来源：http://oq.szxytkj.cn

[G02] 构造函数
来源：http://fx.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ka.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://na.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://po.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ik.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://iu.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ok.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://qx.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://xl.shxzukj.cn

[G03] 实例属性
来源：http://ol.szsharing.cn

Py:   self.name = "x"
来源：http://xc.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://qp.colortex.cn

JS:   this.name = "x";
来源：http://zt.szsharing.cn

TS:   name: string = "x";
来源：http://ov.asd995.cn

Java: private String name;
来源：http://zb.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mf.panjiajie.cn

Ruby: @name = "x"
来源：http://ty.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://qi.hnjuh.cn

[G04] 定义方法
来源：http://yd.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://zb.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ct.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://hq.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://hq.asd995.cn

Java: String greet() { return name; }
来源：http://cx.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dv.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://ce.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ye.hahajie.cn

[G05] 继承
来源：http://ue.nicolike.cn

Py:   class Admin(User): pass
来源：http://mq.nicolike.cn

PHP:  class Admin extends User {}
来源：http://dm.szsharing.cn

JS:   class Admin extends User {}
来源：http://op.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://vj.yuexingan06.cn

Java: class Admin extends User {}
来源：http://lm.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://at.9csxet.cn

Ruby: class Admin < User; end
来源：http://qw.nszjky.cn

C#:   class Admin : User {}
来源：http://zc.muxihuayi.cn

[G06] 重写方法
来源：http://je.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://xl.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pp.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://zs.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://yb.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://oq.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bp.521024.cn

Ruby: def greet; "admin"; end
来源：http://ur.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://fr.szsharing.cn

[G07] 调用父类方法
来源：http://fm.hnjuh.cn

Py:   super().greet()
来源：http://nv.haigaiapp.cn

PHP:  parent::greet();
来源：http://ld.newstarts.cn

JS:   super.greet();
来源：http://lt.newstarts.cn

TS:   super.greet();
来源：http://rc.9csxet.cn

Java: super.greet();
来源：http://hs.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://el.huanxung.cn

Ruby: super
来源：http://kx.huixiangedu.cn

C#:   base.Greet();
来源：http://gk.bjjhwx.cn

[G08] 静态方法与属性
来源：http://hy.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://io.shxzskj.cn

PHP:  public static function f() {}
来源：http://sp.muxihuayi.cn

JS:   static f() {}
来源：http://xo.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ls.huixinmuqiang.cn

Java: static void f() {}
来源：http://ft.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jc.panjiajie.cn

Ruby: def self.f; end
来源：http://zz.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://uv.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://wh.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://od.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ja.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vn.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://si.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://lg.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://jt.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qy.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://kk.shtwfgs.cn

[G10] 访问控制
来源：http://is.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://of.szxytkj.cn

PHP:  public / protected / private
来源：http://wc.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://ea.jianghongdianzi.cn

TS:   public / protected / private
来源：http://qz.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://df.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xt.haigaiapp.cn

Ruby: public / protected / private
来源：http://on.szsharing.cn

C#:   public / protected / private / internal
来源：http://ms.panjiajie.cn

[G11] getter / setter
来源：http://wc.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://by.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dd.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://xn.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://pw.asd995.cn

Java: public String getName() { return name; }
来源：http://hf.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yh.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ju.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://xf.gzmigu.cn

[G12] 对象转字符串
来源：http://ih.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://ot.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dq.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://kq.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://un.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://ke.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://go.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://du.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://ph.asd995.cn

[G13] 判断对象类型
来源：http://zl.9csxet.cn

Py:   isinstance(u, User)
来源：http://kv.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://vo.nszjky.cn

JS:   u instanceof User
来源：http://db.panjiajie.cn

TS:   u instanceof User
来源：http://vl.haigaiapp.cn

Java: u instanceof User
来源：http://qr.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dy.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://hh.hahajie.cn

C#:   u is User
来源：http://ca.newstarts.cn

[G14] 数据类 / record
来源：http://yo.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xf.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://zu.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ll.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://pp.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://dh.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://bv.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sn.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://gd.jctech888.com.cn

[G15] 枚举
来源：http://rl.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ne.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ok.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bz.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jl.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://ma.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bi.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://vs.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kc.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://he.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bl.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://wc.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://cg.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ob.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nb.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kz.gzmigu.cn

Ruby: obj.instance_variables
来源：http://lp.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://tn.wgjwhj.cn

================================================================================
来源：http://uc.gzmigu.cn

H. 异常与错误处理
来源：http://lq.colortex.cn

================================================================================
来源：http://im.shxzskj.cn

[H01] try / catch 基础
来源：http://ax.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ye.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rx.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hy.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qg.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xh.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kk.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://do.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mu.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ai.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kg.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hv.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kr.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fj.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wr.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xa.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hf.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jk.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://ph.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://uh.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zj.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://ei.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ke.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xl.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://py.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ze.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jh.colortex.cn

[H04] 自定义异常类型
来源：http://lk.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://dt.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sz.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://yn.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://lc.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://cj.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sn.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://xf.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://oa.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://dx.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://kj.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bz.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://et.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://lc.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://au.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jc.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://lz.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ru.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://kn.hahajie.cn

Py:   value = d.get("k") or default
来源：http://rx.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://me.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://we.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lz.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aq.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mh.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ju.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://nq.yuntaijiaju.cn

[H07] 断言
来源：http://fc.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://fq.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://dx.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://cl.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://qq.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://ax.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qt.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iy.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://yb.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://gb.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://dn.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ii.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://pm.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pe.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ov.newstarts.cn

Go:   err.Error()
来源：http://vj.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://lr.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://lw.shxzukj.cn

[H09] 带错误码的异常
来源：http://wt.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://px.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://if.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fo.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vb.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kp.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ig.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rm.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bz.hnjuh.cn

[H10] 资源自动释放
来源：http://co.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nf.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lq.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ow.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tz.jctech888.com.cn


<!-- 参考信息 -->