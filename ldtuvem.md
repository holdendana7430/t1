代发 wailian999

[F01] 读取整个文件
来源：http://kk.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://op.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ff.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tr.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dc.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://it.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://no.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://wx.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://ci.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://dy.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zw.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mb.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hb.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yt.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dd.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qn.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rk.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aj.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ca.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eu.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kb.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eb.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xb.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dt.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ym.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://pq.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ui.colortex.cn

[F04] 追加写入文件
来源：http://vs.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ic.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zw.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qs.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oi.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vc.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mj.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wb.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eg.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://xs.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sb.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://ls.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://ln.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://fa.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gq.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rb.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://iv.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://uv.huixiangedu.cn

[F06] 删除文件
来源：http://it.9csxet.cn

Py:   os.remove("a.txt")
来源：http://fs.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://th.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xn.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://li.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fg.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ld.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://xa.521024.cn

C#:   File.Delete("a.txt");
来源：http://vr.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://ol.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ln.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ta.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tz.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jf.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gq.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nd.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qo.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zc.nszjky.cn

[F08] 遍历目录
来源：http://kg.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jl.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eo.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://vc.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://tz.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gl.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ax.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://dz.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://gg.nicolike.cn

[F09] 获取文件大小
来源：http://zx.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://ch.asd995.cn

PHP:  filesize("a.txt");
来源：http://dv.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://jy.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://lk.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cx.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dx.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://gc.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://dr.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://so.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ev.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wq.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jd.hahajie.cn

TS:   path.extname("a.txt")
来源：http://ed.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://te.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ap.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ok.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yi.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://dh.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pd.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ga.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kt.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ib.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kb.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://um.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dm.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ju.yuexingan06.cn

[F12] CSV 读写
来源：http://iv.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fd.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://es.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vf.newstarts.cn

TS:   // 同上
来源：http://sg.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vp.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xi.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ja.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nq.colortex.cn

================================================================================
来源：http://fh.chemitech.net.cn

G. 面向对象
来源：http://tk.hahajie.cn

================================================================================
来源：http://wv.hnjuh.cn

[G01] 定义类
来源：http://zz.huanxung.cn

Py:   class User: pass
来源：http://oa.huixiangedu.cn

PHP:  class User {}
来源：http://qa.wgjwhj.cn

JS:   class User {}
来源：http://re.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://it.colortex.cn

Java: class User {}
来源：http://dv.panjiajie.cn

Go:   type User struct { Name string }
来源：http://rx.hahajie.cn

Ruby: class User; end
来源：http://lp.colortex.cn

C#:   class User {}
来源：http://et.newstarts.cn

[G02] 构造函数
来源：http://gn.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://sw.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ig.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://hu.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://tz.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://du.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gq.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://lf.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://rv.muxihuayi.cn

[G03] 实例属性
来源：http://wl.shtwfgs.cn

Py:   self.name = "x"
来源：http://oe.gzmigu.cn

PHP:  public string $name = "x";
来源：http://hh.yuexingan06.cn

JS:   this.name = "x";
来源：http://an.521024.cn

TS:   name: string = "x";
来源：http://xn.hahajie.cn

Java: private String name;
来源：http://ub.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vh.yuexingan06.cn

Ruby: @name = "x"
来源：http://tb.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://wv.panjiajie.cn

[G04] 定义方法
来源：http://mq.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://zx.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rz.9csxet.cn

JS:   greet() { return this.name; }
来源：http://bw.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://lk.nicolike.cn

Java: String greet() { return name; }
来源：http://bh.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ip.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://tl.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://uu.huixiangedu.cn

[G05] 继承
来源：http://yf.hnjuh.cn

Py:   class Admin(User): pass
来源：http://we.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://mk.shxzskj.cn

JS:   class Admin extends User {}
来源：http://ie.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://yt.hnjuh.cn

Java: class Admin extends User {}
来源：http://gk.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zi.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://gp.shxzukj.cn

C#:   class Admin : User {}
来源：http://kt.lnxyls.cn

[G06] 重写方法
来源：http://uv.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://mx.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rr.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://wv.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://wv.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://lx.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jm.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://qq.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://lo.chemitech.net.cn

[G07] 调用父类方法
来源：http://qg.newstarts.cn

Py:   super().greet()
来源：http://xi.chemitech.net.cn

PHP:  parent::greet();
来源：http://nl.bjjhwx.cn

JS:   super.greet();
来源：http://yp.hahajie.cn

TS:   super.greet();
来源：http://ge.newstarts.cn

Java: super.greet();
来源：http://vh.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xx.huixiangedu.cn

Ruby: super
来源：http://sr.huanxung.cn

C#:   base.Greet();
来源：http://rq.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://qo.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jq.lnxyls.cn

PHP:  public static function f() {}
来源：http://jn.szsharing.cn

JS:   static f() {}
来源：http://gq.yuexingan06.cn

TS:   static f(): void {}
来源：http://ze.gzmigu.cn

Java: static void f() {}
来源：http://hc.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zd.colortex.cn

Ruby: def self.f; end
来源：http://ym.jctech888.com.cn

C#:   public static void F() {}
来源：http://ky.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://ez.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://ez.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pc.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fn.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://jg.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://an.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://dc.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ov.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://rc.nicolike.cn

[G10] 访问控制
来源：http://jy.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://wf.bjjhwx.cn

PHP:  public / protected / private
来源：http://nu.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://gs.newstarts.cn

TS:   public / protected / private
来源：http://zb.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ge.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ns.521024.cn

Ruby: public / protected / private
来源：http://ou.szxytkj.cn

C#:   public / protected / private / internal
来源：http://lq.hnjuh.cn

[G11] getter / setter
来源：http://ol.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://jn.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yx.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xw.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://be.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://cy.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hf.panjiajie.cn

Ruby: attr_accessor :name
来源：http://vi.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://hx.lnxyls.cn

[G12] 对象转字符串
来源：http://hb.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://iv.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ve.nszjky.cn

JS:   toString() { return this.name; }
来源：http://sw.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://kx.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://gw.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qr.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ex.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://yo.nicolike.cn

[G13] 判断对象类型
来源：http://hj.asd995.cn

Py:   isinstance(u, User)
来源：http://hj.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://ij.szsharing.cn

JS:   u instanceof User
来源：http://iq.szxytkj.cn

TS:   u instanceof User
来源：http://xq.panjiajie.cn

Java: u instanceof User
来源：http://mh.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nw.nicolike.cn

Ruby: u.is_a?(User)
来源：http://dq.shxzukj.cn

C#:   u is User
来源：http://qe.newstarts.cn

[G14] 数据类 / record
来源：http://xr.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lx.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://gl.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vv.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://cs.hahajie.cn

Java: record User(String name, int age) {}
来源：http://kc.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://bj.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dh.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://lo.huixinmuqiang.cn

[G15] 枚举
来源：http://od.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zv.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uf.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bx.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lo.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://hu.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sc.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://gv.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pz.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://no.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kv.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://qs.shxzukj.cn

JS:   Object.entries(obj)
来源：http://pq.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://tt.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nl.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fc.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://fw.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://ur.jctech888.com.cn

================================================================================
来源：http://rs.huanxung.cn

H. 异常与错误处理
来源：http://zy.yuntaijiaju.cn

================================================================================
来源：http://hp.szxytkj.cn

[H01] try / catch 基础
来源：http://za.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://is.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nq.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xc.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rl.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vv.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fq.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://df.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zr.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ct.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gq.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oh.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fl.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kz.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ic.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ai.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pw.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mw.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://wt.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://zd.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aw.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://de.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://mx.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bf.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uk.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ed.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kx.shtwfgs.cn

[H04] 自定义异常类型
来源：http://tr.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://tl.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tc.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://pj.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://vq.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://fs.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lu.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://jm.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://im.asd995.cn

[H05] 捕获特定类型
来源：http://hb.yuexingan06.cn

Py:   except ValueError as e:
来源：http://rb.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pb.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://hn.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://mj.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://mo.colortex.cn


<!-- 参考信息 -->