代发 wailian999

Ruby: s.lines
来源：http://wj.panjiajie.cn

C#:   s.Split('\n')
来源：http://za.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://ub.hnjuh.cn

Py:   if not s:
来源：http://kn.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nj.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gc.newstarts.cn

TS:   if (s === "") {}
来源：http://co.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://jr.colortex.cn

Go:   if s == "" {}
来源：http://kj.haigaiapp.cn

Ruby: if s.empty?
来源：http://ym.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vn.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://wr.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wb.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yh.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jt.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://po.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rx.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://re.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bl.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ta.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://yq.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://px.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wb.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eo.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vr.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vc.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nf.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://tm.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hw.shxzukj.cn

================================================================================
来源：http://qy.jianghongdianzi.cn

F. 文件与目录
来源：http://zw.521024.cn

================================================================================
来源：http://ux.panjiajie.cn

[F01] 读取整个文件
来源：http://gb.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kl.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://un.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ua.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jw.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ws.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vb.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://eh.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://jm.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://io.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://us.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ju.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wn.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cr.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wn.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gx.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zv.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bq.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://kf.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://td.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hf.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ui.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mb.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://la.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mf.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://el.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.hahajie.cn

[F04] 追加写入文件
来源：http://fp.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ad.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://td.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yv.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ym.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uq.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://za.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fz.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://ai.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vy.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://tn.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://fz.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://rh.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vj.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pv.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://xq.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://hc.haigaiapp.cn

[F06] 删除文件
来源：http://ip.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://zi.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://wj.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cx.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uv.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xs.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://ql.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ga.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://ex.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://is.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nx.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hn.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pr.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tf.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://im.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://th.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vo.jctech888.com.cn

[F08] 遍历目录
来源：http://xm.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bn.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uu.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://sd.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://us.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qp.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lp.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://yj.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://xg.huanxung.cn

[F09] 获取文件大小
来源：http://tr.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://wp.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://xc.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://tj.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://vo.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mi.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nr.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://az.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mc.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ru.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ea.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ek.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jv.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://rt.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ua.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sd.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ua.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pk.shxzukj.cn

[F11] 复制与移动文件
来源：http://uh.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vp.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gj.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oc.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vy.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dx.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ub.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ku.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pw.hahajie.cn

[F12] CSV 读写
来源：http://xa.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hl.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ew.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.yuexingan06.cn

TS:   // 同上
来源：http://dh.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://by.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://td.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://we.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ln.nszjky.cn

================================================================================
来源：http://me.jianghongdianzi.cn

G. 面向对象
来源：http://nq.muxihuayi.cn

================================================================================
来源：http://cy.wgjwhj.cn

[G01] 定义类
来源：http://mm.yuntaijiaju.cn

Py:   class User: pass
来源：http://uk.colortex.cn

PHP:  class User {}
来源：http://rr.huanxung.cn

JS:   class User {}
来源：http://qt.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://jl.shxzukj.cn

Java: class User {}
来源：http://zg.nicolike.cn

Go:   type User struct { Name string }
来源：http://az.newstarts.cn

Ruby: class User; end
来源：http://hx.jianghongdianzi.cn

C#:   class User {}
来源：http://fy.asd995.cn

[G02] 构造函数
来源：http://vb.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://bv.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://ti.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://go.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://lj.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://do.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://id.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://th.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://tg.huixiangedu.cn

[G03] 实例属性
来源：http://gk.shxzukj.cn

Py:   self.name = "x"
来源：http://tg.shxzskj.cn

PHP:  public string $name = "x";
来源：http://ie.nicolike.cn

JS:   this.name = "x";
来源：http://va.yuexingan06.cn

TS:   name: string = "x";
来源：http://np.yuntaijiaju.cn

Java: private String name;
来源：http://gz.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pn.nszjky.cn

Ruby: @name = "x"
来源：http://lz.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://xe.newstarts.cn

[G04] 定义方法
来源：http://se.nicolike.cn

Py:   def greet(self): return self.name
来源：http://pc.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gi.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://yn.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://to.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ip.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oc.shxzskj.cn

Ruby: def greet; @name; end
来源：http://xi.huanxung.cn

C#:   public string Greet() => Name;
来源：http://vf.shxzukj.cn

[G05] 继承
来源：http://el.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://pu.huanxung.cn

PHP:  class Admin extends User {}
来源：http://dp.lnxyls.cn

JS:   class Admin extends User {}
来源：http://dl.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://nj.chemitech.net.cn

Java: class Admin extends User {}
来源：http://fe.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qj.asd995.cn

Ruby: class Admin < User; end
来源：http://fc.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://in.wgjwhj.cn

[G06] 重写方法
来源：http://va.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://pu.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dy.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://qi.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://vo.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://an.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hy.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://xi.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://vh.asd995.cn

[G07] 调用父类方法
来源：http://ug.nicolike.cn

Py:   super().greet()
来源：http://ty.bjjhwx.cn

PHP:  parent::greet();
来源：http://ah.colortex.cn

JS:   super.greet();
来源：http://tj.jctech888.com.cn

TS:   super.greet();
来源：http://ak.hahajie.cn

Java: super.greet();
来源：http://jp.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cg.shtwfgs.cn

Ruby: super
来源：http://ei.521024.cn

C#:   base.Greet();
来源：http://is.lnxyls.cn

[G08] 静态方法与属性
来源：http://dv.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://le.panjiajie.cn

PHP:  public static function f() {}
来源：http://il.bookmarksfly.cn

JS:   static f() {}
来源：http://sq.9csxet.cn

TS:   static f(): void {}
来源：http://ih.colortex.cn

Java: static void f() {}
来源：http://uh.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://at.muxihuayi.cn

Ruby: def self.f; end
来源：http://ar.huixiangedu.cn

C#:   public static void F() {}
来源：http://vl.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://mr.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://sj.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iu.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kd.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://hm.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://kl.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://cn.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xk.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://kt.wgjwhj.cn

[G10] 访问控制
来源：http://kz.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://ip.9csxet.cn

PHP:  public / protected / private
来源：http://lc.huanxung.cn

JS:   #private 字段；其余公开
来源：http://di.9csxet.cn

TS:   public / protected / private
来源：http://zs.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://lx.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ku.haigaiapp.cn

Ruby: public / protected / private
来源：http://no.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://kk.gzmigu.cn

[G11] getter / setter
来源：http://ch.szsharing.cn

Py:   @property 与 @x.setter
来源：http://zz.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ie.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ez.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://zg.nicolike.cn

Java: public String getName() { return name; }
来源：http://lk.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kd.nicolike.cn

Ruby: attr_accessor :name
来源：http://rz.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://lx.panjiajie.cn

[G12] 对象转字符串
来源：http://fo.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://ot.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sr.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://cu.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ec.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://qk.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vl.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://fj.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://vo.yuexingan06.cn

[G13] 判断对象类型
来源：http://yv.521024.cn

Py:   isinstance(u, User)
来源：http://ef.shtwfgs.cn

PHP:  $u instanceof User
来源：http://xy.bookmarksfly.cn

JS:   u instanceof User
来源：http://ia.nicolike.cn

TS:   u instanceof User
来源：http://jo.hnjuh.cn

Java: u instanceof User
来源：http://xb.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pa.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://jm.wgjwhj.cn

C#:   u is User
来源：http://gg.nicolike.cn

[G14] 数据类 / record
来源：http://zj.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rw.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://au.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tw.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://wx.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://sd.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://ly.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gk.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://yi.shxzukj.cn

[G15] 枚举
来源：http://fe.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oa.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lk.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pc.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vg.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://hg.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vv.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ov.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vj.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://ex.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cq.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://kb.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://dg.panjiajie.cn

TS:   Object.entries(obj)
来源：http://hb.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ft.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hd.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://rt.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://dw.asd995.cn

================================================================================
来源：http://hx.szxytkj.cn

H. 异常与错误处理
来源：http://ur.haigaiapp.cn

================================================================================
来源：http://pv.szsharing.cn

[H01] try / catch 基础
来源：http://qt.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gv.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gx.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://we.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ss.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pf.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lb.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mc.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://li.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://xl.nicolike.cn


<!-- 参考信息 -->