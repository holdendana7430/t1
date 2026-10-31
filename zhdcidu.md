代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://qr.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mo.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://va.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ue.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ey.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kp.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wp.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://st.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://hs.jianghongdianzi.cn

[F06] 删除文件
来源：http://zj.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://or.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://xr.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fq.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yr.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nf.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ql.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://tg.521024.cn

C#:   File.Delete("a.txt");
来源：http://yd.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://tm.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://om.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fo.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ro.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ni.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://os.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jz.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ao.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rw.muxihuayi.cn

[F08] 遍历目录
来源：http://gk.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://im.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ti.521024.cn

JS:   fs.readdirSync("dir")
来源：http://bg.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://gz.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pw.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ta.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://vn.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://bu.huanxung.cn

[F09] 获取文件大小
来源：http://zk.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://pg.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://yq.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://rq.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://ks.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nn.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mg.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://kl.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ok.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gw.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kf.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ym.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pi.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://wp.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ad.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hq.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://da.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yi.huanxung.cn

[F11] 复制与移动文件
来源：http://hn.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ze.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qq.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qf.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qq.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bi.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hk.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jt.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ce.shtwfgs.cn

[F12] CSV 读写
来源：http://iv.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sv.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dw.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bq.colortex.cn

TS:   // 同上
来源：http://qd.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qu.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cc.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ss.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yg.szxytkj.cn

================================================================================
来源：http://mq.lnxyls.cn

G. 面向对象
来源：http://mi.szsharing.cn

================================================================================
来源：http://mo.shtwfgs.cn

[G01] 定义类
来源：http://ft.gzmigu.cn

Py:   class User: pass
来源：http://gf.shxzukj.cn

PHP:  class User {}
来源：http://pv.yuexingan06.cn

JS:   class User {}
来源：http://nh.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://wl.haigaiapp.cn

Java: class User {}
来源：http://oc.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://dn.wgjwhj.cn

Ruby: class User; end
来源：http://mv.bjjhwx.cn

C#:   class User {}
来源：http://gu.bookmarksfly.cn

[G02] 构造函数
来源：http://zn.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://pd.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hm.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://dk.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://hb.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://rl.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ef.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://xf.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://dz.asd995.cn

[G03] 实例属性
来源：http://tz.nszjky.cn

Py:   self.name = "x"
来源：http://ao.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ee.lnxyls.cn

JS:   this.name = "x";
来源：http://wh.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://uy.521024.cn

Java: private String name;
来源：http://ad.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ps.521024.cn

Ruby: @name = "x"
来源：http://kr.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://bo.lnxyls.cn

[G04] 定义方法
来源：http://zd.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://mu.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ur.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://qn.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://rn.szxytkj.cn

Java: String greet() { return name; }
来源：http://rp.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lo.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://ad.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://it.hahajie.cn

[G05] 继承
来源：http://ne.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ud.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://bm.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://we.szxytkj.cn

TS:   class Admin extends User {}
来源：http://zn.shtwfgs.cn

Java: class Admin extends User {}
来源：http://xp.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://py.nicolike.cn

Ruby: class Admin < User; end
来源：http://lb.9csxet.cn

C#:   class Admin : User {}
来源：http://uh.panjiajie.cn

[G06] 重写方法
来源：http://ys.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ya.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mw.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://te.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://xx.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://rd.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kp.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://zw.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://bs.huixiangedu.cn

[G07] 调用父类方法
来源：http://ec.chemitech.net.cn

Py:   super().greet()
来源：http://eu.hahajie.cn

PHP:  parent::greet();
来源：http://rk.panjiajie.cn

JS:   super.greet();
来源：http://ax.asd995.cn

TS:   super.greet();
来源：http://xn.jctech888.com.cn

Java: super.greet();
来源：http://ii.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://na.muxihuayi.cn

Ruby: super
来源：http://pz.shxzukj.cn

C#:   base.Greet();
来源：http://qu.haigaiapp.cn

[G08] 静态方法与属性
来源：http://io.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xd.szxytkj.cn

PHP:  public static function f() {}
来源：http://vx.521024.cn

JS:   static f() {}
来源：http://ba.haigaiapp.cn

TS:   static f(): void {}
来源：http://dt.yuntaijiaju.cn

Java: static void f() {}
来源：http://kk.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rd.shtwfgs.cn

Ruby: def self.f; end
来源：http://lg.panjiajie.cn

C#:   public static void F() {}
来源：http://ej.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://id.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://rf.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ce.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qu.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://gw.nicolike.cn

Java: interface Shape { double area(); }
来源：http://vt.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://hl.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wi.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://gr.shxzukj.cn

[G10] 访问控制
来源：http://wm.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://zt.nicolike.cn

PHP:  public / protected / private
来源：http://fv.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://wh.wgjwhj.cn

TS:   public / protected / private
来源：http://ud.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://cz.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lg.szxytkj.cn

Ruby: public / protected / private
来源：http://zc.hnjuh.cn

C#:   public / protected / private / internal
来源：http://nn.wgjwhj.cn

[G11] getter / setter
来源：http://th.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://uv.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vo.huanxung.cn

JS:   get name() { return this._name; }
来源：http://pk.521024.cn

TS:   get name(): string { return this._name; }
来源：http://gk.shxzskj.cn

Java: public String getName() { return name; }
来源：http://aw.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wc.lnxyls.cn

Ruby: attr_accessor :name
来源：http://fo.nicolike.cn

C#:   public string Name { get; set; }
来源：http://mr.asd995.cn

[G12] 对象转字符串
来源：http://wt.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://zn.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nc.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://vn.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://yi.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://zz.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fa.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://ae.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://sy.nicolike.cn

[G13] 判断对象类型
来源：http://fr.521024.cn

Py:   isinstance(u, User)
来源：http://fv.haigaiapp.cn

PHP:  $u instanceof User
来源：http://kx.nicolike.cn

JS:   u instanceof User
来源：http://py.wgjwhj.cn

TS:   u instanceof User
来源：http://la.haigaiapp.cn

Java: u instanceof User
来源：http://ql.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jr.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://tl.bookmarksfly.cn

C#:   u is User
来源：http://sb.panjiajie.cn

[G14] 数据类 / record
来源：http://yc.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tc.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://sj.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qn.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://by.hahajie.cn

Java: record User(String name, int age) {}
来源：http://dz.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://oi.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zu.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://zj.shxzukj.cn

[G15] 枚举
来源：http://cn.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vp.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ep.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nt.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lj.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://eu.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://de.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://ve.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yg.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ou.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gr.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://fv.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://ss.9csxet.cn

TS:   Object.entries(obj)
来源：http://jr.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kl.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rq.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://vp.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://wb.nszjky.cn

================================================================================
来源：http://it.yuexingan06.cn

H. 异常与错误处理
来源：http://fx.521024.cn

================================================================================
来源：http://zz.bjjhwx.cn

[H01] try / catch 基础
来源：http://ap.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tw.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dg.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fs.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ku.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vc.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fq.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ql.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://at.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ko.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kt.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wl.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qx.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sp.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hi.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rg.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://px.asd995.cn

[H03] 主动抛出异常
来源：http://hb.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://gi.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ks.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://me.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://bx.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://it.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tz.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lf.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ik.shtwfgs.cn

[H04] 自定义异常类型
来源：http://di.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://no.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://et.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://vp.newstarts.cn

TS:   class MyError extends Error {}
来源：http://qg.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://js.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://du.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://gi.nicolike.cn

C#:   class MyException : Exception {}
来源：http://tx.lnxyls.cn

[H05] 捕获特定类型
来源：http://ny.muxihuayi.cn

Py:   except ValueError as e:
来源：http://yq.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://br.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://kd.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://bs.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://wj.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sq.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://mr.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kr.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://zm.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://im.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sf.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jg.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dn.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xp.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jf.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://js.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://qa.nicolike.cn

[H07] 断言
来源：http://ey.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://yz.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://zy.9csxet.cn

JS:   console.assert(x > 0);
来源：http://bg.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://dr.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://aa.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rh.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wh.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://ta.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://mg.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://zn.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ht.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://co.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zq.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hu.hnjuh.cn

Go:   err.Error()
来源：http://oj.521024.cn

Ruby: e.message;  e.backtrace
来源：http://iv.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://oy.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://uu.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ah.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://un.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kh.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://if.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cs.nszjky.cn


<!-- 参考信息 -->