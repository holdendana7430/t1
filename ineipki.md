代发 wailian999

Ruby: File.delete("a.txt")
来源：http://av.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://tv.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://kt.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nb.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nl.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fh.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bn.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ve.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ty.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kh.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xt.haigaiapp.cn

[F08] 遍历目录
来源：http://dy.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jh.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://io.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://xe.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://gs.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cj.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xi.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://rb.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://ra.newstarts.cn

[F09] 获取文件大小
来源：http://eg.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://lu.hahajie.cn

PHP:  filesize("a.txt");
来源：http://sp.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://xz.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://pv.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cq.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xg.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://yy.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://lo.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://vi.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bp.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://df.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yi.hahajie.cn

TS:   path.extname("a.txt")
来源：http://ny.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aq.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tm.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hw.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://il.jctech888.com.cn

[F11] 复制与移动文件
来源：http://ul.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ea.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vh.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qz.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ks.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sy.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bv.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ql.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rx.shxzukj.cn

[F12] CSV 读写
来源：http://ko.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eq.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zy.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zd.huixiangedu.cn

TS:   // 同上
来源：http://lu.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sk.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ed.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vz.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://as.haigaiapp.cn

================================================================================
来源：http://ma.chemitech.net.cn

G. 面向对象
来源：http://hw.jianghongdianzi.cn

================================================================================
来源：http://mq.hnjuh.cn

[G01] 定义类
来源：http://mo.haigaiapp.cn

Py:   class User: pass
来源：http://nx.bookmarksfly.cn

PHP:  class User {}
来源：http://gf.panjiajie.cn

JS:   class User {}
来源：http://hx.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://ix.huixinmuqiang.cn

Java: class User {}
来源：http://am.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://jd.9csxet.cn

Ruby: class User; end
来源：http://nt.bookmarksfly.cn

C#:   class User {}
来源：http://yl.hnjuh.cn

[G02] 构造函数
来源：http://nv.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://hm.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://ll.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://be.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ci.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://te.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://no.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ea.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://rs.colortex.cn

[G03] 实例属性
来源：http://ci.shxzskj.cn

Py:   self.name = "x"
来源：http://uc.shxzukj.cn

PHP:  public string $name = "x";
来源：http://uu.nicolike.cn

JS:   this.name = "x";
来源：http://xg.521024.cn

TS:   name: string = "x";
来源：http://ah.chemitech.net.cn

Java: private String name;
来源：http://rq.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vk.asd995.cn

Ruby: @name = "x"
来源：http://xm.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://hk.colortex.cn

[G04] 定义方法
来源：http://uv.huanxung.cn

Py:   def greet(self): return self.name
来源：http://su.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yb.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://cz.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://aj.gzmigu.cn

Java: String greet() { return name; }
来源：http://wh.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tr.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://jn.newstarts.cn

C#:   public string Greet() => Name;
来源：http://gk.shxzskj.cn

[G05] 继承
来源：http://vn.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://dj.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://jk.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://zr.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://aj.nszjky.cn

Java: class Admin extends User {}
来源：http://ew.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gm.panjiajie.cn

Ruby: class Admin < User; end
来源：http://ft.chemitech.net.cn

C#:   class Admin : User {}
来源：http://hr.colortex.cn

[G06] 重写方法
来源：http://ql.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://lo.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vr.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://gs.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://rl.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://sg.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://au.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://gh.521024.cn

C#:   public override string Greet() => "admin";
来源：http://bt.wgjwhj.cn

[G07] 调用父类方法
来源：http://tz.muxihuayi.cn

Py:   super().greet()
来源：http://wi.yuexingan06.cn

PHP:  parent::greet();
来源：http://mu.haigaiapp.cn

JS:   super.greet();
来源：http://lh.colortex.cn

TS:   super.greet();
来源：http://ee.colortex.cn

Java: super.greet();
来源：http://dd.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dt.shxzskj.cn

Ruby: super
来源：http://pv.hahajie.cn

C#:   base.Greet();
来源：http://xt.9csxet.cn

[G08] 静态方法与属性
来源：http://tw.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://es.yuexingan06.cn

PHP:  public static function f() {}
来源：http://tz.nicolike.cn

JS:   static f() {}
来源：http://jv.jctech888.com.cn

TS:   static f(): void {}
来源：http://te.panjiajie.cn

Java: static void f() {}
来源：http://ms.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tn.shxzskj.cn

Ruby: def self.f; end
来源：http://sd.shxzskj.cn

C#:   public static void F() {}
来源：http://vo.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://xj.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://cm.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xo.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nh.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://pg.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://hf.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://tt.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lx.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://uf.szxytkj.cn

[G10] 访问控制
来源：http://si.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://if.szxytkj.cn

PHP:  public / protected / private
来源：http://ia.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://iu.nicolike.cn

TS:   public / protected / private
来源：http://ep.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://pu.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fg.szxytkj.cn

Ruby: public / protected / private
来源：http://if.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://zr.hnjuh.cn

[G11] getter / setter
来源：http://ju.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://tr.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ks.asd995.cn

JS:   get name() { return this._name; }
来源：http://mg.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://mn.nszjky.cn

Java: public String getName() { return name; }
来源：http://nn.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cm.lnxyls.cn

Ruby: attr_accessor :name
来源：http://zq.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://eg.haigaiapp.cn

[G12] 对象转字符串
来源：http://zp.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://dq.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://de.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://gp.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://tm.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://tk.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wu.huanxung.cn

Ruby: def to_s; @name; end
来源：http://mq.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://xo.yuexingan06.cn

[G13] 判断对象类型
来源：http://hm.nicolike.cn

Py:   isinstance(u, User)
来源：http://vj.nszjky.cn

PHP:  $u instanceof User
来源：http://zj.panjiajie.cn

JS:   u instanceof User
来源：http://jw.521024.cn

TS:   u instanceof User
来源：http://ts.wgjwhj.cn

Java: u instanceof User
来源：http://rp.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://te.colortex.cn

Ruby: u.is_a?(User)
来源：http://ht.szxytkj.cn

C#:   u is User
来源：http://xx.bjjhwx.cn

[G14] 数据类 / record
来源：http://rf.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yq.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://sb.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ed.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://oy.nicolike.cn

Java: record User(String name, int age) {}
来源：http://ch.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://sz.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qt.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://cu.shxzukj.cn

[G15] 枚举
来源：http://of.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://va.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ep.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ca.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fa.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://ei.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sz.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://pr.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yl.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://gh.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ri.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://xq.521024.cn

JS:   Object.entries(obj)
来源：http://vu.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://hq.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ll.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ge.hahajie.cn

Ruby: obj.instance_variables
来源：http://kw.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://cu.asd995.cn

================================================================================
来源：http://ms.jctech888.com.cn

H. 异常与错误处理
来源：http://nd.nszjky.cn

================================================================================
来源：http://ri.shxzukj.cn

[H01] try / catch 基础
来源：http://ag.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lv.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xk.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ft.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jc.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cn.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qg.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pf.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wn.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://qp.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dk.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nd.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bd.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uo.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zb.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bp.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cb.szsharing.cn

[H03] 主动抛出异常
来源：http://xf.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://eu.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://an.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://bx.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://tm.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dj.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mf.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ag.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ae.shxzskj.cn

[H04] 自定义异常类型
来源：http://ue.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://dj.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tv.asd995.cn

JS:   class MyError extends Error {}
来源：http://sy.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://rg.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://uh.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lj.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ft.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://xv.chemitech.net.cn

[H05] 捕获特定类型
来源：http://dz.shxzskj.cn

Py:   except ValueError as e:
来源：http://xh.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jb.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://ld.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://zz.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://ru.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://br.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://yx.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zb.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://xl.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://br.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nh.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ss.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nc.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ze.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jw.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://kj.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://ou.hahajie.cn

[H07] 断言
来源：http://ad.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://so.panjiajie.cn

PHP:  assert($x > 0);
来源：http://ee.colortex.cn

JS:   console.assert(x > 0);
来源：http://tt.hahajie.cn

TS:   console.assert(x > 0);
来源：http://ac.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://ab.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://el.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gi.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://mr.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://di.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://mn.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nd.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://zk.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oa.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://na.wgjwhj.cn

Go:   err.Error()
来源：http://wy.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://il.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://ya.521024.cn

[H09] 带错误码的异常
来源：http://wu.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gf.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pi.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tn.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://si.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kz.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zr.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lg.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kb.huixiangedu.cn

[H10] 资源自动释放
来源：http://pw.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rr.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qv.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xf.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rr.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bo.huanxung.cn

Go:   defer f.Close()
来源：http://hj.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ds.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pj.huanxung.cn

================================================================================
来源：http://nc.521024.cn

I. 正则表达式
来源：http://rh.yuntaijiaju.cn

================================================================================
来源：http://te.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://sm.huixinmuqiang.cn


<!-- 参考信息 -->