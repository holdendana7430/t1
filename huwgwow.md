代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lw.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://le.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dh.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kj.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jf.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gj.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ks.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fz.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://tc.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iu.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://yw.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://xy.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wk.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://os.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ab.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://sm.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://da.panjiajie.cn

[F06] 删除文件
来源：http://gj.hahajie.cn

Py:   os.remove("a.txt")
来源：http://pk.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ck.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qx.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dt.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qy.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://gw.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://od.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://js.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://fp.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gh.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qd.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gs.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dw.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cq.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oi.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ow.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aa.asd995.cn

[F08] 遍历目录
来源：http://sk.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yv.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zt.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://au.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://uu.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xh.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ky.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://wy.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://kw.asd995.cn

[F09] 获取文件大小
来源：http://ej.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://ve.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://qw.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://dg.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://hq.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dd.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ap.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://ig.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://xl.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wz.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nz.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wk.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iq.colortex.cn

TS:   path.extname("a.txt")
来源：http://tn.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bl.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ce.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://os.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jo.colortex.cn

[F11] 复制与移动文件
来源：http://hz.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bf.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rc.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ih.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nl.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hq.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fb.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ab.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ra.shxzukj.cn

[F12] CSV 读写
来源：http://ia.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ja.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jq.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zm.wgjwhj.cn

TS:   // 同上
来源：http://sg.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tn.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bq.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://px.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dd.panjiajie.cn

================================================================================
来源：http://mu.shxzskj.cn

G. 面向对象
来源：http://on.shxzukj.cn

================================================================================
来源：http://oq.szxytkj.cn

[G01] 定义类
来源：http://sv.colortex.cn

Py:   class User: pass
来源：http://vg.newstarts.cn

PHP:  class User {}
来源：http://im.szsharing.cn

JS:   class User {}
来源：http://di.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://bw.newstarts.cn

Java: class User {}
来源：http://ac.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://fe.huixinmuqiang.cn

Ruby: class User; end
来源：http://td.hahajie.cn

C#:   class User {}
来源：http://mz.shxzskj.cn

[G02] 构造函数
来源：http://od.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://zc.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://xs.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://zm.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://jo.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://ez.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://of.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://po.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://eg.521024.cn

[G03] 实例属性
来源：http://zy.bookmarksfly.cn

Py:   self.name = "x"
来源：http://pt.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://oz.bookmarksfly.cn

JS:   this.name = "x";
来源：http://ih.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://dj.yuntaijiaju.cn

Java: private String name;
来源：http://xk.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yj.bjjhwx.cn

Ruby: @name = "x"
来源：http://cc.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ze.lnxyls.cn

[G04] 定义方法
来源：http://hw.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://ph.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ky.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://vr.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://yj.hahajie.cn

Java: String greet() { return name; }
来源：http://cw.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://va.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://ev.9csxet.cn

C#:   public string Greet() => Name;
来源：http://jw.panjiajie.cn

[G05] 继承
来源：http://ng.shxzskj.cn

Py:   class Admin(User): pass
来源：http://uk.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://gn.huanxung.cn

JS:   class Admin extends User {}
来源：http://kl.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://og.hnjuh.cn

Java: class Admin extends User {}
来源：http://dr.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fa.lnxyls.cn

Ruby: class Admin < User; end
来源：http://gl.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ls.521024.cn

[G06] 重写方法
来源：http://ob.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ei.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ss.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://pg.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://cw.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://zo.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://or.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://xo.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://tj.bookmarksfly.cn

[G07] 调用父类方法
来源：http://mi.huanxung.cn

Py:   super().greet()
来源：http://qn.haigaiapp.cn

PHP:  parent::greet();
来源：http://rr.huanxung.cn

JS:   super.greet();
来源：http://se.nicolike.cn

TS:   super.greet();
来源：http://hs.huanxung.cn

Java: super.greet();
来源：http://fw.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://se.jianghongdianzi.cn

Ruby: super
来源：http://ej.9csxet.cn

C#:   base.Greet();
来源：http://dz.colortex.cn

[G08] 静态方法与属性
来源：http://an.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jr.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://ag.bjjhwx.cn

JS:   static f() {}
来源：http://ey.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://kg.muxihuayi.cn

Java: static void f() {}
来源：http://by.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dj.chemitech.net.cn

Ruby: def self.f; end
来源：http://we.chemitech.net.cn

C#:   public static void F() {}
来源：http://jp.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://qv.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://zp.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uz.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vj.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://zb.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://aa.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://vf.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xa.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://ys.haigaiapp.cn

[G10] 访问控制
来源：http://dg.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://as.jctech888.com.cn

PHP:  public / protected / private
来源：http://vd.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://hr.lnxyls.cn

TS:   public / protected / private
来源：http://wk.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://zw.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ns.panjiajie.cn

Ruby: public / protected / private
来源：http://pr.newstarts.cn

C#:   public / protected / private / internal
来源：http://sk.9csxet.cn

[G11] getter / setter
来源：http://co.nszjky.cn

Py:   @property 与 @x.setter
来源：http://er.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://or.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://qz.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://si.lnxyls.cn

Java: public String getName() { return name; }
来源：http://kt.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pc.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://vf.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://au.bjjhwx.cn

[G12] 对象转字符串
来源：http://sa.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://hj.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vi.newstarts.cn

JS:   toString() { return this.name; }
来源：http://nl.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://rq.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://ri.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nn.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://gu.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://qu.9csxet.cn

[G13] 判断对象类型
来源：http://zq.9csxet.cn

Py:   isinstance(u, User)
来源：http://nw.jctech888.com.cn

PHP:  $u instanceof User
来源：http://sf.hahajie.cn

JS:   u instanceof User
来源：http://ah.asd995.cn

TS:   u instanceof User
来源：http://ul.huixinmuqiang.cn

Java: u instanceof User
来源：http://fr.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uf.colortex.cn

Ruby: u.is_a?(User)
来源：http://ng.gzmigu.cn

C#:   u is User
来源：http://zn.lnxyls.cn

[G14] 数据类 / record
来源：http://hg.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ph.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://dt.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zo.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://nz.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://st.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://io.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://au.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://mk.huixinmuqiang.cn

[G15] 枚举
来源：http://fk.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vk.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xt.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wk.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pb.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ui.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pb.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://gi.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pp.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ho.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cl.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ww.gzmigu.cn

JS:   Object.entries(obj)
来源：http://fh.asd995.cn

TS:   Object.entries(obj)
来源：http://bz.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cn.colortex.cn

Ruby: obj.instance_variables
来源：http://fj.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://jf.9csxet.cn

================================================================================
来源：http://kl.nicolike.cn

H. 异常与错误处理
来源：http://pj.huixiangedu.cn

================================================================================
来源：http://mh.521024.cn

[H01] try / catch 基础
来源：http://ks.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tq.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hr.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kb.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://me.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kh.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zs.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://be.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ol.newstarts.cn

[H02] finally / ensure 收尾
来源：http://pk.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xy.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mz.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xe.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fc.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kg.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rg.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cq.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xw.shxzskj.cn

[H03] 主动抛出异常
来源：http://hn.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://ev.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://du.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://br.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://bh.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vx.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lr.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yy.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qr.gzmigu.cn

[H04] 自定义异常类型
来源：http://bi.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://ap.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tl.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://pe.colortex.cn

TS:   class MyError extends Error {}
来源：http://hk.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://xk.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://id.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://fa.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://ni.colortex.cn

[H05] 捕获特定类型
来源：http://pr.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ut.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kr.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://up.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://ib.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://us.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lx.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://kp.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sg.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://nv.colortex.cn

Py:   value = d.get("k") or default
来源：http://fp.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pz.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qo.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sb.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nn.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pu.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://be.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://uw.huixinmuqiang.cn

[H07] 断言
来源：http://hg.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://fu.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://am.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://pf.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://yh.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://rl.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://az.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cl.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://dm.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://xq.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://ue.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gc.lnxyls.cn

JS:   e.message;  e.stack
来源：http://yi.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://um.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mf.yuntaijiaju.cn

Go:   err.Error()
来源：http://bd.colortex.cn


<!-- 参考信息 -->