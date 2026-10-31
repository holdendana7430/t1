代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gc.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://as.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wj.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ke.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sy.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zz.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://of.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iq.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://yd.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fb.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://em.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://fi.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://pm.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nn.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fm.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://qb.521024.cn

C#:   File.Exists("a.txt")
来源：http://pk.bookmarksfly.cn

[F06] 删除文件
来源：http://ka.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://ag.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://qk.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vh.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xe.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ty.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://tz.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://dl.colortex.cn

C#:   File.Delete("a.txt");
来源：http://qi.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://yw.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gw.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pu.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dq.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zt.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ah.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xn.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dm.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sj.shtwfgs.cn

[F08] 遍历目录
来源：http://ht.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tp.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pw.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://zh.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ub.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qi.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://su.colortex.cn

Ruby: Dir.children("dir")
来源：http://og.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://ub.szsharing.cn

[F09] 获取文件大小
来源：http://aa.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://tq.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://re.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://lt.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://je.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pa.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pz.nszjky.cn

Ruby: File.size("a.txt")
来源：http://km.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://tz.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kz.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ff.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xy.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ij.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://sd.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hq.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zl.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ev.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://in.nicolike.cn

[F11] 复制与移动文件
来源：http://jp.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lm.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wd.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ku.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fm.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mk.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fx.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rh.panjiajie.cn

[F12] CSV 读写
来源：http://ql.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sw.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://co.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ig.shxzukj.cn

TS:   // 同上
来源：http://yf.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ph.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aj.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vn.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nk.jctech888.com.cn

================================================================================
来源：http://fo.lnxyls.cn

G. 面向对象
来源：http://cj.muxihuayi.cn

================================================================================
来源：http://da.hahajie.cn

[G01] 定义类
来源：http://gx.muxihuayi.cn

Py:   class User: pass
来源：http://zt.szsharing.cn

PHP:  class User {}
来源：http://fk.szsharing.cn

JS:   class User {}
来源：http://mj.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://sj.bookmarksfly.cn

Java: class User {}
来源：http://ja.colortex.cn

Go:   type User struct { Name string }
来源：http://bc.nszjky.cn

Ruby: class User; end
来源：http://gz.shxzukj.cn

C#:   class User {}
来源：http://eh.shxzskj.cn

[G02] 构造函数
来源：http://vi.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://yk.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://nf.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://yp.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://mu.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://fb.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fe.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://te.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.huanxung.cn

[G03] 实例属性
来源：http://yj.bookmarksfly.cn

Py:   self.name = "x"
来源：http://ce.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://cf.shxzskj.cn

JS:   this.name = "x";
来源：http://ym.shxzukj.cn

TS:   name: string = "x";
来源：http://yk.muxihuayi.cn

Java: private String name;
来源：http://wh.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rp.muxihuayi.cn

Ruby: @name = "x"
来源：http://ki.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ee.szxytkj.cn

[G04] 定义方法
来源：http://qs.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://xq.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ew.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://na.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://pw.newstarts.cn

Java: String greet() { return name; }
来源：http://qa.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oq.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://em.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://lo.gzmigu.cn

[G05] 继承
来源：http://wv.asd995.cn

Py:   class Admin(User): pass
来源：http://vy.szsharing.cn

PHP:  class Admin extends User {}
来源：http://ov.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://al.asd995.cn

TS:   class Admin extends User {}
来源：http://mm.asd995.cn

Java: class Admin extends User {}
来源：http://qr.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qx.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://zz.szsharing.cn

C#:   class Admin : User {}
来源：http://sh.jianghongdianzi.cn

[G06] 重写方法
来源：http://wf.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://rx.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nj.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://wf.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://cu.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://yw.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nm.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://vw.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://xv.hnjuh.cn

[G07] 调用父类方法
来源：http://je.szsharing.cn

Py:   super().greet()
来源：http://es.colortex.cn

PHP:  parent::greet();
来源：http://yk.haigaiapp.cn

JS:   super.greet();
来源：http://vy.haigaiapp.cn

TS:   super.greet();
来源：http://sj.asd995.cn

Java: super.greet();
来源：http://rt.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sc.bookmarksfly.cn

Ruby: super
来源：http://nw.newstarts.cn

C#:   base.Greet();
来源：http://bl.bjjhwx.cn

[G08] 静态方法与属性
来源：http://hl.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sh.colortex.cn

PHP:  public static function f() {}
来源：http://zb.haigaiapp.cn

JS:   static f() {}
来源：http://ef.haigaiapp.cn

TS:   static f(): void {}
来源：http://bx.muxihuayi.cn

Java: static void f() {}
来源：http://ou.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ms.jctech888.com.cn

Ruby: def self.f; end
来源：http://mg.szsharing.cn

C#:   public static void F() {}
来源：http://xf.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://ak.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://uz.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ja.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bg.521024.cn

TS:   interface Shape { area(): number; }
来源：http://sw.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://tq.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://pp.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://np.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ja.9csxet.cn

[G10] 访问控制
来源：http://ak.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xt.9csxet.cn

PHP:  public / protected / private
来源：http://rd.colortex.cn

JS:   #private 字段；其余公开
来源：http://jv.shxzskj.cn

TS:   public / protected / private
来源：http://fm.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://af.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ow.gzmigu.cn

Ruby: public / protected / private
来源：http://jm.shxzskj.cn

C#:   public / protected / private / internal
来源：http://qo.9csxet.cn

[G11] getter / setter
来源：http://ot.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://hb.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tn.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://al.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://aj.shxzskj.cn

Java: public String getName() { return name; }
来源：http://kr.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cq.shxzskj.cn

Ruby: attr_accessor :name
来源：http://tl.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://di.huanxung.cn

[G12] 对象转字符串
来源：http://nh.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://hr.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sv.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://hq.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://ou.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://wm.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dr.nicolike.cn

Ruby: def to_s; @name; end
来源：http://ti.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ul.hnjuh.cn

[G13] 判断对象类型
来源：http://hn.szxytkj.cn

Py:   isinstance(u, User)
来源：http://yq.huixiangedu.cn

PHP:  $u instanceof User
来源：http://gb.newstarts.cn

JS:   u instanceof User
来源：http://zx.huixiangedu.cn

TS:   u instanceof User
来源：http://oj.jctech888.com.cn

Java: u instanceof User
来源：http://rq.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bm.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://rn.szxytkj.cn

C#:   u is User
来源：http://bw.panjiajie.cn

[G14] 数据类 / record
来源：http://qj.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bu.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://tf.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oo.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://cr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://tr.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://or.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sk.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://qq.panjiajie.cn

[G15] 枚举
来源：http://am.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lh.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vg.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vs.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ue.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://to.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ej.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://mn.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tp.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://jh.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qq.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://as.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://ia.9csxet.cn

TS:   Object.entries(obj)
来源：http://hp.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jt.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yu.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://uh.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://io.yuexingan06.cn

================================================================================
来源：http://fu.panjiajie.cn

H. 异常与错误处理
来源：http://wo.colortex.cn

================================================================================
来源：http://wh.colortex.cn

[H01] try / catch 基础
来源：http://nx.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ul.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kg.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://so.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qg.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mi.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ma.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ae.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iz.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://ia.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aa.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mo.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zm.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kg.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://at.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xe.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vc.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oh.nszjky.cn

[H03] 主动抛出异常
来源：http://ea.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://nr.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rg.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://xt.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://gx.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rj.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rc.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lc.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bx.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ad.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://nb.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://co.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://dq.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://my.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://li.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sz.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://fi.huanxung.cn

C#:   class MyException : Exception {}
来源：http://im.bjjhwx.cn

[H05] 捕获特定类型
来源：http://bz.huanxung.cn

Py:   except ValueError as e:
来源：http://uf.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ly.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://cl.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://sk.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ft.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ak.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://tt.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jv.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://fs.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://on.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bf.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fc.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zw.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hq.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://il.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://gw.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://jf.nicolike.cn

[H07] 断言
来源：http://jl.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://oh.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://gb.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://tx.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://hw.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://xp.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zd.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://um.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://kf.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://xi.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://ay.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nt.nicolike.cn

JS:   e.message;  e.stack
来源：http://sb.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ll.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rx.szxytkj.cn

Go:   err.Error()
来源：http://tk.shtwfgs.cn


<!-- 参考信息 -->