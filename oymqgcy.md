代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://eo.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bh.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://te.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://be.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ko.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://pz.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://rk.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ot.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ru.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uy.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zz.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nq.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lk.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lk.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xt.huixiangedu.cn

[F08] 遍历目录
来源：http://qv.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lk.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://en.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://iz.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://pn.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dw.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fm.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://mg.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://wo.colortex.cn

[F09] 获取文件大小
来源：http://ae.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://bh.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://wm.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://wc.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://hc.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wq.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ds.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://yh.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://rb.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://db.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://on.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cv.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hj.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://ac.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jp.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://th.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vk.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://no.bjjhwx.cn

[F11] 复制与移动文件
来源：http://or.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vk.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dm.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bu.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://th.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pi.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cy.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ls.shtwfgs.cn

[F12] CSV 读写
来源：http://nm.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tt.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://og.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qw.bjjhwx.cn

TS:   // 同上
来源：http://jx.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wn.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mn.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ht.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tx.9csxet.cn

================================================================================
来源：http://mk.colortex.cn

G. 面向对象
来源：http://rn.asd995.cn

================================================================================
来源：http://zx.wgjwhj.cn

[G01] 定义类
来源：http://go.shxzukj.cn

Py:   class User: pass
来源：http://wq.nicolike.cn

PHP:  class User {}
来源：http://jk.nicolike.cn

JS:   class User {}
来源：http://do.521024.cn

TS:   class User { name: string = ""; }
来源：http://fk.huixinmuqiang.cn

Java: class User {}
来源：http://xq.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://hd.bookmarksfly.cn

Ruby: class User; end
来源：http://oy.newstarts.cn

C#:   class User {}
来源：http://bk.yuexingan06.cn

[G02] 构造函数
来源：http://zy.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://ew.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://cf.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ac.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://ud.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://kb.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tj.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://fw.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://ub.shtwfgs.cn

[G03] 实例属性
来源：http://bi.panjiajie.cn

Py:   self.name = "x"
来源：http://px.hahajie.cn

PHP:  public string $name = "x";
来源：http://ro.hnjuh.cn

JS:   this.name = "x";
来源：http://ka.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://bp.bookmarksfly.cn

Java: private String name;
来源：http://ys.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xr.szxytkj.cn

Ruby: @name = "x"
来源：http://ae.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://vd.nszjky.cn

[G04] 定义方法
来源：http://ct.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://yf.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://th.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://vl.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://uv.jctech888.com.cn

Java: String greet() { return name; }
来源：http://sg.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hn.nszjky.cn

Ruby: def greet; @name; end
来源：http://si.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://vr.newstarts.cn

[G05] 继承
来源：http://ih.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://uo.nicolike.cn

PHP:  class Admin extends User {}
来源：http://wu.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://es.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://gs.szsharing.cn

Java: class Admin extends User {}
来源：http://tq.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vc.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ce.muxihuayi.cn

C#:   class Admin : User {}
来源：http://mf.huanxung.cn

[G06] 重写方法
来源：http://tt.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://pb.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hm.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://rf.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://np.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://tu.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oj.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://qa.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://cc.nicolike.cn

[G07] 调用父类方法
来源：http://fn.haigaiapp.cn

Py:   super().greet()
来源：http://ec.huixiangedu.cn

PHP:  parent::greet();
来源：http://cr.huixiangedu.cn

JS:   super.greet();
来源：http://cb.yuexingan06.cn

TS:   super.greet();
来源：http://co.panjiajie.cn

Java: super.greet();
来源：http://iq.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pf.nszjky.cn

Ruby: super
来源：http://kv.huixinmuqiang.cn

C#:   base.Greet();
来源：http://wv.shxzukj.cn

[G08] 静态方法与属性
来源：http://ms.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uw.huixiangedu.cn

PHP:  public static function f() {}
来源：http://pb.521024.cn

JS:   static f() {}
来源：http://bt.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://cp.jctech888.com.cn

Java: static void f() {}
来源：http://wl.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://px.bookmarksfly.cn

Ruby: def self.f; end
来源：http://iu.szsharing.cn

C#:   public static void F() {}
来源：http://xj.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://at.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://cn.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dk.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ec.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://fc.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://gq.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://ok.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ab.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ew.wgjwhj.cn

[G10] 访问控制
来源：http://sy.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://xa.hnjuh.cn

PHP:  public / protected / private
来源：http://rl.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://gx.szsharing.cn

TS:   public / protected / private
来源：http://ha.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://xq.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zc.chemitech.net.cn

Ruby: public / protected / private
来源：http://eq.shxzukj.cn

C#:   public / protected / private / internal
来源：http://sz.bookmarksfly.cn

[G11] getter / setter
来源：http://vn.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://qn.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vj.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gq.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://dg.hahajie.cn

Java: public String getName() { return name; }
来源：http://ic.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://re.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://pz.9csxet.cn

C#:   public string Name { get; set; }
来源：http://rg.shtwfgs.cn

[G12] 对象转字符串
来源：http://yt.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://dz.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tw.nszjky.cn

JS:   toString() { return this.name; }
来源：http://wi.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://sa.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://yg.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bs.hahajie.cn

Ruby: def to_s; @name; end
来源：http://dd.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://eo.newstarts.cn

[G13] 判断对象类型
来源：http://xe.asd995.cn

Py:   isinstance(u, User)
来源：http://yj.wgjwhj.cn

PHP:  $u instanceof User
来源：http://vc.shxzskj.cn

JS:   u instanceof User
来源：http://vv.hnjuh.cn

TS:   u instanceof User
来源：http://yb.wgjwhj.cn

Java: u instanceof User
来源：http://qz.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jm.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://uf.huixiangedu.cn

C#:   u is User
来源：http://fl.9csxet.cn

[G14] 数据类 / record
来源：http://zv.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://up.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://zu.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://id.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://db.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://ly.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://rs.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qp.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://md.huanxung.cn

[G15] 枚举
来源：http://ap.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gn.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tu.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uv.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://to.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://fv.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oa.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://eq.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hi.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://up.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ss.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://pd.nicolike.cn

JS:   Object.entries(obj)
来源：http://kb.521024.cn

TS:   Object.entries(obj)
来源：http://jb.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gi.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://st.panjiajie.cn

Ruby: obj.instance_variables
来源：http://ue.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://xj.bookmarksfly.cn

================================================================================
来源：http://im.hnjuh.cn

H. 异常与错误处理
来源：http://zg.newstarts.cn

================================================================================
来源：http://lk.jctech888.com.cn

[H01] try / catch 基础
来源：http://cs.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://af.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://go.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sh.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://op.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uw.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rg.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ze.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ua.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://yv.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nz.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gi.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pi.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cm.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ee.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bx.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rr.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jt.bjjhwx.cn

[H03] 主动抛出异常
来源：http://gb.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://rq.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jm.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://ln.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://rg.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bb.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tr.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ze.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://po.lnxyls.cn

[H04] 自定义异常类型
来源：http://os.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://yc.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lc.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ee.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://pc.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ao.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://xn.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://so.haigaiapp.cn

[H05] 捕获特定类型
来源：http://zt.lnxyls.cn

Py:   except ValueError as e:
来源：http://gt.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fu.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://ny.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://km.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://mp.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ah.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://rw.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ga.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ze.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://qq.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vn.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tc.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ex.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vt.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ls.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://js.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://yf.gzmigu.cn

[H07] 断言
来源：http://xu.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ed.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://ip.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://gj.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://zr.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://xd.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rh.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tv.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://ww.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://ou.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://oo.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ag.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://vn.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://py.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gf.huanxung.cn

Go:   err.Error()
来源：http://iw.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://qn.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://mp.521024.cn

[H09] 带错误码的异常
来源：http://oz.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sz.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ht.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ez.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kw.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ry.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vc.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yf.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pg.521024.cn

[H10] 资源自动释放
来源：http://io.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ci.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aq.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://go.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lw.colortex.cn

Go:   defer f.Close()
来源：http://bz.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kn.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ly.521024.cn


<!-- 参考信息 -->