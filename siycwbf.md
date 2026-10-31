代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ls.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://zv.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oo.huanxung.cn

[F04] 追加写入文件
来源：http://us.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tn.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lx.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qj.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xt.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vb.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://co.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ou.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://js.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://ud.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ge.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://oi.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://de.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://wc.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ct.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xq.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://sw.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ym.newstarts.cn

[F06] 删除文件
来源：http://wy.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ei.9csxet.cn

PHP:  unlink("a.txt");
来源：http://uf.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ja.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kd.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hg.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://ub.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ln.colortex.cn

C#:   File.Delete("a.txt");
来源：http://vo.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://si.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eo.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fz.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ix.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vu.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fe.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sq.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vd.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tx.nicolike.cn

[F08] 遍历目录
来源：http://yl.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rg.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uh.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://oz.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://lg.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hp.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cw.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://ly.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://yi.gzmigu.cn

[F09] 获取文件大小
来源：http://ii.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://pl.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://sq.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://fd.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://yd.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gy.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gc.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://mn.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://zj.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zz.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oq.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zl.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nl.huanxung.cn

TS:   path.extname("a.txt")
来源：http://je.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cp.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pp.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://io.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nw.shxzskj.cn

[F11] 复制与移动文件
来源：http://zp.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lv.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ol.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cj.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://le.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ny.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://is.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bd.huanxung.cn

[F12] CSV 读写
来源：http://ae.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xc.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dc.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://md.muxihuayi.cn

TS:   // 同上
来源：http://zm.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jy.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ua.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lm.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ph.yuntaijiaju.cn

================================================================================
来源：http://pj.9csxet.cn

G. 面向对象
来源：http://ez.jctech888.com.cn

================================================================================
来源：http://ze.gzmigu.cn

[G01] 定义类
来源：http://qy.shxzukj.cn

Py:   class User: pass
来源：http://bu.asd995.cn

PHP:  class User {}
来源：http://ap.huanxung.cn

JS:   class User {}
来源：http://az.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://sz.gzmigu.cn

Java: class User {}
来源：http://vn.9csxet.cn

Go:   type User struct { Name string }
来源：http://hh.asd995.cn

Ruby: class User; end
来源：http://vq.chemitech.net.cn

C#:   class User {}
来源：http://dm.shxzukj.cn

[G02] 构造函数
来源：http://mc.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://lc.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://gh.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://mj.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://kc.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://sv.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cu.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://yw.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://vc.nicolike.cn

[G03] 实例属性
来源：http://wd.chemitech.net.cn

Py:   self.name = "x"
来源：http://yl.hahajie.cn

PHP:  public string $name = "x";
来源：http://fz.gzmigu.cn

JS:   this.name = "x";
来源：http://xc.asd995.cn

TS:   name: string = "x";
来源：http://dl.muxihuayi.cn

Java: private String name;
来源：http://sp.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cz.szsharing.cn

Ruby: @name = "x"
来源：http://uh.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://zm.panjiajie.cn

[G04] 定义方法
来源：http://bi.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://qf.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ak.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://nv.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://nf.521024.cn

Java: String greet() { return name; }
来源：http://hr.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eo.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://qz.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://tc.hnjuh.cn

[G05] 继承
来源：http://yf.lnxyls.cn

Py:   class Admin(User): pass
来源：http://lu.newstarts.cn

PHP:  class Admin extends User {}
来源：http://ve.newstarts.cn

JS:   class Admin extends User {}
来源：http://hr.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://pz.gzmigu.cn

Java: class Admin extends User {}
来源：http://yu.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sl.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ml.huanxung.cn

C#:   class Admin : User {}
来源：http://ke.colortex.cn

[G06] 重写方法
来源：http://at.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://pi.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hm.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://az.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://cc.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://zi.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bi.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://st.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://np.nicolike.cn

[G07] 调用父类方法
来源：http://iv.chemitech.net.cn

Py:   super().greet()
来源：http://cm.bjjhwx.cn

PHP:  parent::greet();
来源：http://zp.yuexingan06.cn

JS:   super.greet();
来源：http://ua.szsharing.cn

TS:   super.greet();
来源：http://sh.chemitech.net.cn

Java: super.greet();
来源：http://pn.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://om.asd995.cn

Ruby: super
来源：http://in.lnxyls.cn

C#:   base.Greet();
来源：http://tf.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://ix.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jv.shxzukj.cn

PHP:  public static function f() {}
来源：http://uh.shtwfgs.cn

JS:   static f() {}
来源：http://an.newstarts.cn

TS:   static f(): void {}
来源：http://ur.yuntaijiaju.cn

Java: static void f() {}
来源：http://ai.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fk.jctech888.com.cn

Ruby: def self.f; end
来源：http://rc.haigaiapp.cn

C#:   public static void F() {}
来源：http://cf.asd995.cn

[G09] 接口 / 抽象类
来源：http://af.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://ur.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nh.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yz.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://ca.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://hg.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://qb.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qo.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ci.gzmigu.cn

[G10] 访问控制
来源：http://kf.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ky.jctech888.com.cn

PHP:  public / protected / private
来源：http://md.newstarts.cn

JS:   #private 字段；其余公开
来源：http://ts.szsharing.cn

TS:   public / protected / private
来源：http://ev.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://ec.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tl.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://jb.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://pn.521024.cn

[G11] getter / setter
来源：http://dm.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://ml.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tl.nicolike.cn

JS:   get name() { return this._name; }
来源：http://xv.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://et.szxytkj.cn

Java: public String getName() { return name; }
来源：http://rp.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jj.szxytkj.cn

Ruby: attr_accessor :name
来源：http://fk.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://yi.colortex.cn

[G12] 对象转字符串
来源：http://ym.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://kq.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pn.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://uh.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://dn.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ko.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zp.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://dw.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://uj.521024.cn

[G13] 判断对象类型
来源：http://nn.shxzskj.cn

Py:   isinstance(u, User)
来源：http://hd.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://gy.shxzskj.cn

JS:   u instanceof User
来源：http://rp.szxytkj.cn

TS:   u instanceof User
来源：http://hm.szsharing.cn

Java: u instanceof User
来源：http://ic.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sw.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://zm.panjiajie.cn

C#:   u is User
来源：http://te.wgjwhj.cn

[G14] 数据类 / record
来源：http://og.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gr.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://no.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ji.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://fm.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://jc.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://di.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wu.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://mw.521024.cn

[G15] 枚举
来源：http://ms.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gj.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sc.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://em.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lg.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://jd.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ku.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://ir.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uh.asd995.cn

[G16] 对象转数组 / 字典
来源：http://cq.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xy.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://aw.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://fa.521024.cn

TS:   Object.entries(obj)
来源：http://kq.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zb.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xc.colortex.cn

Ruby: obj.instance_variables
来源：http://lb.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://xe.panjiajie.cn

================================================================================
来源：http://us.yuexingan06.cn

H. 异常与错误处理
来源：http://oa.yuexingan06.cn

================================================================================
来源：http://uq.hahajie.cn

[H01] try / catch 基础
来源：http://tg.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ht.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cg.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qt.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://py.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jz.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tr.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jg.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uw.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ev.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sf.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kn.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kh.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vu.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cg.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dg.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kr.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cb.newstarts.cn

[H03] 主动抛出异常
来源：http://af.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://zj.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uw.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://rl.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://zw.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bf.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xz.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fn.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ln.panjiajie.cn

[H04] 自定义异常类型
来源：http://ah.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://sc.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rd.nszjky.cn

JS:   class MyError extends Error {}
来源：http://gv.9csxet.cn

TS:   class MyError extends Error {}
来源：http://fg.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://km.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hl.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://vc.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://jt.gzmigu.cn

[H05] 捕获特定类型
来源：http://bb.shxzukj.cn

Py:   except ValueError as e:
来源：http://vz.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dr.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://ok.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://cm.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://cn.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tz.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://jr.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yg.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://sp.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://pv.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ep.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hu.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gn.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zz.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nb.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://mj.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://sf.szxytkj.cn

[H07] 断言
来源：http://lw.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ki.newstarts.cn

PHP:  assert($x > 0);
来源：http://ca.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://ic.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://hw.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://od.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gl.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vx.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://sr.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://vc.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://dj.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xc.yuntaijiaju.cn


<!-- 参考信息 -->