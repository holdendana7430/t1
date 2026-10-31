代发 wailian999

Ruby: s.lines
来源：http://gw.haigaiapp.cn

C#:   s.Split('\n')
来源：http://rv.hahajie.cn

[E20] 判断字符串是否为空
来源：http://vt.muxihuayi.cn

Py:   if not s:
来源：http://om.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tl.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ck.szxytkj.cn

TS:   if (s === "") {}
来源：http://kt.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ng.521024.cn

Go:   if s == "" {}
来源：http://sw.shxzukj.cn

Ruby: if s.empty?
来源：http://kg.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ue.nicolike.cn

[E21] 超长截断加省略号
来源：http://wc.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cc.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yx.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lr.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ku.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://kx.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uv.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vd.szsharing.cn

[E22] 字节长度与字符长度
来源：http://tg.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://po.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lx.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sd.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ha.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cc.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://tz.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yn.huanxung.cn

================================================================================
来源：http://md.yuexingan06.cn

F. 文件与目录
来源：http://eu.panjiajie.cn

================================================================================
来源：http://cj.hnjuh.cn

[F01] 读取整个文件
来源：http://km.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ev.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://or.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bl.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cq.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qq.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://it.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://hk.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://wo.nicolike.cn

[F02] 逐行读取文件
来源：http://nc.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lg.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dj.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hi.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://po.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tp.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kf.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fo.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://kr.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mj.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ch.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ct.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dx.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ov.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ha.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://si.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vs.hahajie.cn

[F04] 追加写入文件
来源：http://jc.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://na.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ra.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zd.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qj.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bo.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bn.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yd.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ps.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://uo.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pb.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://yw.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://zt.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://fr.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mv.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vu.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ub.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://xi.9csxet.cn

[F06] 删除文件
来源：http://fh.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://sa.colortex.cn

PHP:  unlink("a.txt");
来源：http://yh.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ru.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://af.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fg.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://du.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://jp.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://us.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://lq.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yt.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://we.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iz.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lf.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fq.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://km.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qk.shtwfgs.cn

[F08] 遍历目录
来源：http://mi.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dc.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dg.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ba.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://qw.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xh.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yi.newstarts.cn

Ruby: Dir.children("dir")
来源：http://qy.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ua.panjiajie.cn

[F09] 获取文件大小
来源：http://mn.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://xi.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://bl.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://xa.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://cp.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yj.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vz.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://nk.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ri.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://hu.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ff.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fu.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lw.newstarts.cn

TS:   path.extname("a.txt")
来源：http://mz.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ge.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jm.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fa.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wg.panjiajie.cn

[F11] 复制与移动文件
来源：http://nv.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ld.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vx.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jp.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ij.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uh.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sh.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ws.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pc.huixinmuqiang.cn

[F12] CSV 读写
来源：http://bu.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ix.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jm.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gb.szxytkj.cn

TS:   // 同上
来源：http://tf.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pq.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eb.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ik.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bg.muxihuayi.cn

================================================================================
来源：http://it.wgjwhj.cn

G. 面向对象
来源：http://yr.huixiangedu.cn

================================================================================
来源：http://zt.hnjuh.cn

[G01] 定义类
来源：http://zp.colortex.cn

Py:   class User: pass
来源：http://jp.wgjwhj.cn

PHP:  class User {}
来源：http://vp.jctech888.com.cn

JS:   class User {}
来源：http://lj.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://vo.huixinmuqiang.cn

Java: class User {}
来源：http://nl.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://tu.newstarts.cn

Ruby: class User; end
来源：http://qi.shxzukj.cn

C#:   class User {}
来源：http://qn.muxihuayi.cn

[G02] 构造函数
来源：http://gl.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://fq.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://zg.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://zi.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ji.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://zz.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uc.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://tw.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://ao.yuexingan06.cn

[G03] 实例属性
来源：http://tl.panjiajie.cn

Py:   self.name = "x"
来源：http://jk.hahajie.cn

PHP:  public string $name = "x";
来源：http://vp.9csxet.cn

JS:   this.name = "x";
来源：http://vo.huixiangedu.cn

TS:   name: string = "x";
来源：http://gu.nszjky.cn

Java: private String name;
来源：http://up.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cq.bookmarksfly.cn

Ruby: @name = "x"
来源：http://cr.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://zg.yuexingan06.cn

[G04] 定义方法
来源：http://jm.newstarts.cn

Py:   def greet(self): return self.name
来源：http://wz.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kb.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://jg.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://tj.hnjuh.cn

Java: String greet() { return name; }
来源：http://af.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bi.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://nk.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://aw.colortex.cn

[G05] 继承
来源：http://zd.nszjky.cn

Py:   class Admin(User): pass
来源：http://hb.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://hz.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://wf.9csxet.cn

TS:   class Admin extends User {}
来源：http://xx.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://fp.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kz.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ei.szxytkj.cn

C#:   class Admin : User {}
来源：http://ja.szxytkj.cn

[G06] 重写方法
来源：http://jy.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://eu.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dt.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://vx.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://us.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://jd.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rv.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://zd.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://za.hnjuh.cn

[G07] 调用父类方法
来源：http://fl.yuexingan06.cn

Py:   super().greet()
来源：http://mp.9csxet.cn

PHP:  parent::greet();
来源：http://pl.nicolike.cn

JS:   super.greet();
来源：http://ok.wgjwhj.cn

TS:   super.greet();
来源：http://ve.shxzukj.cn

Java: super.greet();
来源：http://he.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hs.nicolike.cn

Ruby: super
来源：http://mi.muxihuayi.cn

C#:   base.Greet();
来源：http://sk.muxihuayi.cn

[G08] 静态方法与属性
来源：http://py.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jy.huixiangedu.cn

PHP:  public static function f() {}
来源：http://cs.huixiangedu.cn

JS:   static f() {}
来源：http://qu.huanxung.cn

TS:   static f(): void {}
来源：http://cj.jctech888.com.cn

Java: static void f() {}
来源：http://qz.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ym.hnjuh.cn

Ruby: def self.f; end
来源：http://by.wgjwhj.cn

C#:   public static void F() {}
来源：http://ak.nszjky.cn

[G09] 接口 / 抽象类
来源：http://pm.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://yj.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ay.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://up.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://vl.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://ei.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://cy.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qc.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://rj.gzmigu.cn

[G10] 访问控制
来源：http://yz.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://fj.szxytkj.cn

PHP:  public / protected / private
来源：http://xx.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://xc.huixiangedu.cn

TS:   public / protected / private
来源：http://gk.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://an.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yf.shxzukj.cn

Ruby: public / protected / private
来源：http://en.colortex.cn

C#:   public / protected / private / internal
来源：http://lf.huanxung.cn

[G11] getter / setter
来源：http://md.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://zx.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ve.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://fx.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://gd.521024.cn

Java: public String getName() { return name; }
来源：http://dd.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ln.lnxyls.cn

Ruby: attr_accessor :name
来源：http://dw.asd995.cn

C#:   public string Name { get; set; }
来源：http://rx.newstarts.cn

[G12] 对象转字符串
来源：http://wq.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://hl.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xh.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://me.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://ew.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://uc.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sk.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ws.521024.cn

C#:   public override string ToString() => Name;
来源：http://xd.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://rd.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://sm.muxihuayi.cn

PHP:  $u instanceof User
来源：http://fv.hnjuh.cn

JS:   u instanceof User
来源：http://hd.bjjhwx.cn

TS:   u instanceof User
来源：http://gy.szsharing.cn

Java: u instanceof User
来源：http://qj.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ou.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ls.haigaiapp.cn

C#:   u is User
来源：http://gv.hnjuh.cn

[G14] 数据类 / record
来源：http://yd.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yn.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://te.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sg.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://iy.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://uu.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://aw.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tg.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://oj.nicolike.cn

[G15] 枚举
来源：http://ap.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uw.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iw.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ja.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wc.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://cw.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ru.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://op.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yg.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://fi.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uo.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://dk.hnjuh.cn

JS:   Object.entries(obj)
来源：http://kz.szsharing.cn

TS:   Object.entries(obj)
来源：http://qh.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sd.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fm.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://xv.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://qh.gzmigu.cn

================================================================================
来源：http://sg.wgjwhj.cn

H. 异常与错误处理
来源：http://vh.hahajie.cn

================================================================================
来源：http://ih.lnxyls.cn

[H01] try / catch 基础
来源：http://gp.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mi.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kx.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fk.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cd.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kj.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hw.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://je.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bs.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://dp.shxzskj.cn


<!-- 参考信息 -->