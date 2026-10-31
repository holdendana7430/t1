代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://up.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://xl.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nt.huanxung.cn

[F04] 追加写入文件
来源：http://xw.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ar.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://go.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sf.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://na.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://za.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ix.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ls.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jn.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://vx.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://je.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://mg.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://zi.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://sj.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vq.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ap.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://qt.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://we.nszjky.cn

[F06] 删除文件
来源：http://bs.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://ga.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://yh.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rw.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vl.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fu.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://ph.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://mf.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://qs.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://kk.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jh.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qu.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bw.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xi.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://re.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xz.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yi.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gy.hahajie.cn

[F08] 遍历目录
来源：http://cm.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ff.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://do.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://tc.521024.cn

TS:   fs.readdirSync("dir")
来源：http://lw.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lr.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kt.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://xq.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://hu.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://wy.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://pj.9csxet.cn

PHP:  filesize("a.txt");
来源：http://mn.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://dl.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://jo.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://in.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cw.newstarts.cn

Ruby: File.size("a.txt")
来源：http://cq.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://pj.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://on.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rl.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jh.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mi.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://rd.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yp.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ri.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bv.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ki.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://sz.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ta.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tj.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vr.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jw.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://se.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://op.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zo.chemitech.net.cn

[F12] CSV 读写
来源：http://fx.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mf.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pj.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yp.521024.cn

TS:   // 同上
来源：http://mf.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wh.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wr.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sz.jianghongdianzi.cn

================================================================================
来源：http://xt.nszjky.cn

G. 面向对象
来源：http://pd.panjiajie.cn

================================================================================
来源：http://qb.521024.cn

[G01] 定义类
来源：http://on.bookmarksfly.cn

Py:   class User: pass
来源：http://kh.shtwfgs.cn

PHP:  class User {}
来源：http://lj.szsharing.cn

JS:   class User {}
来源：http://ty.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://vq.nszjky.cn

Java: class User {}
来源：http://hj.521024.cn

Go:   type User struct { Name string }
来源：http://sn.gzmigu.cn

Ruby: class User; end
来源：http://bq.bjjhwx.cn

C#:   class User {}
来源：http://mb.colortex.cn

[G02] 构造函数
来源：http://ku.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://zk.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://sz.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ns.colortex.cn

TS:   constructor(public name: string) {}
来源：http://sp.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://ux.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wh.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://od.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://yp.panjiajie.cn

[G03] 实例属性
来源：http://ei.newstarts.cn

Py:   self.name = "x"
来源：http://dm.lnxyls.cn

PHP:  public string $name = "x";
来源：http://ze.shxzskj.cn

JS:   this.name = "x";
来源：http://vj.hnjuh.cn

TS:   name: string = "x";
来源：http://nw.lnxyls.cn

Java: private String name;
来源：http://ys.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jm.bjjhwx.cn

Ruby: @name = "x"
来源：http://bm.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://sc.huixiangedu.cn

[G04] 定义方法
来源：http://js.newstarts.cn

Py:   def greet(self): return self.name
来源：http://vp.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wm.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://co.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://nu.szxytkj.cn

Java: String greet() { return name; }
来源：http://oq.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iw.szxytkj.cn

Ruby: def greet; @name; end
来源：http://sv.asd995.cn

C#:   public string Greet() => Name;
来源：http://dd.newstarts.cn

[G05] 继承
来源：http://co.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://ti.huanxung.cn

PHP:  class Admin extends User {}
来源：http://iw.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://mj.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://jv.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://rn.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dk.asd995.cn

Ruby: class Admin < User; end
来源：http://ju.asd995.cn

C#:   class Admin : User {}
来源：http://as.jctech888.com.cn

[G06] 重写方法
来源：http://sj.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://nv.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uj.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://sf.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://jl.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ay.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xm.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://bc.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://ko.szxytkj.cn

[G07] 调用父类方法
来源：http://tp.asd995.cn

Py:   super().greet()
来源：http://hm.colortex.cn

PHP:  parent::greet();
来源：http://zy.chemitech.net.cn

JS:   super.greet();
来源：http://fn.jctech888.com.cn

TS:   super.greet();
来源：http://dn.shxzskj.cn

Java: super.greet();
来源：http://gh.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zp.hnjuh.cn

Ruby: super
来源：http://fu.panjiajie.cn

C#:   base.Greet();
来源：http://mb.newstarts.cn

[G08] 静态方法与属性
来源：http://mf.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oi.bjjhwx.cn

PHP:  public static function f() {}
来源：http://ip.huanxung.cn

JS:   static f() {}
来源：http://qv.asd995.cn

TS:   static f(): void {}
来源：http://tx.huanxung.cn

Java: static void f() {}
来源：http://vw.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rl.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://jw.hahajie.cn

C#:   public static void F() {}
来源：http://gx.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://sj.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://jh.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zp.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iq.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://xn.nszjky.cn

Java: interface Shape { double area(); }
来源：http://tj.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://zi.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uf.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://qh.szsharing.cn

[G10] 访问控制
来源：http://gt.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://da.shxzukj.cn

PHP:  public / protected / private
来源：http://jj.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ju.bjjhwx.cn

TS:   public / protected / private
来源：http://xq.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://jz.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hi.jctech888.com.cn

Ruby: public / protected / private
来源：http://mv.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://sf.colortex.cn

[G11] getter / setter
来源：http://vf.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://ie.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ti.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://dl.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://vw.panjiajie.cn

Java: public String getName() { return name; }
来源：http://kf.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vc.hahajie.cn

Ruby: attr_accessor :name
来源：http://ag.nszjky.cn

C#:   public string Name { get; set; }
来源：http://kv.chemitech.net.cn

[G12] 对象转字符串
来源：http://do.521024.cn

Py:   def __str__(self): return self.name
来源：http://kh.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aw.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://sj.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://rt.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://vq.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jj.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://fl.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://ph.szxytkj.cn

[G13] 判断对象类型
来源：http://cw.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://zv.huixiangedu.cn

PHP:  $u instanceof User
来源：http://hq.panjiajie.cn

JS:   u instanceof User
来源：http://qv.colortex.cn

TS:   u instanceof User
来源：http://ou.chemitech.net.cn

Java: u instanceof User
来源：http://om.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kp.colortex.cn

Ruby: u.is_a?(User)
来源：http://cj.bjjhwx.cn

C#:   u is User
来源：http://mq.haigaiapp.cn

[G14] 数据类 / record
来源：http://qp.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ud.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://av.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fe.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://vc.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://rk.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://yc.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qb.colortex.cn

C#:   record User(string Name, int Age);
来源：http://ml.hnjuh.cn

[G15] 枚举
来源：http://ca.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rr.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rv.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gq.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aa.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://ql.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://it.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://iw.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xs.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://pp.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kc.asd995.cn

PHP:  get_object_vars($obj);
来源：http://dn.lnxyls.cn

JS:   Object.entries(obj)
来源：http://tz.shxzukj.cn

TS:   Object.entries(obj)
来源：http://zw.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cv.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mg.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://je.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://my.nszjky.cn

================================================================================
来源：http://jb.shxzskj.cn

H. 异常与错误处理
来源：http://ol.shtwfgs.cn

================================================================================
来源：http://qs.huanxung.cn

[H01] try / catch 基础
来源：http://gs.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://va.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mu.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vg.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yn.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lj.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hl.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cr.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lk.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vn.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hi.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ab.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qb.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hy.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ja.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kb.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ik.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jl.hahajie.cn

[H03] 主动抛出异常
来源：http://bf.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://cm.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nx.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://bi.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://to.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dh.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tk.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://au.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xs.bjjhwx.cn

[H04] 自定义异常类型
来源：http://jp.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://vu.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aw.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://kh.nszjky.cn

TS:   class MyError extends Error {}
来源：http://rt.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://gt.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yt.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://ne.521024.cn

C#:   class MyException : Exception {}
来源：http://gl.bjjhwx.cn

[H05] 捕获特定类型
来源：http://vr.shxzskj.cn

Py:   except ValueError as e:
来源：http://bw.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sw.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://qc.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://xu.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://vp.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rx.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://bo.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://az.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://yc.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://de.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://po.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kf.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hr.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nn.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ty.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://tr.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://sl.nicolike.cn

[H07] 断言
来源：http://iq.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://mi.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://cf.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://wm.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://aa.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://eq.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vo.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hv.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://me.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://qu.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://se.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yo.gzmigu.cn


<!-- 参考信息 -->