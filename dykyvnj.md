代发 wailian999

Ruby: File.delete("a.txt")
来源：http://pe.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://vx.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://mm.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fu.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tv.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fc.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://es.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cs.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pm.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lt.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cu.yuexingan06.cn

[F08] 遍历目录
来源：http://op.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rh.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qh.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://tu.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://gh.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://py.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cd.9csxet.cn

Ruby: Dir.children("dir")
来源：http://fh.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://eg.bjjhwx.cn

[F09] 获取文件大小
来源：http://bz.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://qn.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://bd.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://rz.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://ch.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://px.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dx.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://dw.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://nm.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://sp.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oa.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cy.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://id.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://sr.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ht.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zg.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://py.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ri.gzmigu.cn

[F11] 复制与移动文件
来源：http://iv.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ri.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hl.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ut.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vm.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zq.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ky.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jc.hnjuh.cn

[F12] CSV 读写
来源：http://qa.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wl.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nk.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fe.muxihuayi.cn

TS:   // 同上
来源：http://xf.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bn.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dr.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ek.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kc.lnxyls.cn

================================================================================
来源：http://sx.szsharing.cn

G. 面向对象
来源：http://ng.hnjuh.cn

================================================================================
来源：http://tb.huanxung.cn

[G01] 定义类
来源：http://cp.panjiajie.cn

Py:   class User: pass
来源：http://xj.bjjhwx.cn

PHP:  class User {}
来源：http://rx.wgjwhj.cn

JS:   class User {}
来源：http://rx.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://au.huixiangedu.cn

Java: class User {}
来源：http://pg.hahajie.cn

Go:   type User struct { Name string }
来源：http://gf.nszjky.cn

Ruby: class User; end
来源：http://ct.yuntaijiaju.cn

C#:   class User {}
来源：http://lj.panjiajie.cn

[G02] 构造函数
来源：http://gx.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://js.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://oh.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ya.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://uy.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://wc.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://er.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://rk.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://ln.jianghongdianzi.cn

[G03] 实例属性
来源：http://yy.9csxet.cn

Py:   self.name = "x"
来源：http://du.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://yc.chemitech.net.cn

JS:   this.name = "x";
来源：http://cp.szsharing.cn

TS:   name: string = "x";
来源：http://zy.hahajie.cn

Java: private String name;
来源：http://vq.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jp.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://xr.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://qi.newstarts.cn

[G04] 定义方法
来源：http://sd.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://dx.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vg.asd995.cn

JS:   greet() { return this.name; }
来源：http://tw.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://lf.gzmigu.cn

Java: String greet() { return name; }
来源：http://bw.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yg.nicolike.cn

Ruby: def greet; @name; end
来源：http://gc.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ir.yuexingan06.cn

[G05] 继承
来源：http://br.hahajie.cn

Py:   class Admin(User): pass
来源：http://ml.newstarts.cn

PHP:  class Admin extends User {}
来源：http://ul.huanxung.cn

JS:   class Admin extends User {}
来源：http://wl.hahajie.cn

TS:   class Admin extends User {}
来源：http://pi.wgjwhj.cn

Java: class Admin extends User {}
来源：http://pi.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aq.huanxung.cn

Ruby: class Admin < User; end
来源：http://is.chemitech.net.cn

C#:   class Admin : User {}
来源：http://xh.hnjuh.cn

[G06] 重写方法
来源：http://ka.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://rq.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ry.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://im.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://ve.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://nn.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rl.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://ul.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://yj.asd995.cn

[G07] 调用父类方法
来源：http://gt.9csxet.cn

Py:   super().greet()
来源：http://wz.nicolike.cn

PHP:  parent::greet();
来源：http://ow.chemitech.net.cn

JS:   super.greet();
来源：http://ju.9csxet.cn

TS:   super.greet();
来源：http://xw.hahajie.cn

Java: super.greet();
来源：http://fl.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rd.newstarts.cn

Ruby: super
来源：http://wq.yuntaijiaju.cn

C#:   base.Greet();
来源：http://hp.chemitech.net.cn

[G08] 静态方法与属性
来源：http://kf.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://et.muxihuayi.cn

PHP:  public static function f() {}
来源：http://pn.lnxyls.cn

JS:   static f() {}
来源：http://yg.bookmarksfly.cn

TS:   static f(): void {}
来源：http://vw.wgjwhj.cn

Java: static void f() {}
来源：http://kf.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://do.newstarts.cn

Ruby: def self.f; end
来源：http://en.newstarts.cn

C#:   public static void F() {}
来源：http://nz.colortex.cn

[G09] 接口 / 抽象类
来源：http://al.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://gj.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wg.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ei.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://fd.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://yq.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://rq.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jz.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://ic.521024.cn

[G10] 访问控制
来源：http://wc.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://kh.lnxyls.cn

PHP:  public / protected / private
来源：http://ua.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://go.shxzskj.cn

TS:   public / protected / private
来源：http://pj.asd995.cn

Java: public / protected / private / 默认包级
来源：http://re.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mg.haigaiapp.cn

Ruby: public / protected / private
来源：http://te.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://aj.szxytkj.cn

[G11] getter / setter
来源：http://uv.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://ov.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ph.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://vy.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://jk.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://wc.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tm.panjiajie.cn

Ruby: attr_accessor :name
来源：http://tu.nszjky.cn

C#:   public string Name { get; set; }
来源：http://kt.haigaiapp.cn

[G12] 对象转字符串
来源：http://sa.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://ed.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ts.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://jt.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://qt.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://ly.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pw.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://sw.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://es.shxzskj.cn

[G13] 判断对象类型
来源：http://xh.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://ey.9csxet.cn

PHP:  $u instanceof User
来源：http://vu.huixinmuqiang.cn

JS:   u instanceof User
来源：http://kg.asd995.cn

TS:   u instanceof User
来源：http://eh.nicolike.cn

Java: u instanceof User
来源：http://xf.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jb.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://sv.haigaiapp.cn

C#:   u is User
来源：http://px.haigaiapp.cn

[G14] 数据类 / record
来源：http://dz.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ie.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://yy.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uw.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://xf.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://am.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://cc.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qq.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://ve.szxytkj.cn

[G15] 枚举
来源：http://fx.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rn.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jd.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fa.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vc.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://ai.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ra.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://kj.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ek.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://cm.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ra.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://vd.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://qe.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://mn.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zb.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jn.asd995.cn

Ruby: obj.instance_variables
来源：http://wy.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://yn.shxzukj.cn

================================================================================
来源：http://gg.szsharing.cn

H. 异常与错误处理
来源：http://bz.9csxet.cn

================================================================================
来源：http://bn.szxytkj.cn

[H01] try / catch 基础
来源：http://jm.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://os.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ib.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lk.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uu.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iw.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fm.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://na.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://of.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://mz.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ua.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xd.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vo.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gw.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://te.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mt.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bc.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ih.huanxung.cn

[H03] 主动抛出异常
来源：http://md.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://fx.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xn.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://vm.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://eu.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lj.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nb.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dj.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://in.lnxyls.cn

[H04] 自定义异常类型
来源：http://fw.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://jw.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cq.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://ky.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://ry.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://pc.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rg.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://mp.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://dw.colortex.cn

[H05] 捕获特定类型
来源：http://ep.nszjky.cn

Py:   except ValueError as e:
来源：http://ax.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pw.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://lr.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://cp.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://xb.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xg.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://ev.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://ju.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://tq.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sh.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nx.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qv.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zk.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wo.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://fr.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://gf.nszjky.cn

[H07] 断言
来源：http://nw.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://kq.szsharing.cn

PHP:  assert($x > 0);
来源：http://op.huanxung.cn

JS:   console.assert(x > 0);
来源：http://nt.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ey.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://ox.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oa.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jc.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://pm.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://kz.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://oz.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rx.hahajie.cn

JS:   e.message;  e.stack
来源：http://ga.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aq.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hb.colortex.cn

Go:   err.Error()
来源：http://zt.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://zo.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://cm.521024.cn

[H09] 带错误码的异常
来源：http://bq.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pi.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zg.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://my.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oj.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ni.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://og.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zh.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ht.muxihuayi.cn

[H10] 资源自动释放
来源：http://yq.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://by.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://om.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sp.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ty.bookmarksfly.cn

Go:   defer f.Close()
来源：http://sv.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eh.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cx.bjjhwx.cn

================================================================================
来源：http://xn.haigaiapp.cn

I. 正则表达式
来源：http://oo.huixinmuqiang.cn

================================================================================
来源：http://cp.shxzskj.cn

[I01] 判断是否匹配
来源：http://qc.colortex.cn


<!-- 参考信息 -->