代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://kz.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qn.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ee.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://dv.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://ns.szxytkj.cn

[F06] 删除文件
来源：http://rg.nicolike.cn

Py:   os.remove("a.txt")
来源：http://os.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://ig.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yw.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://el.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kg.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://eu.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://mn.colortex.cn

C#:   File.Delete("a.txt");
来源：http://qi.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://il.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sz.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://un.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mn.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ry.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://um.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ig.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zu.lnxyls.cn

[F08] 遍历目录
来源：http://ta.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cy.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pi.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://ta.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://hq.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://si.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nu.nicolike.cn

Ruby: Dir.children("dir")
来源：http://de.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://th.jctech888.com.cn

[F09] 获取文件大小
来源：http://kq.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://kg.asd995.cn

PHP:  filesize("a.txt");
来源：http://gu.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://cv.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ty.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qz.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://px.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://rd.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://rl.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://ni.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xs.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zx.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gz.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://zm.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ik.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zb.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rd.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kk.hahajie.cn

[F11] 复制与移动文件
来源：http://xb.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gq.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rv.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pu.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nm.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tm.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xv.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://px.asd995.cn

[F12] CSV 读写
来源：http://pe.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yy.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wq.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sp.jctech888.com.cn

TS:   // 同上
来源：http://dz.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xh.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zv.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ma.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dj.yuexingan06.cn

================================================================================
来源：http://lg.colortex.cn

G. 面向对象
来源：http://nh.colortex.cn

================================================================================
来源：http://fu.9csxet.cn

[G01] 定义类
来源：http://jw.panjiajie.cn

Py:   class User: pass
来源：http://iv.chemitech.net.cn

PHP:  class User {}
来源：http://az.gzmigu.cn

JS:   class User {}
来源：http://av.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://oy.szsharing.cn

Java: class User {}
来源：http://vy.nicolike.cn

Go:   type User struct { Name string }
来源：http://fs.chemitech.net.cn

Ruby: class User; end
来源：http://ht.shxzukj.cn

C#:   class User {}
来源：http://ut.newstarts.cn

[G02] 构造函数
来源：http://nj.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://lm.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://mo.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://wh.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://by.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://ja.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ok.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://zh.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://cd.colortex.cn

[G03] 实例属性
来源：http://tk.wgjwhj.cn

Py:   self.name = "x"
来源：http://jo.nszjky.cn

PHP:  public string $name = "x";
来源：http://uh.nszjky.cn

JS:   this.name = "x";
来源：http://hk.colortex.cn

TS:   name: string = "x";
来源：http://so.huanxung.cn

Java: private String name;
来源：http://vp.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gi.newstarts.cn

Ruby: @name = "x"
来源：http://qx.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://hq.lnxyls.cn

[G04] 定义方法
来源：http://uc.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://aw.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kb.newstarts.cn

JS:   greet() { return this.name; }
来源：http://ll.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://yx.panjiajie.cn

Java: String greet() { return name; }
来源：http://rr.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pm.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://vc.nicolike.cn

C#:   public string Greet() => Name;
来源：http://nt.9csxet.cn

[G05] 继承
来源：http://jj.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://eg.9csxet.cn

PHP:  class Admin extends User {}
来源：http://dq.lnxyls.cn

JS:   class Admin extends User {}
来源：http://lp.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://tj.hahajie.cn

Java: class Admin extends User {}
来源：http://hx.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bv.nszjky.cn

Ruby: class Admin < User; end
来源：http://rv.hahajie.cn

C#:   class Admin : User {}
来源：http://yy.shxzskj.cn

[G06] 重写方法
来源：http://yu.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://vl.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xi.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://ss.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ls.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://dm.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pq.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://zg.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://fw.lnxyls.cn

[G07] 调用父类方法
来源：http://pa.nszjky.cn

Py:   super().greet()
来源：http://zp.chemitech.net.cn

PHP:  parent::greet();
来源：http://dr.szxytkj.cn

JS:   super.greet();
来源：http://oz.colortex.cn

TS:   super.greet();
来源：http://kv.9csxet.cn

Java: super.greet();
来源：http://vg.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qv.chemitech.net.cn

Ruby: super
来源：http://yn.jianghongdianzi.cn

C#:   base.Greet();
来源：http://pt.asd995.cn

[G08] 静态方法与属性
来源：http://af.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nq.muxihuayi.cn

PHP:  public static function f() {}
来源：http://zz.yuntaijiaju.cn

JS:   static f() {}
来源：http://gt.bjjhwx.cn

TS:   static f(): void {}
来源：http://uf.nszjky.cn

Java: static void f() {}
来源：http://it.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nh.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://te.521024.cn

C#:   public static void F() {}
来源：http://wi.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://wg.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://mj.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ir.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eq.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://ij.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://in.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://nl.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kw.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://kr.shxzukj.cn

[G10] 访问控制
来源：http://pz.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://ib.nicolike.cn

PHP:  public / protected / private
来源：http://gc.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://fw.huixiangedu.cn

TS:   public / protected / private
来源：http://wk.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://bz.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nx.nicolike.cn

Ruby: public / protected / private
来源：http://bl.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://qk.chemitech.net.cn

[G11] getter / setter
来源：http://ry.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://km.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wm.newstarts.cn

JS:   get name() { return this._name; }
来源：http://ho.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://wm.shxzskj.cn

Java: public String getName() { return name; }
来源：http://nx.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eo.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ck.521024.cn

C#:   public string Name { get; set; }
来源：http://rx.szxytkj.cn

[G12] 对象转字符串
来源：http://bv.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://rv.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ja.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://wv.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://vu.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://fh.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lt.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ru.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://df.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://yf.shxzskj.cn

Py:   isinstance(u, User)
来源：http://hl.yuexingan06.cn

PHP:  $u instanceof User
来源：http://wc.9csxet.cn

JS:   u instanceof User
来源：http://gq.jianghongdianzi.cn

TS:   u instanceof User
来源：http://xx.huanxung.cn

Java: u instanceof User
来源：http://lu.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nj.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://jf.szxytkj.cn

C#:   u is User
来源：http://dr.wgjwhj.cn

[G14] 数据类 / record
来源：http://bo.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ty.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://aa.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vn.521024.cn

TS:   type User = { name: string; age: number };
来源：http://ne.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://rs.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://gn.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://is.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://hk.yuexingan06.cn

[G15] 枚举
来源：http://qn.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wn.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lw.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kj.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dm.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://yk.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ax.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://uw.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cf.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://nl.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ws.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://ox.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://zt.521024.cn

TS:   Object.entries(obj)
来源：http://qi.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wv.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wz.nszjky.cn

Ruby: obj.instance_variables
来源：http://qo.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://az.panjiajie.cn

================================================================================
来源：http://xc.newstarts.cn

H. 异常与错误处理
来源：http://gh.hahajie.cn

================================================================================
来源：http://bw.jctech888.com.cn

[H01] try / catch 基础
来源：http://gy.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://so.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ty.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zy.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://er.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wh.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yq.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://po.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dp.huanxung.cn

[H02] finally / ensure 收尾
来源：http://xe.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dp.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cq.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wk.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ur.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qh.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ap.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qs.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://le.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://vj.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://jz.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://un.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://zi.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://yp.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xd.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ts.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ep.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gq.hnjuh.cn

[H04] 自定义异常类型
来源：http://hp.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://th.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wq.521024.cn

JS:   class MyError extends Error {}
来源：http://qc.hahajie.cn

TS:   class MyError extends Error {}
来源：http://xo.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ys.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://os.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://dc.nszjky.cn

C#:   class MyException : Exception {}
来源：http://hj.panjiajie.cn

[H05] 捕获特定类型
来源：http://ll.nszjky.cn

Py:   except ValueError as e:
来源：http://rg.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ym.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://rc.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://gd.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://vf.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xj.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://zq.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zc.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://nu.asd995.cn

Py:   value = d.get("k") or default
来源：http://vt.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ty.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://od.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ap.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hb.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sp.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://jc.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://um.bjjhwx.cn

[H07] 断言
来源：http://rf.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://cj.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://og.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ko.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://cy.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://mr.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ex.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sp.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://du.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://rd.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://jj.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dy.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://hl.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kq.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wl.huanxung.cn

Go:   err.Error()
来源：http://vb.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://gr.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://gq.shxzukj.cn

[H09] 带错误码的异常
来源：http://uw.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gz.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wc.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kh.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sj.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xk.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wq.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sc.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fm.bjjhwx.cn

[H10] 资源自动释放
来源：http://kv.shtwfgs.cn


<!-- 参考信息 -->