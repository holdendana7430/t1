代发 wailian999

Ruby: File.delete("a.txt")
来源：http://qj.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://tk.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://yg.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ey.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ao.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dz.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hn.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qo.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ye.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lj.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dd.szxytkj.cn

[F08] 遍历目录
来源：http://fb.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vo.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zc.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://xi.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://lh.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fi.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sn.nszjky.cn

Ruby: Dir.children("dir")
来源：http://li.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://uf.huixiangedu.cn

[F09] 获取文件大小
来源：http://gn.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://dn.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://nk.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://fh.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://jc.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://je.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fm.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://jc.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://wg.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://xf.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yr.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ss.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fs.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://vf.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xn.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://re.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vo.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ae.asd995.cn

[F11] 复制与移动文件
来源：http://ww.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jz.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sw.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ix.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lr.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yt.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ip.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yq.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zy.jctech888.com.cn

[F12] CSV 读写
来源：http://nd.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cw.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cs.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rv.asd995.cn

TS:   // 同上
来源：http://kl.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://je.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yx.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tt.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ca.szxytkj.cn

================================================================================
来源：http://qt.panjiajie.cn

G. 面向对象
来源：http://sb.jianghongdianzi.cn

================================================================================
来源：http://xv.muxihuayi.cn

[G01] 定义类
来源：http://jz.huixinmuqiang.cn

Py:   class User: pass
来源：http://pa.colortex.cn

PHP:  class User {}
来源：http://ci.panjiajie.cn

JS:   class User {}
来源：http://eo.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://kg.huanxung.cn

Java: class User {}
来源：http://pz.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://rn.9csxet.cn

Ruby: class User; end
来源：http://ib.newstarts.cn

C#:   class User {}
来源：http://tx.bookmarksfly.cn

[G02] 构造函数
来源：http://ho.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://rv.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://tu.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://ij.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://hn.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://ek.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ao.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://pl.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ri.huixinmuqiang.cn

[G03] 实例属性
来源：http://ls.bookmarksfly.cn

Py:   self.name = "x"
来源：http://cs.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://ax.panjiajie.cn

JS:   this.name = "x";
来源：http://zs.nicolike.cn

TS:   name: string = "x";
来源：http://gz.9csxet.cn

Java: private String name;
来源：http://oj.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yl.nszjky.cn

Ruby: @name = "x"
来源：http://ak.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://zf.nicolike.cn

[G04] 定义方法
来源：http://sq.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://or.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://px.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://tz.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://qe.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ms.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vs.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://rg.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://jo.szxytkj.cn

[G05] 继承
来源：http://zv.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ky.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://fw.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://vu.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ew.szsharing.cn

Java: class Admin extends User {}
来源：http://sv.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yp.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ub.lnxyls.cn

C#:   class Admin : User {}
来源：http://qz.huixiangedu.cn

[G06] 重写方法
来源：http://ch.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://dh.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rq.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://py.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://yc.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://gq.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zi.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://cs.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://gm.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zp.hahajie.cn

Py:   super().greet()
来源：http://nf.muxihuayi.cn

PHP:  parent::greet();
来源：http://gp.yuexingan06.cn

JS:   super.greet();
来源：http://li.huixinmuqiang.cn

TS:   super.greet();
来源：http://ha.huixiangedu.cn

Java: super.greet();
来源：http://fr.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vn.9csxet.cn

Ruby: super
来源：http://at.huixiangedu.cn

C#:   base.Greet();
来源：http://js.hahajie.cn

[G08] 静态方法与属性
来源：http://zd.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ez.chemitech.net.cn

PHP:  public static function f() {}
来源：http://jq.bjjhwx.cn

JS:   static f() {}
来源：http://qb.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://la.huixinmuqiang.cn

Java: static void f() {}
来源：http://bu.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mg.szsharing.cn

Ruby: def self.f; end
来源：http://nj.521024.cn

C#:   public static void F() {}
来源：http://kp.nszjky.cn

[G09] 接口 / 抽象类
来源：http://hp.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://nv.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qp.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jv.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://sx.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://pq.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://yt.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yo.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://wg.shxzskj.cn

[G10] 访问控制
来源：http://lb.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://xq.panjiajie.cn

PHP:  public / protected / private
来源：http://ro.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://cq.nicolike.cn

TS:   public / protected / private
来源：http://qe.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://fd.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qa.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ki.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://cx.shxzskj.cn

[G11] getter / setter
来源：http://jq.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://gp.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gj.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ks.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://lz.9csxet.cn

Java: public String getName() { return name; }
来源：http://rl.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lq.521024.cn

Ruby: attr_accessor :name
来源：http://ly.szsharing.cn

C#:   public string Name { get; set; }
来源：http://jz.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://wf.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://nq.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qo.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://sk.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://dg.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ha.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zx.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://nc.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://ud.szsharing.cn

[G13] 判断对象类型
来源：http://wc.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ty.hahajie.cn

PHP:  $u instanceof User
来源：http://cr.szsharing.cn

JS:   u instanceof User
来源：http://yz.wgjwhj.cn

TS:   u instanceof User
来源：http://sj.huixiangedu.cn

Java: u instanceof User
来源：http://jl.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nv.hahajie.cn

Ruby: u.is_a?(User)
来源：http://nx.hahajie.cn

C#:   u is User
来源：http://xi.nicolike.cn

[G14] 数据类 / record
来源：http://nd.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sh.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://sq.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dr.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://bp.521024.cn

Java: record User(String name, int age) {}
来源：http://os.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://hn.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qo.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://cd.huixinmuqiang.cn

[G15] 枚举
来源：http://ui.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fl.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ua.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ul.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vl.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://aq.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vv.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://jv.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pi.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://ic.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ay.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://of.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://vn.szsharing.cn

TS:   Object.entries(obj)
来源：http://vi.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ep.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fh.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://iv.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://yx.hahajie.cn

================================================================================
来源：http://dp.jianghongdianzi.cn

H. 异常与错误处理
来源：http://lw.hahajie.cn

================================================================================
来源：http://fo.haigaiapp.cn

[H01] try / catch 基础
来源：http://wu.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ms.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pp.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gf.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://as.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dj.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ar.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mk.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gj.hahajie.cn

[H02] finally / ensure 收尾
来源：http://qr.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xp.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tz.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bz.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ys.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dd.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://el.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dp.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kt.colortex.cn

[H03] 主动抛出异常
来源：http://rn.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://fn.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xq.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://nv.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://at.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fc.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nc.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sn.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nv.hnjuh.cn

[H04] 自定义异常类型
来源：http://zt.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://jq.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jp.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://nk.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://ow.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://gi.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ov.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://rb.newstarts.cn

C#:   class MyException : Exception {}
来源：http://fy.colortex.cn

[H05] 捕获特定类型
来源：http://ef.lnxyls.cn

Py:   except ValueError as e:
来源：http://zb.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wz.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://iq.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://lh.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://cp.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://av.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://jh.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://el.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://cw.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://vk.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uk.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ia.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fj.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hk.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gr.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://uf.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://sp.hnjuh.cn

[H07] 断言
来源：http://wf.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://zj.nicolike.cn

PHP:  assert($x > 0);
来源：http://ag.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://fx.asd995.cn

TS:   console.assert(x > 0);
来源：http://dq.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://bz.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hs.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oi.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://zd.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://aa.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://ba.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zf.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://dk.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tu.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rt.bjjhwx.cn

Go:   err.Error()
来源：http://cw.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://fj.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://ek.shxzukj.cn

[H09] 带错误码的异常
来源：http://wc.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://si.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bc.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://za.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ru.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gz.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sd.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ec.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rk.chemitech.net.cn

[H10] 资源自动释放
来源：http://cn.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vo.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qz.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ut.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oe.bjjhwx.cn

Go:   defer f.Close()
来源：http://aa.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yq.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://as.shxzskj.cn

================================================================================
来源：http://fy.shxzukj.cn

I. 正则表达式
来源：http://ls.huixiangedu.cn

================================================================================
来源：http://cz.newstarts.cn

[I01] 判断是否匹配
来源：http://dy.gzmigu.cn


<!-- 参考信息 -->