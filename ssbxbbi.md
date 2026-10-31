代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://cd.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://do.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://of.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://pp.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://uf.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://an.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tn.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://dj.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://pb.gzmigu.cn

[F06] 删除文件
来源：http://hb.asd995.cn

Py:   os.remove("a.txt")
来源：http://te.szsharing.cn

PHP:  unlink("a.txt");
来源：http://hp.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yl.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sk.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jo.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ml.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://hz.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://xm.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ek.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ge.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mc.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://an.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lu.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gv.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pw.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qf.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vp.lnxyls.cn

[F08] 遍历目录
来源：http://eh.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ht.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ci.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://vk.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ob.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gg.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ow.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://iu.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://kl.huanxung.cn

[F09] 获取文件大小
来源：http://fa.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://hh.huanxung.cn

PHP:  filesize("a.txt");
来源：http://sy.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://yi.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://on.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ek.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ml.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://rb.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://vd.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://yh.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zo.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vi.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uw.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://hb.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ic.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dk.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zt.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xs.panjiajie.cn

[F11] 复制与移动文件
来源：http://zb.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zb.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://va.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kx.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ax.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rr.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xd.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cm.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uz.gzmigu.cn

[F12] CSV 读写
来源：http://oo.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ph.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://up.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yy.shxzukj.cn

TS:   // 同上
来源：http://yv.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cn.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pi.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xe.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ar.nszjky.cn

================================================================================
来源：http://tw.huixinmuqiang.cn

G. 面向对象
来源：http://qu.hnjuh.cn

================================================================================
来源：http://ay.bjjhwx.cn

[G01] 定义类
来源：http://wv.chemitech.net.cn

Py:   class User: pass
来源：http://wx.yuexingan06.cn

PHP:  class User {}
来源：http://cf.bjjhwx.cn

JS:   class User {}
来源：http://ga.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://ei.szxytkj.cn

Java: class User {}
来源：http://zz.colortex.cn

Go:   type User struct { Name string }
来源：http://ug.shtwfgs.cn

Ruby: class User; end
来源：http://mg.szxytkj.cn

C#:   class User {}
来源：http://hx.hahajie.cn

[G02] 构造函数
来源：http://ok.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wg.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://od.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://pb.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://az.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ui.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aq.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ie.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://vl.szxytkj.cn

[G03] 实例属性
来源：http://lw.nszjky.cn

Py:   self.name = "x"
来源：http://th.colortex.cn

PHP:  public string $name = "x";
来源：http://vo.521024.cn

JS:   this.name = "x";
来源：http://pu.nicolike.cn

TS:   name: string = "x";
来源：http://gv.huixinmuqiang.cn

Java: private String name;
来源：http://zd.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gb.shxzukj.cn

Ruby: @name = "x"
来源：http://kf.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.chemitech.net.cn

[G04] 定义方法
来源：http://xb.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://cc.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hj.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://bg.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://gh.huixiangedu.cn

Java: String greet() { return name; }
来源：http://kg.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fg.nszjky.cn

Ruby: def greet; @name; end
来源：http://qa.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://du.szxytkj.cn

[G05] 继承
来源：http://bj.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://fc.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://dk.nicolike.cn

JS:   class Admin extends User {}
来源：http://xz.9csxet.cn

TS:   class Admin extends User {}
来源：http://km.gzmigu.cn

Java: class Admin extends User {}
来源：http://vb.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lc.hnjuh.cn

Ruby: class Admin < User; end
来源：http://ma.szsharing.cn

C#:   class Admin : User {}
来源：http://zz.nszjky.cn

[G06] 重写方法
来源：http://yk.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://jz.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://np.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://tf.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://zl.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://os.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oa.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://el.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://oi.nszjky.cn

[G07] 调用父类方法
来源：http://pi.nicolike.cn

Py:   super().greet()
来源：http://cz.colortex.cn

PHP:  parent::greet();
来源：http://av.jctech888.com.cn

JS:   super.greet();
来源：http://sz.nicolike.cn

TS:   super.greet();
来源：http://xk.huanxung.cn

Java: super.greet();
来源：http://al.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ua.asd995.cn

Ruby: super
来源：http://fn.hahajie.cn

C#:   base.Greet();
来源：http://cd.hahajie.cn

[G08] 静态方法与属性
来源：http://od.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zk.jctech888.com.cn

PHP:  public static function f() {}
来源：http://lq.521024.cn

JS:   static f() {}
来源：http://cf.nszjky.cn

TS:   static f(): void {}
来源：http://te.yuntaijiaju.cn

Java: static void f() {}
来源：http://ge.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vz.szxytkj.cn

Ruby: def self.f; end
来源：http://bq.yuexingan06.cn

C#:   public static void F() {}
来源：http://ol.newstarts.cn

[G09] 接口 / 抽象类
来源：http://yh.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://dt.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lg.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qj.521024.cn

TS:   interface Shape { area(): number; }
来源：http://gz.nicolike.cn

Java: interface Shape { double area(); }
来源：http://au.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://cs.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://di.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ej.shxzskj.cn

[G10] 访问控制
来源：http://dp.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ya.huixiangedu.cn

PHP:  public / protected / private
来源：http://fb.huanxung.cn

JS:   #private 字段；其余公开
来源：http://mu.chemitech.net.cn

TS:   public / protected / private
来源：http://ak.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://zj.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wc.hahajie.cn

Ruby: public / protected / private
来源：http://hc.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://qc.9csxet.cn

[G11] getter / setter
来源：http://nf.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://nw.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iu.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://nu.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://mm.gzmigu.cn

Java: public String getName() { return name; }
来源：http://jy.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gc.szsharing.cn

Ruby: attr_accessor :name
来源：http://mx.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://qk.panjiajie.cn

[G12] 对象转字符串
来源：http://je.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ge.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ah.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://di.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://qp.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://sn.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ir.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://lr.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://qn.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://mf.521024.cn

Py:   isinstance(u, User)
来源：http://gf.hahajie.cn

PHP:  $u instanceof User
来源：http://wa.nicolike.cn

JS:   u instanceof User
来源：http://zv.nszjky.cn

TS:   u instanceof User
来源：http://uq.lnxyls.cn

Java: u instanceof User
来源：http://fx.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cg.nszjky.cn

Ruby: u.is_a?(User)
来源：http://xc.huixinmuqiang.cn

C#:   u is User
来源：http://xn.hnjuh.cn

[G14] 数据类 / record
来源：http://dt.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rk.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://de.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vv.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://ok.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://md.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://xx.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rz.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://iu.panjiajie.cn

[G15] 枚举
来源：http://sj.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zi.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mp.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iv.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mt.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://kv.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pw.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://ll.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bm.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://nm.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kh.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://fq.lnxyls.cn

JS:   Object.entries(obj)
来源：http://tf.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://jg.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wb.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rz.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://jq.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ut.bjjhwx.cn

================================================================================
来源：http://sr.newstarts.cn

H. 异常与错误处理
来源：http://yz.huixinmuqiang.cn

================================================================================
来源：http://ns.wgjwhj.cn

[H01] try / catch 基础
来源：http://lo.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tc.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lz.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://no.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ay.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sp.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://za.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gz.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ol.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://dg.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rq.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wd.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cv.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iy.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vx.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mo.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nq.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uw.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://oi.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://kc.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ts.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://an.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://qv.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://om.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xh.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vz.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sz.huixiangedu.cn

[H04] 自定义异常类型
来源：http://hn.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://by.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://om.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://xd.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://yx.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://os.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iz.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://rd.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://uq.gzmigu.cn

[H05] 捕获特定类型
来源：http://ts.huanxung.cn

Py:   except ValueError as e:
来源：http://jb.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ll.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ps.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://hn.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://jz.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pu.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://oh.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eh.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://bp.colortex.cn

Py:   value = d.get("k") or default
来源：http://gw.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fl.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gl.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://di.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kv.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jv.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://dr.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://im.chemitech.net.cn

[H07] 断言
来源：http://lu.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://qb.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ho.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://nj.szsharing.cn

TS:   console.assert(x > 0);
来源：http://yg.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://rh.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cw.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mr.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://yg.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://fv.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://nm.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kg.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://ks.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qg.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zx.wgjwhj.cn

Go:   err.Error()
来源：http://sm.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://uj.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://qb.szxytkj.cn

[H09] 带错误码的异常
来源：http://cx.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ye.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nk.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aj.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vg.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xa.wgjwhj.cn


<!-- 参考信息 -->