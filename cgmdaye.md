代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://tl.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://wi.yuexingan06.cn

Java: s.lines().toList()
来源：http://jg.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://hf.shtwfgs.cn

Ruby: s.lines
来源：http://zb.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ql.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://vn.hahajie.cn

Py:   if not s:
来源：http://nq.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hk.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yx.asd995.cn

TS:   if (s === "") {}
来源：http://kl.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://vr.bookmarksfly.cn

Go:   if s == "" {}
来源：http://zo.nszjky.cn

Ruby: if s.empty?
来源：http://lj.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://um.panjiajie.cn

[E21] 超长截断加省略号
来源：http://uc.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uy.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dw.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ir.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ja.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://md.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://hh.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eg.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cd.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://if.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ql.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nt.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pa.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hc.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fd.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://ui.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hc.hnjuh.cn

================================================================================
来源：http://lw.haigaiapp.cn

F. 文件与目录
来源：http://oo.hahajie.cn

================================================================================
来源：http://ba.shxzukj.cn

[F01] 读取整个文件
来源：http://rq.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qc.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://wr.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://no.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pc.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ek.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qk.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ot.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://th.newstarts.cn

[F02] 逐行读取文件
来源：http://zx.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ev.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qy.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gh.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hf.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nm.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kp.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://so.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fx.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://sh.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ta.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pr.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wv.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pa.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ni.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ep.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://gi.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://my.shxzukj.cn

[F04] 追加写入文件
来源：http://tr.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vx.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hc.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jm.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ur.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mt.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bi.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wx.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://so.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://hr.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dg.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://du.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://ww.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://bh.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://br.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://er.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://xj.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://fu.szsharing.cn

[F06] 删除文件
来源：http://uq.9csxet.cn

Py:   os.remove("a.txt")
来源：http://yk.nszjky.cn

PHP:  unlink("a.txt");
来源：http://fl.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iv.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hb.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ys.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://rs.asd995.cn

Ruby: File.delete("a.txt")
来源：http://mr.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://iu.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://sw.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gq.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://id.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ec.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hw.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pd.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gg.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nk.szsharing.cn

[F08] 遍历目录
来源：http://dz.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://im.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://js.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://ej.521024.cn

TS:   fs.readdirSync("dir")
来源：http://hq.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rg.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dg.nicolike.cn

Ruby: Dir.children("dir")
来源：http://fe.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://ix.newstarts.cn

[F09] 获取文件大小
来源：http://gb.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://nh.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://kp.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://vw.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://tk.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cc.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qy.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://ye.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://dn.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ik.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lm.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kn.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tf.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://qy.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ll.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://de.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yr.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pd.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://uq.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xi.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ox.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qb.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vr.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fp.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tm.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yg.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xe.panjiajie.cn

[F12] CSV 读写
来源：http://yt.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sd.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hj.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ad.gzmigu.cn

TS:   // 同上
来源：http://az.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ry.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vy.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vk.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bx.chemitech.net.cn

================================================================================
来源：http://lz.colortex.cn

G. 面向对象
来源：http://ke.colortex.cn

================================================================================
来源：http://xr.bookmarksfly.cn

[G01] 定义类
来源：http://sd.nszjky.cn

Py:   class User: pass
来源：http://hb.huanxung.cn

PHP:  class User {}
来源：http://gk.hnjuh.cn

JS:   class User {}
来源：http://rf.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://qi.nszjky.cn

Java: class User {}
来源：http://sx.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://en.huanxung.cn

Ruby: class User; end
来源：http://fk.szsharing.cn

C#:   class User {}
来源：http://yv.521024.cn

[G02] 构造函数
来源：http://md.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://en.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://et.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://kh.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://lo.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://yb.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zn.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://fe.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://fc.panjiajie.cn

[G03] 实例属性
来源：http://fr.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://ko.nicolike.cn

PHP:  public string $name = "x";
来源：http://no.wgjwhj.cn

JS:   this.name = "x";
来源：http://bu.asd995.cn

TS:   name: string = "x";
来源：http://wu.jctech888.com.cn

Java: private String name;
来源：http://eb.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yq.gzmigu.cn

Ruby: @name = "x"
来源：http://os.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://rd.jctech888.com.cn

[G04] 定义方法
来源：http://hk.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://rx.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://am.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://qc.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ap.nicolike.cn

Java: String greet() { return name; }
来源：http://sa.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jv.521024.cn

Ruby: def greet; @name; end
来源：http://du.521024.cn

C#:   public string Greet() => Name;
来源：http://aa.yuexingan06.cn

[G05] 继承
来源：http://iu.asd995.cn

Py:   class Admin(User): pass
来源：http://qx.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://hr.lnxyls.cn

JS:   class Admin extends User {}
来源：http://yf.lnxyls.cn

TS:   class Admin extends User {}
来源：http://uo.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://hn.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ge.newstarts.cn

Ruby: class Admin < User; end
来源：http://gw.hnjuh.cn

C#:   class Admin : User {}
来源：http://qq.asd995.cn

[G06] 重写方法
来源：http://mq.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://cc.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ld.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://vc.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://ax.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://hw.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://id.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://hn.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://rc.haigaiapp.cn

[G07] 调用父类方法
来源：http://ni.yuexingan06.cn

Py:   super().greet()
来源：http://lh.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://yk.gzmigu.cn

JS:   super.greet();
来源：http://hu.huixiangedu.cn

TS:   super.greet();
来源：http://pj.shxzukj.cn

Java: super.greet();
来源：http://yv.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tn.haigaiapp.cn

Ruby: super
来源：http://cn.yuexingan06.cn

C#:   base.Greet();
来源：http://ya.jctech888.com.cn

[G08] 静态方法与属性
来源：http://zp.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://of.jctech888.com.cn

PHP:  public static function f() {}
来源：http://qp.muxihuayi.cn

JS:   static f() {}
来源：http://di.shxzukj.cn

TS:   static f(): void {}
来源：http://oo.nicolike.cn

Java: static void f() {}
来源：http://hp.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xa.colortex.cn

Ruby: def self.f; end
来源：http://ym.szxytkj.cn

C#:   public static void F() {}
来源：http://fv.colortex.cn

[G09] 接口 / 抽象类
来源：http://to.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://fw.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zm.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xk.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://is.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://hb.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://cf.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eq.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://mo.panjiajie.cn

[G10] 访问控制
来源：http://yt.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://fr.haigaiapp.cn

PHP:  public / protected / private
来源：http://ce.hahajie.cn

JS:   #private 字段；其余公开
来源：http://fn.jianghongdianzi.cn

TS:   public / protected / private
来源：http://wh.asd995.cn

Java: public / protected / private / 默认包级
来源：http://os.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ln.shxzukj.cn

Ruby: public / protected / private
来源：http://sm.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://zs.szxytkj.cn

[G11] getter / setter
来源：http://wc.colortex.cn

Py:   @property 与 @x.setter
来源：http://jm.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sj.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://wd.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://lj.panjiajie.cn

Java: public String getName() { return name; }
来源：http://ns.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://de.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://qj.asd995.cn

C#:   public string Name { get; set; }
来源：http://dw.bjjhwx.cn

[G12] 对象转字符串
来源：http://kj.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://pm.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rb.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://tn.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://vp.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://uu.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uv.huanxung.cn

Ruby: def to_s; @name; end
来源：http://cq.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://zj.bjjhwx.cn

[G13] 判断对象类型
来源：http://om.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://wt.gzmigu.cn

PHP:  $u instanceof User
来源：http://ow.lnxyls.cn

JS:   u instanceof User
来源：http://jx.haigaiapp.cn

TS:   u instanceof User
来源：http://kr.gzmigu.cn

Java: u instanceof User
来源：http://bp.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cd.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://nq.gzmigu.cn

C#:   u is User
来源：http://pj.huixiangedu.cn

[G14] 数据类 / record
来源：http://ym.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ax.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://az.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://he.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://tj.9csxet.cn

Java: record User(String name, int age) {}
来源：http://xy.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ey.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vw.asd995.cn

C#:   record User(string Name, int Age);
来源：http://gu.9csxet.cn

[G15] 枚举
来源：http://cw.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ie.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ja.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://la.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fe.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://zm.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pp.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://ev.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cb.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://ku.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bx.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://yg.szsharing.cn

JS:   Object.entries(obj)
来源：http://lo.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ow.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eu.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fy.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://um.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://dc.huixinmuqiang.cn

================================================================================
来源：http://cm.asd995.cn

H. 异常与错误处理
来源：http://zr.jianghongdianzi.cn

================================================================================
来源：http://ec.nszjky.cn

[H01] try / catch 基础
来源：http://mz.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ft.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vy.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rd.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kh.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://px.nicolike.cn


<!-- 参考信息 -->