代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zn.asd995.cn

================================================================================
来源：http://sm.haigaiapp.cn

F. 文件与目录
来源：http://re.colortex.cn

================================================================================
来源：http://fb.newstarts.cn

[F01] 读取整个文件
来源：http://ql.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ld.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://jn.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sn.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fq.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://up.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ry.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ve.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://uk.shxzskj.cn

[F02] 逐行读取文件
来源：http://de.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cz.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nh.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ww.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qy.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yc.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qg.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iv.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dh.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://xz.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uj.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gy.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://un.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fb.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gk.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://by.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://th.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://co.bjjhwx.cn

[F04] 追加写入文件
来源：http://bp.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gh.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hi.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dp.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://js.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ng.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iu.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qn.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zk.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://zs.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mu.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://ip.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://rk.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://cl.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pa.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://di.521024.cn

Ruby: File.exist?("a.txt")
来源：http://sh.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://iq.asd995.cn

[F06] 删除文件
来源：http://hc.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://pd.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://pw.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ed.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iw.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vq.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://kb.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://jt.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://lk.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://jo.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qs.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xj.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://af.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ca.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rf.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pj.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rg.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://li.9csxet.cn

[F08] 遍历目录
来源：http://gz.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jt.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://si.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://yz.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://xq.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yh.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iz.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://nd.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://bb.lnxyls.cn

[F09] 获取文件大小
来源：http://ox.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://hy.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://cn.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://hf.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://pw.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wo.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gb.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://eb.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://qi.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://yk.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mu.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mh.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rl.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://ig.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fh.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gq.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dd.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ey.yuexingan06.cn

[F11] 复制与移动文件
来源：http://xj.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mq.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hx.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ov.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ap.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ra.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pi.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qj.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fo.huixinmuqiang.cn

[F12] CSV 读写
来源：http://vo.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bm.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qu.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nl.haigaiapp.cn

TS:   // 同上
来源：http://tt.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kn.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yu.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ho.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://er.muxihuayi.cn

================================================================================
来源：http://fg.hnjuh.cn

G. 面向对象
来源：http://qo.shxzskj.cn

================================================================================
来源：http://cz.jianghongdianzi.cn

[G01] 定义类
来源：http://tn.haigaiapp.cn

Py:   class User: pass
来源：http://mf.shtwfgs.cn

PHP:  class User {}
来源：http://sb.jctech888.com.cn

JS:   class User {}
来源：http://pi.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://jt.hnjuh.cn

Java: class User {}
来源：http://rp.asd995.cn

Go:   type User struct { Name string }
来源：http://ow.haigaiapp.cn

Ruby: class User; end
来源：http://uu.521024.cn

C#:   class User {}
来源：http://bs.yuexingan06.cn

[G02] 构造函数
来源：http://os.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://pl.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://nb.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://ga.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://uh.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://jw.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pe.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://et.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://bm.newstarts.cn

[G03] 实例属性
来源：http://am.nszjky.cn

Py:   self.name = "x"
来源：http://fz.shxzukj.cn

PHP:  public string $name = "x";
来源：http://mf.gzmigu.cn

JS:   this.name = "x";
来源：http://po.lnxyls.cn

TS:   name: string = "x";
来源：http://kc.bjjhwx.cn

Java: private String name;
来源：http://gk.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xg.shxzukj.cn

Ruby: @name = "x"
来源：http://nu.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://bw.nicolike.cn

[G04] 定义方法
来源：http://au.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://ca.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zu.huanxung.cn

JS:   greet() { return this.name; }
来源：http://pp.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://dk.hnjuh.cn

Java: String greet() { return name; }
来源：http://ax.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ff.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://cg.nszjky.cn

C#:   public string Greet() => Name;
来源：http://xq.shtwfgs.cn

[G05] 继承
来源：http://uf.newstarts.cn

Py:   class Admin(User): pass
来源：http://tz.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://pl.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://om.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://gb.szxytkj.cn

Java: class Admin extends User {}
来源：http://gx.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xp.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://ek.newstarts.cn

C#:   class Admin : User {}
来源：http://xr.szsharing.cn

[G06] 重写方法
来源：http://ry.asd995.cn

Py:   def greet(self): return "admin"
来源：http://rf.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wo.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://fe.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://wq.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://ve.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wi.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://mw.521024.cn

C#:   public override string Greet() => "admin";
来源：http://fn.szxytkj.cn

[G07] 调用父类方法
来源：http://yi.newstarts.cn

Py:   super().greet()
来源：http://hq.shxzukj.cn

PHP:  parent::greet();
来源：http://es.yuntaijiaju.cn

JS:   super.greet();
来源：http://kk.muxihuayi.cn

TS:   super.greet();
来源：http://nu.huixinmuqiang.cn

Java: super.greet();
来源：http://id.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dj.colortex.cn

Ruby: super
来源：http://yv.muxihuayi.cn

C#:   base.Greet();
来源：http://av.jctech888.com.cn

[G08] 静态方法与属性
来源：http://ah.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://um.wgjwhj.cn

PHP:  public static function f() {}
来源：http://op.jctech888.com.cn

JS:   static f() {}
来源：http://gg.9csxet.cn

TS:   static f(): void {}
来源：http://xw.hnjuh.cn

Java: static void f() {}
来源：http://dq.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://te.hahajie.cn

Ruby: def self.f; end
来源：http://ng.yuexingan06.cn

C#:   public static void F() {}
来源：http://br.9csxet.cn

[G09] 接口 / 抽象类
来源：http://uq.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://ga.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ts.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hi.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://in.nszjky.cn

Java: interface Shape { double area(); }
来源：http://ke.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://so.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fn.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://nz.shxzskj.cn

[G10] 访问控制
来源：http://xw.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://br.szsharing.cn

PHP:  public / protected / private
来源：http://zf.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://zn.hnjuh.cn

TS:   public / protected / private
来源：http://gz.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://jl.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rb.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://bo.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://gy.newstarts.cn

[G11] getter / setter
来源：http://kn.521024.cn

Py:   @property 与 @x.setter
来源：http://ag.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ly.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://ke.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://vb.szsharing.cn

Java: public String getName() { return name; }
来源：http://va.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fx.gzmigu.cn

Ruby: attr_accessor :name
来源：http://mk.colortex.cn

C#:   public string Name { get; set; }
来源：http://jl.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://tq.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://dw.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gr.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://id.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://pk.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://uy.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://od.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://ps.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://aq.panjiajie.cn

[G13] 判断对象类型
来源：http://rv.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://wx.panjiajie.cn

PHP:  $u instanceof User
来源：http://yp.hahajie.cn

JS:   u instanceof User
来源：http://ao.nszjky.cn

TS:   u instanceof User
来源：http://ph.huixiangedu.cn

Java: u instanceof User
来源：http://qc.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bj.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://gc.shxzukj.cn

C#:   u is User
来源：http://xz.muxihuayi.cn

[G14] 数据类 / record
来源：http://cj.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jx.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://zs.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ot.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://qc.521024.cn

Java: record User(String name, int age) {}
来源：http://vg.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://mx.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wj.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://lg.szsharing.cn

[G15] 枚举
来源：http://jx.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bu.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tm.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://we.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kx.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://zx.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://da.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://va.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qi.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://pa.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rx.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://lk.szxytkj.cn

JS:   Object.entries(obj)
来源：http://oc.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ub.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ga.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://su.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://rv.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://vm.nicolike.cn

================================================================================
来源：http://tt.hnjuh.cn

H. 异常与错误处理
来源：http://jk.haigaiapp.cn

================================================================================
来源：http://rv.shtwfgs.cn

[H01] try / catch 基础
来源：http://cb.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ic.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ri.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pc.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ok.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qi.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vq.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://df.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uk.szsharing.cn

[H02] finally / ensure 收尾
来源：http://en.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yr.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qf.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ov.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tx.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tg.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://su.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ds.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://td.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ov.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://pq.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yp.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://hh.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://ak.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ay.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://np.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sv.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cl.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://jm.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://hx.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ne.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://xr.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://jc.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://mw.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ge.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://tv.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://ot.shtwfgs.cn

[H05] 捕获特定类型
来源：http://ue.lnxyls.cn

Py:   except ValueError as e:
来源：http://iq.nszjky.cn


<!-- 参考信息 -->