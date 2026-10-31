代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://db.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rq.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://xi.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ry.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://fb.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://my.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cr.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://di.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://xf.colortex.cn

[F06] 删除文件
来源：http://hd.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://ho.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://nq.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cs.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rz.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kb.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://au.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://jq.colortex.cn

C#:   File.Delete("a.txt");
来源：http://xa.asd995.cn

[F07] 创建目录（含多级）
来源：http://tg.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qn.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hv.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bi.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uo.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://of.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yi.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vl.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://af.shxzukj.cn

[F08] 遍历目录
来源：http://gg.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zl.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cg.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://jp.521024.cn

TS:   fs.readdirSync("dir")
来源：http://bg.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qp.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ma.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://dm.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://hi.newstarts.cn

[F09] 获取文件大小
来源：http://cl.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://yp.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://hj.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://tu.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://aw.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oj.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://el.colortex.cn

Ruby: File.size("a.txt")
来源：http://ye.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://xt.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://pm.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kh.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gf.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://me.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://kl.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ot.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yu.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ii.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://de.hnjuh.cn

[F11] 复制与移动文件
来源：http://nm.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dz.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nl.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://an.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ll.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ed.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ba.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wx.szxytkj.cn

[F12] CSV 读写
来源：http://ll.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ic.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xb.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bn.panjiajie.cn

TS:   // 同上
来源：http://wa.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zl.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kk.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jw.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kj.yuexingan06.cn

================================================================================
来源：http://ll.nszjky.cn

G. 面向对象
来源：http://bq.huixinmuqiang.cn

================================================================================
来源：http://ib.9csxet.cn

[G01] 定义类
来源：http://co.shxzskj.cn

Py:   class User: pass
来源：http://wc.yuexingan06.cn

PHP:  class User {}
来源：http://jm.hahajie.cn

JS:   class User {}
来源：http://kq.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://rx.huixiangedu.cn

Java: class User {}
来源：http://wq.gzmigu.cn

Go:   type User struct { Name string }
来源：http://un.bookmarksfly.cn

Ruby: class User; end
来源：http://un.muxihuayi.cn

C#:   class User {}
来源：http://jz.jctech888.com.cn

[G02] 构造函数
来源：http://rm.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://je.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://ea.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://kb.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://va.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://ek.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wx.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://cx.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://cn.lnxyls.cn

[G03] 实例属性
来源：http://er.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://sr.szxytkj.cn

PHP:  public string $name = "x";
来源：http://rv.asd995.cn

JS:   this.name = "x";
来源：http://fv.nszjky.cn

TS:   name: string = "x";
来源：http://cy.gzmigu.cn

Java: private String name;
来源：http://qm.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yu.hnjuh.cn

Ruby: @name = "x"
来源：http://zs.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://xs.lnxyls.cn

[G04] 定义方法
来源：http://ll.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ve.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ru.szsharing.cn

JS:   greet() { return this.name; }
来源：http://wj.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://vi.nicolike.cn

Java: String greet() { return name; }
来源：http://bb.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xf.shxzskj.cn

Ruby: def greet; @name; end
来源：http://ns.huanxung.cn

C#:   public string Greet() => Name;
来源：http://ba.szsharing.cn

[G05] 继承
来源：http://os.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://pm.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://cy.9csxet.cn

JS:   class Admin extends User {}
来源：http://qu.521024.cn

TS:   class Admin extends User {}
来源：http://kz.panjiajie.cn

Java: class Admin extends User {}
来源：http://ee.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gq.szxytkj.cn

Ruby: class Admin < User; end
来源：http://tq.gzmigu.cn

C#:   class Admin : User {}
来源：http://am.wgjwhj.cn

[G06] 重写方法
来源：http://vb.colortex.cn

Py:   def greet(self): return "admin"
来源：http://te.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kc.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://wz.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://zb.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://pb.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qm.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://as.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://fi.bookmarksfly.cn

[G07] 调用父类方法
来源：http://sw.jianghongdianzi.cn

Py:   super().greet()
来源：http://ex.szsharing.cn

PHP:  parent::greet();
来源：http://qd.yuntaijiaju.cn

JS:   super.greet();
来源：http://qt.jctech888.com.cn

TS:   super.greet();
来源：http://mg.hahajie.cn

Java: super.greet();
来源：http://mk.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ty.asd995.cn

Ruby: super
来源：http://to.newstarts.cn

C#:   base.Greet();
来源：http://bf.nicolike.cn

[G08] 静态方法与属性
来源：http://qh.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fg.wgjwhj.cn

PHP:  public static function f() {}
来源：http://za.newstarts.cn

JS:   static f() {}
来源：http://hw.hnjuh.cn

TS:   static f(): void {}
来源：http://tg.huanxung.cn

Java: static void f() {}
来源：http://tf.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rc.huanxung.cn

Ruby: def self.f; end
来源：http://dj.shxzskj.cn

C#:   public static void F() {}
来源：http://oz.newstarts.cn

[G09] 接口 / 抽象类
来源：http://ry.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://te.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://as.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fk.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://ti.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://bl.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://ok.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://im.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://fo.yuntaijiaju.cn

[G10] 访问控制
来源：http://hk.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://re.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gt.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ga.bjjhwx.cn

TS:   public / protected / private
来源：http://tc.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://pz.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nw.chemitech.net.cn

Ruby: public / protected / private
来源：http://bw.panjiajie.cn

C#:   public / protected / private / internal
来源：http://sj.jctech888.com.cn

[G11] getter / setter
来源：http://fz.521024.cn

Py:   @property 与 @x.setter
来源：http://cg.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xp.hahajie.cn

JS:   get name() { return this._name; }
来源：http://tq.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://dz.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://wj.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tx.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://aq.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://zz.muxihuayi.cn

[G12] 对象转字符串
来源：http://rh.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://pj.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vj.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://qm.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://cq.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://un.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ra.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://se.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://rh.nicolike.cn

[G13] 判断对象类型
来源：http://en.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://ms.szxytkj.cn

PHP:  $u instanceof User
来源：http://yb.lnxyls.cn

JS:   u instanceof User
来源：http://uf.huixinmuqiang.cn

TS:   u instanceof User
来源：http://xm.nszjky.cn

Java: u instanceof User
来源：http://hd.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wk.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://ql.bjjhwx.cn

C#:   u is User
来源：http://is.huanxung.cn

[G14] 数据类 / record
来源：http://sf.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://js.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://ru.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uf.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://fg.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://nx.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://ta.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bu.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://ff.jianghongdianzi.cn

[G15] 枚举
来源：http://wg.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fi.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ja.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://or.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xw.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://co.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sy.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://pj.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kq.521024.cn

[G16] 对象转数组 / 字典
来源：http://tz.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://au.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://oi.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://kt.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://xv.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://up.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xl.hnjuh.cn

Ruby: obj.instance_variables
来源：http://az.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ru.shtwfgs.cn

================================================================================
来源：http://sd.huixiangedu.cn

H. 异常与错误处理
来源：http://te.shxzskj.cn

================================================================================
来源：http://tm.shxzskj.cn

[H01] try / catch 基础
来源：http://nj.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ki.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pu.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ua.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cv.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cq.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jr.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lp.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sg.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://yn.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mf.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vd.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://re.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yt.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vk.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lj.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ns.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hl.huanxung.cn

[H03] 主动抛出异常
来源：http://sb.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://ph.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mu.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://fs.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://rc.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jg.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qt.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ui.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bu.bjjhwx.cn

[H04] 自定义异常类型
来源：http://gm.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://qs.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cc.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://oc.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://gh.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://bf.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ji.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://jj.9csxet.cn

C#:   class MyException : Exception {}
来源：http://si.9csxet.cn

[H05] 捕获特定类型
来源：http://yc.muxihuayi.cn

Py:   except ValueError as e:
来源：http://id.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oc.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://yj.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://gh.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://hb.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zr.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://dt.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://di.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://lk.huanxung.cn

Py:   value = d.get("k") or default
来源：http://fa.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xt.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pz.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bv.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bd.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ll.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://xc.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://we.colortex.cn

[H07] 断言
来源：http://fa.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://lm.asd995.cn

PHP:  assert($x > 0);
来源：http://kc.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://jk.nszjky.cn

TS:   console.assert(x > 0);
来源：http://wj.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://jx.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jp.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ef.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://mz.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://qw.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://dw.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pz.szxytkj.cn

JS:   e.message;  e.stack
来源：http://rv.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mn.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rd.huixinmuqiang.cn

Go:   err.Error()
来源：http://vx.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://kb.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://vh.haigaiapp.cn

[H09] 带错误码的异常
来源：http://sx.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rd.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zn.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nm.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zw.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sl.colortex.cn


<!-- 参考信息 -->