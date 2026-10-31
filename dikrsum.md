代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wa.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lq.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://st.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wz.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ys.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ox.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ae.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nk.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ii.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hf.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rg.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uc.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ms.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://cl.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fe.jctech888.com.cn

[F04] 追加写入文件
来源：http://jz.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://up.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ws.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kh.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ib.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vi.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tb.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qz.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mc.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://di.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wm.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://tw.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://fs.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://dg.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bm.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fz.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://xx.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ic.521024.cn

[F06] 删除文件
来源：http://zy.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://li.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://ja.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mt.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rc.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ai.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://bj.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://zo.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://bk.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://sk.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://li.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ht.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xt.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tf.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tq.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mx.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pa.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://od.asd995.cn

[F08] 遍历目录
来源：http://ni.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rt.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pe.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://po.521024.cn

TS:   fs.readdirSync("dir")
来源：http://ql.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kb.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://px.hahajie.cn

Ruby: Dir.children("dir")
来源：http://qd.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://es.nicolike.cn

[F09] 获取文件大小
来源：http://ui.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://cz.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://no.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://um.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://lb.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rc.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wd.521024.cn

Ruby: File.size("a.txt")
来源：http://zy.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://qc.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://fa.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oc.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xd.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yn.nszjky.cn

TS:   path.extname("a.txt")
来源：http://na.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cc.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gh.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xz.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vo.hahajie.cn

[F11] 复制与移动文件
来源：http://vp.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yh.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ik.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gc.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pe.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dx.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zx.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ef.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xp.chemitech.net.cn

[F12] CSV 读写
来源：http://ml.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fo.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aj.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://it.nszjky.cn

TS:   // 同上
来源：http://ur.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xf.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pa.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kz.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kh.nszjky.cn

================================================================================
来源：http://bo.yuntaijiaju.cn

G. 面向对象
来源：http://ez.jianghongdianzi.cn

================================================================================
来源：http://vx.bjjhwx.cn

[G01] 定义类
来源：http://xd.shxzukj.cn

Py:   class User: pass
来源：http://ef.colortex.cn

PHP:  class User {}
来源：http://ib.gzmigu.cn

JS:   class User {}
来源：http://ha.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://id.chemitech.net.cn

Java: class User {}
来源：http://jd.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://yo.521024.cn

Ruby: class User; end
来源：http://wg.szxytkj.cn

C#:   class User {}
来源：http://jo.panjiajie.cn

[G02] 构造函数
来源：http://se.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://xr.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://vv.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://hj.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://xx.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://ay.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://so.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://az.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://pm.jctech888.com.cn

[G03] 实例属性
来源：http://pw.lnxyls.cn

Py:   self.name = "x"
来源：http://jf.lnxyls.cn

PHP:  public string $name = "x";
来源：http://gy.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ff.shxzukj.cn

TS:   name: string = "x";
来源：http://cr.jianghongdianzi.cn

Java: private String name;
来源：http://vj.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nf.bookmarksfly.cn

Ruby: @name = "x"
来源：http://hj.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://nw.chemitech.net.cn

[G04] 定义方法
来源：http://vg.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vn.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mw.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://fs.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://zv.521024.cn

Java: String greet() { return name; }
来源：http://jz.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zn.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://pv.newstarts.cn

C#:   public string Greet() => Name;
来源：http://fk.9csxet.cn

[G05] 继承
来源：http://ey.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://fm.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://yu.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://bx.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://le.nszjky.cn

Java: class Admin extends User {}
来源：http://ox.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vq.9csxet.cn

Ruby: class Admin < User; end
来源：http://ld.nicolike.cn

C#:   class Admin : User {}
来源：http://ae.lnxyls.cn

[G06] 重写方法
来源：http://fu.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://wv.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://td.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://xi.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://gz.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://zn.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rt.521024.cn

Ruby: def greet; "admin"; end
来源：http://uy.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://rq.nicolike.cn

[G07] 调用父类方法
来源：http://lh.9csxet.cn

Py:   super().greet()
来源：http://qy.shxzukj.cn

PHP:  parent::greet();
来源：http://mz.hnjuh.cn

JS:   super.greet();
来源：http://ke.521024.cn

TS:   super.greet();
来源：http://cs.wgjwhj.cn

Java: super.greet();
来源：http://xo.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ha.bjjhwx.cn

Ruby: super
来源：http://dc.lnxyls.cn

C#:   base.Greet();
来源：http://bg.shtwfgs.cn

[G08] 静态方法与属性
来源：http://yb.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zr.muxihuayi.cn

PHP:  public static function f() {}
来源：http://hy.huixiangedu.cn

JS:   static f() {}
来源：http://rc.nszjky.cn

TS:   static f(): void {}
来源：http://zx.hnjuh.cn

Java: static void f() {}
来源：http://yk.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oq.newstarts.cn

Ruby: def self.f; end
来源：http://cl.chemitech.net.cn

C#:   public static void F() {}
来源：http://jp.nicolike.cn

[G09] 接口 / 抽象类
来源：http://kv.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://az.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gn.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gz.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://rm.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ys.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://hq.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lj.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://is.gzmigu.cn

[G10] 访问控制
来源：http://gs.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://vv.jctech888.com.cn

PHP:  public / protected / private
来源：http://fs.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://bn.521024.cn

TS:   public / protected / private
来源：http://dl.521024.cn

Java: public / protected / private / 默认包级
来源：http://tt.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fj.huixiangedu.cn

Ruby: public / protected / private
来源：http://qh.hnjuh.cn

C#:   public / protected / private / internal
来源：http://gg.newstarts.cn

[G11] getter / setter
来源：http://pd.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://nf.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ro.9csxet.cn

JS:   get name() { return this._name; }
来源：http://jo.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ki.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://dr.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://av.shxzukj.cn

Ruby: attr_accessor :name
来源：http://jg.asd995.cn

C#:   public string Name { get; set; }
来源：http://mq.9csxet.cn

[G12] 对象转字符串
来源：http://zr.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://jn.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ex.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://zi.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://cy.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://kp.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tq.huanxung.cn

Ruby: def to_s; @name; end
来源：http://qf.colortex.cn

C#:   public override string ToString() => Name;
来源：http://sm.jctech888.com.cn

[G13] 判断对象类型
来源：http://ac.521024.cn

Py:   isinstance(u, User)
来源：http://hq.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ja.bjjhwx.cn

JS:   u instanceof User
来源：http://qg.gzmigu.cn

TS:   u instanceof User
来源：http://hh.newstarts.cn

Java: u instanceof User
来源：http://iu.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kg.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://oa.lnxyls.cn

C#:   u is User
来源：http://tc.nicolike.cn

[G14] 数据类 / record
来源：http://pc.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ni.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://mf.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ls.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://aw.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://zb.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ks.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wi.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://to.shxzukj.cn

[G15] 枚举
来源：http://br.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xs.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xe.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kq.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xy.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://dq.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cg.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://zq.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ql.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://pf.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aj.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://yr.9csxet.cn

JS:   Object.entries(obj)
来源：http://ph.9csxet.cn

TS:   Object.entries(obj)
来源：http://vd.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://re.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mq.hahajie.cn

Ruby: obj.instance_variables
来源：http://yx.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://eo.lnxyls.cn

================================================================================
来源：http://fg.asd995.cn

H. 异常与错误处理
来源：http://zj.huanxung.cn

================================================================================
来源：http://od.521024.cn

[H01] try / catch 基础
来源：http://xg.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tg.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://no.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lk.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ph.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ga.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kg.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lw.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yq.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://fj.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mn.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dd.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xo.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bd.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://up.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wk.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vf.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pu.panjiajie.cn

[H03] 主动抛出异常
来源：http://td.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://or.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ho.asd995.cn

JS:   throw new Error("错误信息");
来源：http://sd.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://wu.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ag.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tp.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xb.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ki.huixiangedu.cn

[H04] 自定义异常类型
来源：http://wo.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://cd.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tt.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://yf.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://cw.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://zt.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ql.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://vj.colortex.cn

C#:   class MyException : Exception {}
来源：http://sy.chemitech.net.cn

[H05] 捕获特定类型
来源：http://lh.szxytkj.cn

Py:   except ValueError as e:
来源：http://zb.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mo.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ho.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vi.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://zl.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xb.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://ac.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pd.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://xh.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://ku.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bx.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nk.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://by.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ak.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gu.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://jm.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://gh.asd995.cn


<!-- 参考信息 -->