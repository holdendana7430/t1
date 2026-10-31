代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://tc.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.colortex.cn

PHP:  file_exists("a.txt");
来源：http://zg.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://hm.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://pw.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uh.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pq.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://qu.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://ct.bjjhwx.cn

[F06] 删除文件
来源：http://oh.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://lx.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://ps.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ha.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fh.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ln.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://jy.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://kh.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://gb.nicolike.cn

[F07] 创建目录（含多级）
来源：http://mw.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bv.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ca.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ir.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://td.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://om.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vo.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ro.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lc.nicolike.cn

[F08] 遍历目录
来源：http://rc.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uj.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pd.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://tg.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://rx.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pf.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ga.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://wh.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://ye.chemitech.net.cn

[F09] 获取文件大小
来源：http://pl.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://rp.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://cg.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://up.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://jq.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yx.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nc.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://we.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://wv.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://wx.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nk.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zb.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hh.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://rv.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nv.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://co.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rh.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://id.yuexingan06.cn

[F11] 复制与移动文件
来源：http://hf.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dv.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://li.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cd.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fs.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://di.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ts.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ta.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://up.nicolike.cn

[F12] CSV 读写
来源：http://rl.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vz.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vl.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://of.bookmarksfly.cn

TS:   // 同上
来源：http://ui.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tz.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hg.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gc.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rk.gzmigu.cn

================================================================================
来源：http://ed.szxytkj.cn

G. 面向对象
来源：http://wv.szsharing.cn

================================================================================
来源：http://ep.521024.cn

[G01] 定义类
来源：http://ce.yuntaijiaju.cn

Py:   class User: pass
来源：http://dz.chemitech.net.cn

PHP:  class User {}
来源：http://uc.shtwfgs.cn

JS:   class User {}
来源：http://hv.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://hv.yuexingan06.cn

Java: class User {}
来源：http://sa.huanxung.cn

Go:   type User struct { Name string }
来源：http://oo.gzmigu.cn

Ruby: class User; end
来源：http://yg.shxzskj.cn

C#:   class User {}
来源：http://fp.bookmarksfly.cn

[G02] 构造函数
来源：http://re.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://rn.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://py.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ee.521024.cn

TS:   constructor(public name: string) {}
来源：http://ao.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ks.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hx.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://wf.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://wu.nicolike.cn

[G03] 实例属性
来源：http://sl.shtwfgs.cn

Py:   self.name = "x"
来源：http://uy.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://sp.muxihuayi.cn

JS:   this.name = "x";
来源：http://gz.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://ej.newstarts.cn

Java: private String name;
来源：http://ki.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://op.bookmarksfly.cn

Ruby: @name = "x"
来源：http://lc.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://kv.szsharing.cn

[G04] 定义方法
来源：http://gd.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://ch.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qt.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://ba.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://fx.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://td.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oh.hnjuh.cn

Ruby: def greet; @name; end
来源：http://dw.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://hl.bjjhwx.cn

[G05] 继承
来源：http://vv.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://zt.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://mo.shxzukj.cn

JS:   class Admin extends User {}
来源：http://aa.panjiajie.cn

TS:   class Admin extends User {}
来源：http://oa.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://lp.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fv.gzmigu.cn

Ruby: class Admin < User; end
来源：http://nd.nicolike.cn

C#:   class Admin : User {}
来源：http://yl.9csxet.cn

[G06] 重写方法
来源：http://db.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://vl.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nu.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://rq.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://ki.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://ko.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yj.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://ci.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://eh.shxzukj.cn

[G07] 调用父类方法
来源：http://pk.hnjuh.cn

Py:   super().greet()
来源：http://qu.shtwfgs.cn

PHP:  parent::greet();
来源：http://du.haigaiapp.cn

JS:   super.greet();
来源：http://mk.szsharing.cn

TS:   super.greet();
来源：http://yz.521024.cn

Java: super.greet();
来源：http://ft.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mp.yuexingan06.cn

Ruby: super
来源：http://zs.haigaiapp.cn

C#:   base.Greet();
来源：http://nb.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://pi.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jz.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://zf.9csxet.cn

JS:   static f() {}
来源：http://tx.muxihuayi.cn

TS:   static f(): void {}
来源：http://wc.asd995.cn

Java: static void f() {}
来源：http://mc.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hv.yuexingan06.cn

Ruby: def self.f; end
来源：http://lj.shxzukj.cn

C#:   public static void F() {}
来源：http://br.hahajie.cn

[G09] 接口 / 抽象类
来源：http://cv.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://cs.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vh.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yu.521024.cn

TS:   interface Shape { area(): number; }
来源：http://pa.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://mp.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://jo.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ig.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://ay.shtwfgs.cn

[G10] 访问控制
来源：http://ii.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ix.szsharing.cn

PHP:  public / protected / private
来源：http://rc.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://oz.shxzskj.cn

TS:   public / protected / private
来源：http://mh.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://pr.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ri.nszjky.cn

Ruby: public / protected / private
来源：http://oo.newstarts.cn

C#:   public / protected / private / internal
来源：http://mm.nicolike.cn

[G11] getter / setter
来源：http://cw.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://ax.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sj.asd995.cn

JS:   get name() { return this._name; }
来源：http://ue.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ko.huanxung.cn

Java: public String getName() { return name; }
来源：http://gz.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tn.shxzukj.cn

Ruby: attr_accessor :name
来源：http://me.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://em.panjiajie.cn

[G12] 对象转字符串
来源：http://ag.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://qp.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gb.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://yy.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://am.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://ft.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qr.colortex.cn

Ruby: def to_s; @name; end
来源：http://bf.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://yq.szsharing.cn

[G13] 判断对象类型
来源：http://nw.lnxyls.cn

Py:   isinstance(u, User)
来源：http://pv.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ms.9csxet.cn

JS:   u instanceof User
来源：http://kc.szxytkj.cn

TS:   u instanceof User
来源：http://wl.bjjhwx.cn

Java: u instanceof User
来源：http://ba.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dn.asd995.cn

Ruby: u.is_a?(User)
来源：http://jf.yuexingan06.cn

C#:   u is User
来源：http://pt.gzmigu.cn

[G14] 数据类 / record
来源：http://zs.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mf.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bs.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gc.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://ti.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://ar.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://wf.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mi.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://fg.jianghongdianzi.cn

[G15] 枚举
来源：http://hi.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cv.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zr.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wf.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jn.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://af.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nn.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://hb.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wh.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://in.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qh.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://js.nszjky.cn

JS:   Object.entries(obj)
来源：http://py.shxzskj.cn

TS:   Object.entries(obj)
来源：http://mw.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wm.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gb.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://hk.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://vq.nszjky.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

H. 异常与错误处理
来源：http://yw.nszjky.cn

================================================================================
来源：http://dy.shxzskj.cn

[H01] try / catch 基础
来源：http://rp.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zy.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ee.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://un.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rf.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ai.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wp.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ac.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nf.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ve.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ou.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cm.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rb.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tz.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xc.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rg.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ou.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pf.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://dl.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://nh.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://js.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://sp.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://hc.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nq.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jc.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://er.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uq.asd995.cn

[H04] 自定义异常类型
来源：http://ke.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://hk.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://si.nszjky.cn

JS:   class MyError extends Error {}
来源：http://yb.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://on.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ld.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rx.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://dg.nszjky.cn

C#:   class MyException : Exception {}
来源：http://gq.huixiangedu.cn

[H05] 捕获特定类型
来源：http://gc.haigaiapp.cn

Py:   except ValueError as e:
来源：http://jp.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bx.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ls.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://dg.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://oc.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mo.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://gh.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xv.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://tl.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://fq.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dq.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ni.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zc.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hg.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://je.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://wb.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://gy.yuexingan06.cn

[H07] 断言
来源：http://wq.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://iw.gzmigu.cn

PHP:  assert($x > 0);
来源：http://vt.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://xy.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://nl.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://nn.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sr.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ha.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://gz.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://kp.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://vf.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jo.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://ks.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hj.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bb.gzmigu.cn

Go:   err.Error()
来源：http://wh.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://lx.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://ia.nicolike.cn

[H09] 带错误码的异常
来源：http://rm.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eb.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gu.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ay.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pg.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sh.shtwfgs.cn


<!-- 参考信息 -->