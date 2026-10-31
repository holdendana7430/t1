代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fn.szsharing.cn

[E19] 多行文本按行拆分
来源：http://be.szxytkj.cn

Py:   s.splitlines()
来源：http://qm.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bv.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://kc.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ed.521024.cn

Java: s.lines().toList()
来源：http://wi.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://hm.shxzukj.cn

Ruby: s.lines
来源：http://kv.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://sw.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://zd.521024.cn

Py:   if not s:
来源：http://at.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ea.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ff.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ip.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://vh.gzmigu.cn

Go:   if s == "" {}
来源：http://cq.gzmigu.cn

Ruby: if s.empty?
来源：http://ns.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bg.nicolike.cn

[E21] 超长截断加省略号
来源：http://sl.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cg.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ir.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fj.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ty.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://td.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://pn.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nj.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://se.szsharing.cn

[E22] 字节长度与字符长度
来源：http://vt.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://js.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://je.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uu.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://da.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uj.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gh.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://xi.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jv.huixinmuqiang.cn

================================================================================
来源：http://un.hnjuh.cn

F. 文件与目录
来源：http://zs.lnxyls.cn

================================================================================
来源：http://jl.haigaiapp.cn

[F01] 读取整个文件
来源：http://qq.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rc.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://nj.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bi.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xl.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iu.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ln.hahajie.cn

Ruby: File.read("a.txt")
来源：http://wx.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://gt.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://fr.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yy.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fl.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ib.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rl.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xu.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://za.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dy.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qn.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://bc.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cf.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gv.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ss.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sm.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eu.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ty.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dx.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pp.shxzskj.cn

[F04] 追加写入文件
来源：http://jl.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bn.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kq.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nc.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://in.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rp.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ov.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hm.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://aw.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lz.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://rq.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://xk.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://mk.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bm.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://to.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://il.asd995.cn

C#:   File.Exists("a.txt")
来源：http://xa.gzmigu.cn

[F06] 删除文件
来源：http://pg.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://ln.9csxet.cn

PHP:  unlink("a.txt");
来源：http://xy.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pi.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zp.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fc.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ax.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://gh.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://vf.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://hc.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jy.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wr.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cy.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zs.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zx.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zw.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tj.nicolike.cn

[F08] 遍历目录
来源：http://dc.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gh.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mt.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://eo.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://kl.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cq.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yy.colortex.cn

Ruby: Dir.children("dir")
来源：http://mx.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://fo.hnjuh.cn

[F09] 获取文件大小
来源：http://eu.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://nk.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://fl.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://rr.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://md.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uv.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bm.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ig.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://id.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ap.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vk.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ey.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mi.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://jf.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yb.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ic.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iq.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wh.panjiajie.cn

[F11] 复制与移动文件
来源：http://su.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qo.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zu.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wt.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yj.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bf.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ww.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gf.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ws.gzmigu.cn

[F12] CSV 读写
来源：http://fc.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zv.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://er.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://of.newstarts.cn

TS:   // 同上
来源：http://fz.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://di.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qa.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xo.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yo.hnjuh.cn

================================================================================
来源：http://to.szsharing.cn

G. 面向对象
来源：http://yt.szxytkj.cn

================================================================================
来源：http://cs.gzmigu.cn

[G01] 定义类
来源：http://uf.szxytkj.cn

Py:   class User: pass
来源：http://iy.hahajie.cn

PHP:  class User {}
来源：http://zo.lnxyls.cn

JS:   class User {}
来源：http://fx.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://ez.hahajie.cn

Java: class User {}
来源：http://bb.colortex.cn

Go:   type User struct { Name string }
来源：http://nn.asd995.cn

Ruby: class User; end
来源：http://yp.shtwfgs.cn

C#:   class User {}
来源：http://yj.nicolike.cn

[G02] 构造函数
来源：http://kk.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://zp.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://iu.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ka.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://kp.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://or.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uz.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://it.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ww.shxzskj.cn

[G03] 实例属性
来源：http://wo.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://xp.hnjuh.cn

PHP:  public string $name = "x";
来源：http://sr.huanxung.cn

JS:   this.name = "x";
来源：http://yv.panjiajie.cn

TS:   name: string = "x";
来源：http://he.hnjuh.cn

Java: private String name;
来源：http://bt.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dn.hnjuh.cn

Ruby: @name = "x"
来源：http://tc.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://up.chemitech.net.cn

[G04] 定义方法
来源：http://af.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://yz.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://up.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://wo.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://zs.9csxet.cn

Java: String greet() { return name; }
来源：http://yf.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ys.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://gf.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://gm.shtwfgs.cn

[G05] 继承
来源：http://eb.newstarts.cn

Py:   class Admin(User): pass
来源：http://hu.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://py.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://yj.asd995.cn

TS:   class Admin extends User {}
来源：http://ug.lnxyls.cn

Java: class Admin extends User {}
来源：http://zx.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zl.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://qi.jctech888.com.cn

C#:   class Admin : User {}
来源：http://ty.huanxung.cn

[G06] 重写方法
来源：http://nm.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://cm.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tl.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://xp.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://bk.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://te.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://os.colortex.cn

Ruby: def greet; "admin"; end
来源：http://fl.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://bi.lnxyls.cn

[G07] 调用父类方法
来源：http://vu.shxzskj.cn

Py:   super().greet()
来源：http://ku.muxihuayi.cn

PHP:  parent::greet();
来源：http://sn.jctech888.com.cn

JS:   super.greet();
来源：http://uz.hnjuh.cn

TS:   super.greet();
来源：http://py.yuexingan06.cn

Java: super.greet();
来源：http://pf.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pe.huixiangedu.cn

Ruby: super
来源：http://wx.hnjuh.cn

C#:   base.Greet();
来源：http://sn.gzmigu.cn

[G08] 静态方法与属性
来源：http://eh.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rc.huanxung.cn

PHP:  public static function f() {}
来源：http://jn.muxihuayi.cn

JS:   static f() {}
来源：http://li.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://sz.9csxet.cn

Java: static void f() {}
来源：http://wv.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fs.yuexingan06.cn

Ruby: def self.f; end
来源：http://pa.nicolike.cn

C#:   public static void F() {}
来源：http://em.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://lq.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://sb.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mo.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sa.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://dx.huanxung.cn

Java: interface Shape { double area(); }
来源：http://sl.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://xf.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zz.521024.cn

C#:   interface IShape { double Area(); }
来源：http://zs.szxytkj.cn

[G10] 访问控制
来源：http://ya.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://mf.colortex.cn

PHP:  public / protected / private
来源：http://qt.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://ba.nicolike.cn

TS:   public / protected / private
来源：http://oi.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://sz.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ao.szxytkj.cn

Ruby: public / protected / private
来源：http://lu.hnjuh.cn

C#:   public / protected / private / internal
来源：http://rr.jianghongdianzi.cn

[G11] getter / setter
来源：http://dy.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://fo.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jc.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://pu.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://do.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://cp.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kh.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://db.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://pl.shxzskj.cn

[G12] 对象转字符串
来源：http://oz.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://rx.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mj.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://iv.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://dt.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://fk.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cj.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://dm.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://gy.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://re.lnxyls.cn

Py:   isinstance(u, User)
来源：http://ga.yuexingan06.cn

PHP:  $u instanceof User
来源：http://bq.bookmarksfly.cn

JS:   u instanceof User
来源：http://qn.bookmarksfly.cn

TS:   u instanceof User
来源：http://xo.muxihuayi.cn

Java: u instanceof User
来源：http://fx.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lw.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://wu.hnjuh.cn

C#:   u is User
来源：http://fl.asd995.cn

[G14] 数据类 / record
来源：http://ky.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ol.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://mh.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pk.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://rz.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://ia.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://gn.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://do.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ih.asd995.cn

[G15] 枚举
来源：http://ta.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aj.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qd.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cm.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://md.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://fp.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wj.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://oa.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://co.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://lv.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://by.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://dq.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://sj.521024.cn

TS:   Object.entries(obj)
来源：http://bo.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ei.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uk.9csxet.cn

Ruby: obj.instance_variables
来源：http://ol.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.gzmigu.cn

================================================================================
来源：http://ej.jianghongdianzi.cn

H. 异常与错误处理
来源：http://kd.9csxet.cn

================================================================================
来源：http://uo.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://co.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://un.nicolike.cn


<!-- 参考信息 -->