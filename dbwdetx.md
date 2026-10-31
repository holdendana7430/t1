代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://gl.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vb.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ah.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://fw.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://zc.bookmarksfly.cn

[F06] 删除文件
来源：http://zt.huanxung.cn

Py:   os.remove("a.txt")
来源：http://nb.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://lg.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bg.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rw.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ih.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://zu.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://fz.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://gb.huanxung.cn

[F07] 创建目录（含多级）
来源：http://er.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mt.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fr.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kg.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pj.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hs.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ah.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ns.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wm.newstarts.cn

[F08] 遍历目录
来源：http://mq.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xz.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://le.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://oe.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://sn.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ie.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ip.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://pj.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://fo.haigaiapp.cn

[F09] 获取文件大小
来源：http://bn.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://bh.colortex.cn

PHP:  filesize("a.txt");
来源：http://jg.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://xv.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://is.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bp.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fp.newstarts.cn

Ruby: File.size("a.txt")
来源：http://zk.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://eu.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ur.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://of.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ya.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ro.szsharing.cn

TS:   path.extname("a.txt")
来源：http://xf.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kr.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ud.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ek.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wc.huanxung.cn

[F11] 复制与移动文件
来源：http://xt.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tc.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ug.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://th.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oc.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hj.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dd.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zd.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hd.huixinmuqiang.cn

[F12] CSV 读写
来源：http://uq.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xu.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bl.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oi.muxihuayi.cn

TS:   // 同上
来源：http://fe.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ww.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uc.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hn.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fe.asd995.cn

================================================================================
来源：http://qj.hahajie.cn

G. 面向对象
来源：http://kt.colortex.cn

================================================================================
来源：http://ej.bjjhwx.cn

[G01] 定义类
来源：http://vz.jianghongdianzi.cn

Py:   class User: pass
来源：http://pa.haigaiapp.cn

PHP:  class User {}
来源：http://rq.bjjhwx.cn

JS:   class User {}
来源：http://nb.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://hi.huixinmuqiang.cn

Java: class User {}
来源：http://qd.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://tx.haigaiapp.cn

Ruby: class User; end
来源：http://vp.huanxung.cn

C#:   class User {}
来源：http://bo.asd995.cn

[G02] 构造函数
来源：http://ty.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://an.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://mm.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://lh.asd995.cn

TS:   constructor(public name: string) {}
来源：http://il.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://yy.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fj.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ln.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://sv.huixinmuqiang.cn

[G03] 实例属性
来源：http://do.bjjhwx.cn

Py:   self.name = "x"
来源：http://tw.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://wy.newstarts.cn

JS:   this.name = "x";
来源：http://ki.nszjky.cn

TS:   name: string = "x";
来源：http://jn.gzmigu.cn

Java: private String name;
来源：http://al.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qo.hnjuh.cn

Ruby: @name = "x"
来源：http://pb.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://wj.szsharing.cn

[G04] 定义方法
来源：http://lw.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://yn.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zw.newstarts.cn

JS:   greet() { return this.name; }
来源：http://uw.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://ox.gzmigu.cn

Java: String greet() { return name; }
来源：http://yl.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xb.szxytkj.cn

Ruby: def greet; @name; end
来源：http://kw.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://jq.nszjky.cn

[G05] 继承
来源：http://wc.shxzukj.cn

Py:   class Admin(User): pass
来源：http://mu.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://uc.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://ml.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://vy.bjjhwx.cn

Java: class Admin extends User {}
来源：http://hy.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eo.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://de.szsharing.cn

C#:   class Admin : User {}
来源：http://eb.huixinmuqiang.cn

[G06] 重写方法
来源：http://qh.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://jj.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zi.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://uj.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://lm.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://tl.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ws.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://pu.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://nu.shtwfgs.cn

[G07] 调用父类方法
来源：http://qf.jianghongdianzi.cn

Py:   super().greet()
来源：http://yv.lnxyls.cn

PHP:  parent::greet();
来源：http://hb.huixinmuqiang.cn

JS:   super.greet();
来源：http://td.yuntaijiaju.cn

TS:   super.greet();
来源：http://vk.muxihuayi.cn

Java: super.greet();
来源：http://eh.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dg.bookmarksfly.cn

Ruby: super
来源：http://sp.asd995.cn

C#:   base.Greet();
来源：http://db.shxzskj.cn

[G08] 静态方法与属性
来源：http://zm.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gr.chemitech.net.cn

PHP:  public static function f() {}
来源：http://fu.lnxyls.cn

JS:   static f() {}
来源：http://px.colortex.cn

TS:   static f(): void {}
来源：http://gl.9csxet.cn

Java: static void f() {}
来源：http://nj.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wk.hnjuh.cn

Ruby: def self.f; end
来源：http://pc.gzmigu.cn

C#:   public static void F() {}
来源：http://pv.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://nd.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://oz.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sq.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wu.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://um.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ox.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://om.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dq.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://ck.lnxyls.cn

[G10] 访问控制
来源：http://wh.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://dq.huanxung.cn

PHP:  public / protected / private
来源：http://zn.asd995.cn

JS:   #private 字段；其余公开
来源：http://og.muxihuayi.cn

TS:   public / protected / private
来源：http://qg.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://rm.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tp.bookmarksfly.cn

Ruby: public / protected / private
来源：http://gx.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://qj.bookmarksfly.cn

[G11] getter / setter
来源：http://wu.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://bz.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jy.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://uw.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://rr.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://va.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ux.nicolike.cn

Ruby: attr_accessor :name
来源：http://ej.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://vf.haigaiapp.cn

[G12] 对象转字符串
来源：http://wh.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://lh.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jg.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://mu.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://sf.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://xp.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zj.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://pb.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://kw.bookmarksfly.cn

[G13] 判断对象类型
来源：http://xj.szxytkj.cn

Py:   isinstance(u, User)
来源：http://wi.haigaiapp.cn

PHP:  $u instanceof User
来源：http://ck.yuntaijiaju.cn

JS:   u instanceof User
来源：http://li.yuntaijiaju.cn

TS:   u instanceof User
来源：http://jn.jctech888.com.cn

Java: u instanceof User
来源：http://bw.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ig.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://by.szsharing.cn

C#:   u is User
来源：http://lv.newstarts.cn

[G14] 数据类 / record
来源：http://hz.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://go.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://bw.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jt.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://rn.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://ii.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://er.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gf.asd995.cn

C#:   record User(string Name, int Age);
来源：http://cz.haigaiapp.cn

[G15] 枚举
来源：http://fe.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mb.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yk.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tf.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xl.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://ov.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mt.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://uq.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mf.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://mj.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mj.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://sv.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://be.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://lq.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pv.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dg.shxzskj.cn

Ruby: obj.instance_variables
来源：http://dq.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ux.nszjky.cn

================================================================================
来源：http://hd.nszjky.cn

H. 异常与错误处理
来源：http://ta.shxzskj.cn

================================================================================
来源：http://ci.panjiajie.cn

[H01] try / catch 基础
来源：http://tn.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lq.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ro.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://on.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pe.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rz.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zk.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bp.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ab.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://bn.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pt.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ch.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fg.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gx.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://za.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mb.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://im.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qg.shxzukj.cn

[H03] 主动抛出异常
来源：http://ay.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://cu.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wm.asd995.cn

JS:   throw new Error("错误信息");
来源：http://fs.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://om.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kc.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gm.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xs.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://la.nszjky.cn

[H04] 自定义异常类型
来源：http://mj.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://hr.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://re.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ty.nszjky.cn

TS:   class MyError extends Error {}
来源：http://ot.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://nr.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ij.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://dj.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://nb.yuexingan06.cn

[H05] 捕获特定类型
来源：http://tz.shxzukj.cn

Py:   except ValueError as e:
来源：http://gz.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nt.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://yp.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://zo.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://nz.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gg.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://uh.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ui.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://wp.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://lk.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://er.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://en.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ez.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ge.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://km.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://cs.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://gj.hahajie.cn

[H07] 断言
来源：http://tp.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://yu.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://vv.szsharing.cn

JS:   console.assert(x > 0);
来源：http://fl.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://gd.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://zj.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hb.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sd.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://bj.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://eq.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://py.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wr.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://sd.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uq.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ar.wgjwhj.cn

Go:   err.Error()
来源：http://ga.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://bb.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://ms.nszjky.cn

[H09] 带错误码的异常
来源：http://lh.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hs.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dg.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mn.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dt.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gs.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pi.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rk.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qm.lnxyls.cn

[H10] 资源自动释放
来源：http://kx.521024.cn


<!-- 参考信息 -->