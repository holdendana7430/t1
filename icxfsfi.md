代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://zg.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cw.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://an.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://af.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://kr.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qs.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gr.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://wp.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ia.hahajie.cn

[F06] 删除文件
来源：http://tv.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://sk.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://xv.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gv.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nt.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ey.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://wc.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://xa.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ur.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://yk.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rj.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qy.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yz.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://os.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cq.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ql.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://no.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qv.colortex.cn

[F08] 遍历目录
来源：http://wd.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qz.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mw.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://qs.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://pq.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dz.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dw.nszjky.cn

Ruby: Dir.children("dir")
来源：http://ec.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://qk.521024.cn

[F09] 获取文件大小
来源：http://fo.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://ml.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://dp.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://xc.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://iv.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hn.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iq.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ph.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ji.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://dk.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ix.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ou.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ff.szsharing.cn

TS:   path.extname("a.txt")
来源：http://wr.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vl.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uv.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dx.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uw.chemitech.net.cn

[F11] 复制与移动文件
来源：http://da.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bc.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://go.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uc.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oe.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://go.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fo.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lr.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vy.yuexingan06.cn

[F12] CSV 读写
来源：http://sr.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gj.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hc.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qb.hahajie.cn

TS:   // 同上
来源：http://yl.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wo.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nn.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cd.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://gn.bookmarksfly.cn

G. 面向对象
来源：http://sf.jctech888.com.cn

================================================================================
来源：http://gs.asd995.cn

[G01] 定义类
来源：http://eb.9csxet.cn

Py:   class User: pass
来源：http://av.lnxyls.cn

PHP:  class User {}
来源：http://cm.muxihuayi.cn

JS:   class User {}
来源：http://ti.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://wp.huixiangedu.cn

Java: class User {}
来源：http://ap.521024.cn

Go:   type User struct { Name string }
来源：http://ss.shxzukj.cn

Ruby: class User; end
来源：http://ca.yuntaijiaju.cn

C#:   class User {}
来源：http://dl.newstarts.cn

[G02] 构造函数
来源：http://zc.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://tt.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://is.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://sl.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://ax.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://ps.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oz.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://zb.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://qu.chemitech.net.cn

[G03] 实例属性
来源：http://gq.hnjuh.cn

Py:   self.name = "x"
来源：http://eh.szsharing.cn

PHP:  public string $name = "x";
来源：http://yd.asd995.cn

JS:   this.name = "x";
来源：http://lk.bookmarksfly.cn

TS:   name: string = "x";
来源：http://fh.hahajie.cn

Java: private String name;
来源：http://ju.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pp.shxzskj.cn

Ruby: @name = "x"
来源：http://kc.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://so.huixiangedu.cn

[G04] 定义方法
来源：http://rd.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://uz.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dw.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://ts.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://dv.nszjky.cn

Java: String greet() { return name; }
来源：http://yj.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bd.colortex.cn

Ruby: def greet; @name; end
来源：http://lx.521024.cn

C#:   public string Greet() => Name;
来源：http://wf.lnxyls.cn

[G05] 继承
来源：http://pe.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://fy.colortex.cn

PHP:  class Admin extends User {}
来源：http://al.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://rn.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://dq.yuexingan06.cn

Java: class Admin extends User {}
来源：http://xe.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ck.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://na.szsharing.cn

C#:   class Admin : User {}
来源：http://zf.shtwfgs.cn

[G06] 重写方法
来源：http://la.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://fs.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yp.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://mc.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://cq.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://sh.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ca.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ak.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://bp.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://oi.nicolike.cn

Py:   super().greet()
来源：http://mw.huanxung.cn

PHP:  parent::greet();
来源：http://lz.gzmigu.cn

JS:   super.greet();
来源：http://ye.hahajie.cn

TS:   super.greet();
来源：http://nk.gzmigu.cn

Java: super.greet();
来源：http://ro.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lg.asd995.cn

Ruby: super
来源：http://qe.nicolike.cn

C#:   base.Greet();
来源：http://pd.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://jl.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://su.haigaiapp.cn

PHP:  public static function f() {}
来源：http://vq.jianghongdianzi.cn

JS:   static f() {}
来源：http://av.jctech888.com.cn

TS:   static f(): void {}
来源：http://nk.shtwfgs.cn

Java: static void f() {}
来源：http://ot.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kq.chemitech.net.cn

Ruby: def self.f; end
来源：http://ef.huixiangedu.cn

C#:   public static void F() {}
来源：http://lo.nszjky.cn

[G09] 接口 / 抽象类
来源：http://jr.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://as.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iz.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gy.521024.cn

TS:   interface Shape { area(): number; }
来源：http://fv.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://bt.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ip.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qz.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://ie.wgjwhj.cn

[G10] 访问控制
来源：http://tw.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://zi.shxzskj.cn

PHP:  public / protected / private
来源：http://if.szsharing.cn

JS:   #private 字段；其余公开
来源：http://qo.colortex.cn

TS:   public / protected / private
来源：http://sb.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://qc.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fu.9csxet.cn

Ruby: public / protected / private
来源：http://hk.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://wh.nicolike.cn

[G11] getter / setter
来源：http://bc.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ql.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cr.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://gj.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://vv.9csxet.cn

Java: public String getName() { return name; }
来源：http://oc.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://to.huanxung.cn

Ruby: attr_accessor :name
来源：http://nq.nicolike.cn

C#:   public string Name { get; set; }
来源：http://df.521024.cn

[G12] 对象转字符串
来源：http://qi.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://iw.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qs.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://wd.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://dq.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://gt.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pk.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://lz.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://af.panjiajie.cn

[G13] 判断对象类型
来源：http://av.hnjuh.cn

Py:   isinstance(u, User)
来源：http://ge.lnxyls.cn

PHP:  $u instanceof User
来源：http://rh.haigaiapp.cn

JS:   u instanceof User
来源：http://vl.huixinmuqiang.cn

TS:   u instanceof User
来源：http://pb.hnjuh.cn

Java: u instanceof User
来源：http://fw.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mg.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://bz.yuexingan06.cn

C#:   u is User
来源：http://ll.chemitech.net.cn

[G14] 数据类 / record
来源：http://wv.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yz.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://xr.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pd.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://kq.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://gc.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ns.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pj.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://nm.yuexingan06.cn

[G15] 枚举
来源：http://ia.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xf.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ht.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ep.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ew.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://vo.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mr.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://ah.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://we.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://lm.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hl.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://nx.newstarts.cn

JS:   Object.entries(obj)
来源：http://ce.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://hw.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mu.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bq.nicolike.cn

Ruby: obj.instance_variables
来源：http://eq.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://ct.hnjuh.cn

================================================================================
来源：http://ic.lnxyls.cn

H. 异常与错误处理
来源：http://uh.bjjhwx.cn

================================================================================
来源：http://wj.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://wy.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jq.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xc.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://az.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lm.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bd.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bz.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://if.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pb.asd995.cn

[H02] finally / ensure 收尾
来源：http://jq.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ec.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dx.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://in.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://av.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zc.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zi.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wd.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zd.asd995.cn

[H03] 主动抛出异常
来源：http://oz.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://ea.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://og.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://ft.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://ai.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cx.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ss.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pw.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://si.9csxet.cn

[H04] 自定义异常类型
来源：http://vv.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://vv.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tr.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://dz.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://cw.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://fv.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ay.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://zh.huanxung.cn

C#:   class MyException : Exception {}
来源：http://aq.bjjhwx.cn

[H05] 捕获特定类型
来源：http://tv.haigaiapp.cn

Py:   except ValueError as e:
来源：http://or.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vr.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://uz.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://wt.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qh.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://je.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://hn.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vk.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://qf.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://ne.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gu.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tq.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jq.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kt.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sb.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ii.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://om.wgjwhj.cn

[H07] 断言
来源：http://jh.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://ms.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://dq.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://lt.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://aj.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://yg.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://it.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mp.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://xs.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://xi.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://dz.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dw.nicolike.cn

JS:   e.message;  e.stack
来源：http://uc.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dk.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sz.haigaiapp.cn

Go:   err.Error()
来源：http://co.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://vc.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://tr.szsharing.cn

[H09] 带错误码的异常
来源：http://ue.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xn.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ek.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zh.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gu.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vb.huixiangedu.cn


<!-- 参考信息 -->