代发 wailian999

C#:   File.Exists("a.txt")
来源：http://rz.yuexingan06.cn

[F06] 删除文件
来源：http://ck.521024.cn

Py:   os.remove("a.txt")
来源：http://au.asd995.cn

PHP:  unlink("a.txt");
来源：http://px.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ry.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hx.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vb.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://qo.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://wu.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://rp.9csxet.cn

[F07] 创建目录（含多级）
来源：http://uh.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ch.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jp.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gh.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wj.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rj.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kr.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nj.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kr.nicolike.cn

[F08] 遍历目录
来源：http://pe.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jo.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ao.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://vr.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://mz.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mu.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pp.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://bm.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ig.9csxet.cn

[F09] 获取文件大小
来源：http://ud.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://qv.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://wv.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://kx.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://fd.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wd.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vh.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://jq.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://vo.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://zc.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vm.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tw.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hp.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://uf.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xa.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tx.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ca.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mb.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://hg.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dc.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rf.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pt.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bm.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rs.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pi.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ej.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zm.yuntaijiaju.cn

[F12] CSV 读写
来源：http://xj.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mu.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gu.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pu.shxzukj.cn

TS:   // 同上
来源：http://ps.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jo.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mt.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mm.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kd.hahajie.cn

================================================================================
来源：http://gu.huixiangedu.cn

G. 面向对象
来源：http://fm.newstarts.cn

================================================================================
来源：http://ks.bookmarksfly.cn

[G01] 定义类
来源：http://za.hnjuh.cn

Py:   class User: pass
来源：http://lx.shtwfgs.cn

PHP:  class User {}
来源：http://lj.chemitech.net.cn

JS:   class User {}
来源：http://xi.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://fq.huanxung.cn

Java: class User {}
来源：http://su.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://ud.jctech888.com.cn

Ruby: class User; end
来源：http://cw.521024.cn

C#:   class User {}
来源：http://sl.bjjhwx.cn

[G02] 构造函数
来源：http://uy.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://nq.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://nd.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://vj.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://sm.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://pw.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uv.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://dl.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://ax.haigaiapp.cn

[G03] 实例属性
来源：http://fa.9csxet.cn

Py:   self.name = "x"
来源：http://rm.nszjky.cn

PHP:  public string $name = "x";
来源：http://db.szsharing.cn

JS:   this.name = "x";
来源：http://zz.hahajie.cn

TS:   name: string = "x";
来源：http://ne.newstarts.cn

Java: private String name;
来源：http://yu.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vu.asd995.cn

Ruby: @name = "x"
来源：http://wu.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://iy.jctech888.com.cn

[G04] 定义方法
来源：http://mi.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://gh.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ie.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://ba.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://sd.shtwfgs.cn

Java: String greet() { return name; }
来源：http://vo.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zw.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://gt.nicolike.cn

C#:   public string Greet() => Name;
来源：http://vj.nszjky.cn

[G05] 继承
来源：http://tg.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://cu.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://vr.hnjuh.cn

JS:   class Admin extends User {}
来源：http://de.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://bg.shxzukj.cn

Java: class Admin extends User {}
来源：http://fn.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hn.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://od.nicolike.cn

C#:   class Admin : User {}
来源：http://gs.muxihuayi.cn

[G06] 重写方法
来源：http://il.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://nr.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ch.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://xg.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://mg.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://lf.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qt.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://dc.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://ty.shtwfgs.cn

[G07] 调用父类方法
来源：http://uw.lnxyls.cn

Py:   super().greet()
来源：http://xa.haigaiapp.cn

PHP:  parent::greet();
来源：http://ji.bookmarksfly.cn

JS:   super.greet();
来源：http://yo.shxzukj.cn

TS:   super.greet();
来源：http://xv.jctech888.com.cn

Java: super.greet();
来源：http://la.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ja.huixiangedu.cn

Ruby: super
来源：http://nw.hahajie.cn

C#:   base.Greet();
来源：http://gs.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://nt.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://es.asd995.cn

PHP:  public static function f() {}
来源：http://ma.panjiajie.cn

JS:   static f() {}
来源：http://oi.lnxyls.cn

TS:   static f(): void {}
来源：http://vz.haigaiapp.cn

Java: static void f() {}
来源：http://kx.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pr.huixiangedu.cn

Ruby: def self.f; end
来源：http://rs.panjiajie.cn

C#:   public static void F() {}
来源：http://dw.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://fu.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://fu.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pr.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://qv.szsharing.cn

Java: interface Shape { double area(); }
来源：http://ic.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://da.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oe.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://il.yuexingan06.cn

[G10] 访问控制
来源：http://qm.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://jz.hahajie.cn

PHP:  public / protected / private
来源：http://ao.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://xx.colortex.cn

TS:   public / protected / private
来源：http://wf.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://rk.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lp.shtwfgs.cn

Ruby: public / protected / private
来源：http://ef.huanxung.cn

C#:   public / protected / private / internal
来源：http://ix.yuexingan06.cn

[G11] getter / setter
来源：http://hx.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://dp.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://to.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://rd.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://cv.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://mj.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pe.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://db.newstarts.cn

C#:   public string Name { get; set; }
来源：http://yg.shxzskj.cn

[G12] 对象转字符串
来源：http://wl.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://tz.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pk.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://zc.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://fz.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://eo.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ay.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://fw.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://nr.bookmarksfly.cn

[G13] 判断对象类型
来源：http://ss.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://pc.asd995.cn

PHP:  $u instanceof User
来源：http://hn.huanxung.cn

JS:   u instanceof User
来源：http://ie.nszjky.cn

TS:   u instanceof User
来源：http://mp.lnxyls.cn

Java: u instanceof User
来源：http://qm.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ya.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://lq.chemitech.net.cn

C#:   u is User
来源：http://vm.shtwfgs.cn

[G14] 数据类 / record
来源：http://sd.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://br.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://oq.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zp.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://gm.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://jn.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://tr.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ly.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://en.nicolike.cn

[G15] 枚举
来源：http://va.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cz.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ct.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ve.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qe.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://ml.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hh.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://od.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ed.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://az.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tb.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://jx.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ad.newstarts.cn

TS:   Object.entries(obj)
来源：http://re.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cq.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mh.szsharing.cn

Ruby: obj.instance_variables
来源：http://dp.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ml.shtwfgs.cn

================================================================================
来源：http://qm.huixinmuqiang.cn

H. 异常与错误处理
来源：http://lo.nszjky.cn

================================================================================
来源：http://em.nicolike.cn

[H01] try / catch 基础
来源：http://yv.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pd.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xh.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wm.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hb.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://au.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rk.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zu.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lz.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ja.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gi.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ga.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tc.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://in.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zy.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wv.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dl.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://md.panjiajie.cn

[H03] 主动抛出异常
来源：http://mb.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://dc.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cd.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://mb.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://hy.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cy.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ut.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gr.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mp.yuexingan06.cn

[H04] 自定义异常类型
来源：http://sa.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://mo.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gt.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://hm.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://su.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://zj.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://op.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://bm.521024.cn

C#:   class MyException : Exception {}
来源：http://dy.asd995.cn

[H05] 捕获特定类型
来源：http://sf.9csxet.cn

Py:   except ValueError as e:
来源：http://pa.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://no.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://vv.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ev.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://hf.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qf.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://jj.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oo.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://ic.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://wg.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ey.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bo.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jv.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ru.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tq.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://as.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://zk.nszjky.cn

[H07] 断言
来源：http://dp.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ti.newstarts.cn

PHP:  assert($x > 0);
来源：http://lz.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://yu.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://wy.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://ni.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nc.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yx.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://xf.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://mm.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://xf.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ww.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://jz.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dj.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dn.shxzskj.cn

Go:   err.Error()
来源：http://yz.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://di.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ar.haigaiapp.cn

[H09] 带错误码的异常
来源：http://tp.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lc.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pp.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ev.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ws.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vr.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fp.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bq.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ym.jctech888.com.cn

[H10] 资源自动释放
来源：http://ur.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://px.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kv.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nq.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gl.nszjky.cn


<!-- 参考信息 -->