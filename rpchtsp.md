代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rw.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ng.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uf.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ls.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://li.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ev.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://kg.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://eu.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://oi.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://si.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xc.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://mj.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://fs.huixiangedu.cn

[F06] 删除文件
来源：http://bo.nszjky.cn

Py:   os.remove("a.txt")
来源：http://rv.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://rl.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mq.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ef.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gu.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://dx.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://st.asd995.cn

C#:   File.Delete("a.txt");
来源：http://vs.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://kw.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qr.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xx.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://as.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ba.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xp.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qq.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fz.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zi.newstarts.cn

[F08] 遍历目录
来源：http://xs.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ku.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yn.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://hz.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://lf.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nb.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zb.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://jk.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://cp.jctech888.com.cn

[F09] 获取文件大小
来源：http://tm.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://zq.colortex.cn

PHP:  filesize("a.txt");
来源：http://cn.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://np.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://jp.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bs.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ma.9csxet.cn

Ruby: File.size("a.txt")
来源：http://ir.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://oo.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://te.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ol.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xt.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ac.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://am.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wt.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ul.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bm.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ur.lnxyls.cn

[F11] 复制与移动文件
来源：http://vt.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wh.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jo.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lv.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pc.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ru.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qv.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qf.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rb.jctech888.com.cn

[F12] CSV 读写
来源：http://an.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dz.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ax.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yz.colortex.cn

TS:   // 同上
来源：http://ha.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wp.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ha.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rx.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pe.gzmigu.cn

================================================================================
来源：http://dh.lnxyls.cn

G. 面向对象
来源：http://wo.gzmigu.cn

================================================================================
来源：http://ks.jctech888.com.cn

[G01] 定义类
来源：http://sf.gzmigu.cn

Py:   class User: pass
来源：http://xy.521024.cn

PHP:  class User {}
来源：http://lw.521024.cn

JS:   class User {}
来源：http://fx.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://bp.lnxyls.cn

Java: class User {}
来源：http://gt.szxytkj.cn

Go:   type User struct { Name string }
来源：http://cz.521024.cn

Ruby: class User; end
来源：http://fw.gzmigu.cn

C#:   class User {}
来源：http://dn.shxzskj.cn

[G02] 构造函数
来源：http://dj.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://vx.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://md.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://rz.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://wb.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://qy.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vg.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://rz.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://cb.panjiajie.cn

[G03] 实例属性
来源：http://yt.lnxyls.cn

Py:   self.name = "x"
来源：http://kn.panjiajie.cn

PHP:  public string $name = "x";
来源：http://sl.huixiangedu.cn

JS:   this.name = "x";
来源：http://dy.hnjuh.cn

TS:   name: string = "x";
来源：http://qz.yuexingan06.cn

Java: private String name;
来源：http://bb.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lc.colortex.cn

Ruby: @name = "x"
来源：http://fm.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ko.huixinmuqiang.cn

[G04] 定义方法
来源：http://gd.newstarts.cn

Py:   def greet(self): return self.name
来源：http://pq.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cw.hahajie.cn

JS:   greet() { return this.name; }
来源：http://bp.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://uq.muxihuayi.cn

Java: String greet() { return name; }
来源：http://cz.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gx.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://mk.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://ka.jianghongdianzi.cn

[G05] 继承
来源：http://zg.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://zl.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://vw.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://co.panjiajie.cn

TS:   class Admin extends User {}
来源：http://jl.colortex.cn

Java: class Admin extends User {}
来源：http://dz.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ua.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://br.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://kd.colortex.cn

[G06] 重写方法
来源：http://xr.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://vy.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://la.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://nk.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://cn.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://xm.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fr.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://gu.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://be.asd995.cn

[G07] 调用父类方法
来源：http://ll.gzmigu.cn

Py:   super().greet()
来源：http://kb.colortex.cn

PHP:  parent::greet();
来源：http://xj.szxytkj.cn

JS:   super.greet();
来源：http://ab.huixinmuqiang.cn

TS:   super.greet();
来源：http://xx.szsharing.cn

Java: super.greet();
来源：http://vh.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://za.hnjuh.cn

Ruby: super
来源：http://kw.jctech888.com.cn

C#:   base.Greet();
来源：http://pu.9csxet.cn

[G08] 静态方法与属性
来源：http://fr.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kz.huixiangedu.cn

PHP:  public static function f() {}
来源：http://xq.shxzukj.cn

JS:   static f() {}
来源：http://ko.haigaiapp.cn

TS:   static f(): void {}
来源：http://np.nszjky.cn

Java: static void f() {}
来源：http://mz.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jy.colortex.cn

Ruby: def self.f; end
来源：http://kx.bjjhwx.cn

C#:   public static void F() {}
来源：http://yp.hahajie.cn

[G09] 接口 / 抽象类
来源：http://yh.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://zj.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xv.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ij.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://rs.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://ug.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://pt.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tm.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://lf.shtwfgs.cn

[G10] 访问控制
来源：http://iy.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://lg.muxihuayi.cn

PHP:  public / protected / private
来源：http://ya.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://lc.szsharing.cn

TS:   public / protected / private
来源：http://ts.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://sm.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bx.szxytkj.cn

Ruby: public / protected / private
来源：http://mt.521024.cn

C#:   public / protected / private / internal
来源：http://wr.yuntaijiaju.cn

[G11] getter / setter
来源：http://yj.nszjky.cn

Py:   @property 与 @x.setter
来源：http://xi.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ep.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://ie.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://sa.panjiajie.cn

Java: public String getName() { return name; }
来源：http://sg.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mj.asd995.cn

Ruby: attr_accessor :name
来源：http://vt.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://yp.panjiajie.cn

[G12] 对象转字符串
来源：http://cb.colortex.cn

Py:   def __str__(self): return self.name
来源：http://mm.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bi.521024.cn

JS:   toString() { return this.name; }
来源：http://ub.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://jh.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://pv.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://os.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://yq.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://dd.newstarts.cn

[G13] 判断对象类型
来源：http://xl.lnxyls.cn

Py:   isinstance(u, User)
来源：http://px.lnxyls.cn

PHP:  $u instanceof User
来源：http://pd.wgjwhj.cn

JS:   u instanceof User
来源：http://qr.asd995.cn

TS:   u instanceof User
来源：http://sc.nszjky.cn

Java: u instanceof User
来源：http://ac.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mi.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://yo.gzmigu.cn

C#:   u is User
来源：http://gx.huixiangedu.cn

[G14] 数据类 / record
来源：http://kh.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wy.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://kx.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://di.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ru.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://us.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://di.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zv.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://kv.huixiangedu.cn

[G15] 枚举
来源：http://zo.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dz.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ws.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pd.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xr.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://dh.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gw.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://yt.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lq.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://wn.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dp.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ay.asd995.cn

JS:   Object.entries(obj)
来源：http://wq.colortex.cn

TS:   Object.entries(obj)
来源：http://az.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bz.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kb.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://kn.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://my.panjiajie.cn

================================================================================
来源：http://uc.chemitech.net.cn

H. 异常与错误处理
来源：http://an.lnxyls.cn

================================================================================
来源：http://bg.newstarts.cn

[H01] try / catch 基础
来源：http://qm.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kz.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hn.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yk.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pv.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ps.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rw.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ta.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nt.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vl.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xe.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oo.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lv.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cu.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tp.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tx.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zm.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wy.huixiangedu.cn

[H03] 主动抛出异常
来源：http://hn.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://om.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ou.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://zn.asd995.cn

TS:   throw new Error("错误信息");
来源：http://aq.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hn.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://og.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dx.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lv.hnjuh.cn

[H04] 自定义异常类型
来源：http://em.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://mc.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hi.szsharing.cn

JS:   class MyError extends Error {}
来源：http://nk.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://cw.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ou.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nt.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://jm.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://nn.newstarts.cn

[H05] 捕获特定类型
来源：http://ue.shxzskj.cn

Py:   except ValueError as e:
来源：http://ob.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zi.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://qi.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://yk.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://rd.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ii.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://dk.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yv.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ob.hahajie.cn

Py:   value = d.get("k") or default
来源：http://hk.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hi.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pi.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ty.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aw.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mw.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://vz.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://rx.newstarts.cn

[H07] 断言
来源：http://se.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://ux.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://ff.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://zj.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://rz.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://bx.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ui.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://az.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://lb.521024.cn

[H08] 获取错误信息与堆栈
来源：http://sv.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://fp.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fr.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ww.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jk.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://at.nicolike.cn

Go:   err.Error()
来源：http://ca.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://eq.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://fk.chemitech.net.cn

[H09] 带错误码的异常
来源：http://tr.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ki.shxzukj.cn


<!-- 参考信息 -->