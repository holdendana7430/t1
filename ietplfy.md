代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kc.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://wj.lnxyls.cn

Py:   s.splitlines()
来源：http://tr.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nj.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://dh.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://mb.muxihuayi.cn

Java: s.lines().toList()
来源：http://oo.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://jv.hnjuh.cn

Ruby: s.lines
来源：http://my.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://gv.521024.cn

[E20] 判断字符串是否为空
来源：http://ur.nszjky.cn

Py:   if not s:
来源：http://dh.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gz.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uq.colortex.cn

TS:   if (s === "") {}
来源：http://ib.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://wd.nszjky.cn

Go:   if s == "" {}
来源：http://pf.521024.cn

Ruby: if s.empty?
来源：http://sj.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gz.9csxet.cn

[E21] 超长截断加省略号
来源：http://ui.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gy.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tx.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vg.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kn.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iw.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://sd.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gq.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uk.newstarts.cn

[E22] 字节长度与字符长度
来源：http://vw.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ly.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tp.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://al.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://il.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bb.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://sg.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cn.shtwfgs.cn

================================================================================
来源：http://dl.shxzukj.cn

F. 文件与目录
来源：http://me.nicolike.cn

================================================================================
来源：http://uk.wgjwhj.cn

[F01] 读取整个文件
来源：http://xs.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ma.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ke.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zy.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zo.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ax.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gm.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://ef.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://va.nicolike.cn

[F02] 逐行读取文件
来源：http://uf.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ej.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lv.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yg.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tl.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nd.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nc.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fa.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mz.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ni.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oj.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qh.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ri.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gq.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cj.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://on.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ji.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hp.shxzskj.cn

[F04] 追加写入文件
来源：http://dm.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ph.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wb.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rd.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ci.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qx.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sf.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hh.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ts.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://jn.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://af.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://tv.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://jk.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://rq.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xf.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yr.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://hi.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://bm.jianghongdianzi.cn

[F06] 删除文件
来源：http://tq.colortex.cn

Py:   os.remove("a.txt")
来源：http://ji.521024.cn

PHP:  unlink("a.txt");
来源：http://fv.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ym.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ba.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ql.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://yn.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://fo.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://gt.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://gs.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hv.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yd.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jz.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ms.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vc.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gf.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bq.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://of.bjjhwx.cn

[F08] 遍历目录
来源：http://xw.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uq.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ql.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ez.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://vk.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://md.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fc.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://rh.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://nl.hnjuh.cn

[F09] 获取文件大小
来源：http://wx.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://jk.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://eu.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ko.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mc.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jf.szsharing.cn

Ruby: File.size("a.txt")
来源：http://bj.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://wa.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://tm.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dg.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jz.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dh.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://dn.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yn.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ct.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ha.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ia.gzmigu.cn

[F11] 复制与移动文件
来源：http://yv.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rx.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ng.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mt.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ez.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qr.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xf.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rk.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fq.jctech888.com.cn

[F12] CSV 读写
来源：http://vj.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sa.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://my.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ps.asd995.cn

TS:   // 同上
来源：http://mb.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bu.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dn.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hp.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rp.wgjwhj.cn

================================================================================
来源：http://eb.nszjky.cn

G. 面向对象
来源：http://it.asd995.cn

================================================================================
来源：http://em.szxytkj.cn

[G01] 定义类
来源：http://zn.nszjky.cn

Py:   class User: pass
来源：http://we.huixiangedu.cn

PHP:  class User {}
来源：http://ch.521024.cn

JS:   class User {}
来源：http://ri.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://ej.jianghongdianzi.cn

Java: class User {}
来源：http://ty.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ph.chemitech.net.cn

Ruby: class User; end
来源：http://ao.asd995.cn

C#:   class User {}
来源：http://hn.yuntaijiaju.cn

[G02] 构造函数
来源：http://cs.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://pa.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://fz.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ew.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://sj.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://na.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bi.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://id.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://qa.jctech888.com.cn

[G03] 实例属性
来源：http://ea.colortex.cn

Py:   self.name = "x"
来源：http://nq.521024.cn

PHP:  public string $name = "x";
来源：http://zs.shxzskj.cn

JS:   this.name = "x";
来源：http://nc.jctech888.com.cn

TS:   name: string = "x";
来源：http://tp.bookmarksfly.cn

Java: private String name;
来源：http://mk.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yk.nicolike.cn

Ruby: @name = "x"
来源：http://ly.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://ka.shxzskj.cn

[G04] 定义方法
来源：http://bl.nszjky.cn

Py:   def greet(self): return self.name
来源：http://ws.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ox.asd995.cn

JS:   greet() { return this.name; }
来源：http://dv.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://gf.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://oa.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gv.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://zb.huanxung.cn

C#:   public string Greet() => Name;
来源：http://hl.huixiangedu.cn

[G05] 继承
来源：http://sx.9csxet.cn

Py:   class Admin(User): pass
来源：http://ys.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://zn.gzmigu.cn

JS:   class Admin extends User {}
来源：http://df.hahajie.cn

TS:   class Admin extends User {}
来源：http://du.shtwfgs.cn

Java: class Admin extends User {}
来源：http://xg.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gf.hahajie.cn

Ruby: class Admin < User; end
来源：http://jv.szxytkj.cn

C#:   class Admin : User {}
来源：http://vu.shxzukj.cn

[G06] 重写方法
来源：http://lz.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ea.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ty.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://ru.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://jo.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://ia.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fo.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://rw.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://tg.asd995.cn

[G07] 调用父类方法
来源：http://gv.shxzukj.cn

Py:   super().greet()
来源：http://cg.huanxung.cn

PHP:  parent::greet();
来源：http://lw.yuntaijiaju.cn

JS:   super.greet();
来源：http://ug.haigaiapp.cn

TS:   super.greet();
来源：http://vd.yuexingan06.cn

Java: super.greet();
来源：http://zc.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sq.huixiangedu.cn

Ruby: super
来源：http://uk.yuexingan06.cn

C#:   base.Greet();
来源：http://vf.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ri.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://us.bjjhwx.cn

PHP:  public static function f() {}
来源：http://zg.jianghongdianzi.cn

JS:   static f() {}
来源：http://ly.lnxyls.cn

TS:   static f(): void {}
来源：http://iv.bookmarksfly.cn

Java: static void f() {}
来源：http://zn.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mr.muxihuayi.cn

Ruby: def self.f; end
来源：http://yd.panjiajie.cn

C#:   public static void F() {}
来源：http://tv.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://kl.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://sy.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cd.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nb.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://no.9csxet.cn

Java: interface Shape { double area(); }
来源：http://js.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://tj.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ny.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://yk.jianghongdianzi.cn

[G10] 访问控制
来源：http://qt.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://dq.asd995.cn

PHP:  public / protected / private
来源：http://op.newstarts.cn

JS:   #private 字段；其余公开
来源：http://xs.hnjuh.cn

TS:   public / protected / private
来源：http://zw.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://bi.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zv.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://xz.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ej.gzmigu.cn

[G11] getter / setter
来源：http://zp.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://rr.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wr.szsharing.cn

JS:   get name() { return this._name; }
来源：http://ry.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://vj.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://wo.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bs.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://gy.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ox.newstarts.cn

[G12] 对象转字符串
来源：http://cs.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://dn.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yo.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://jb.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://fz.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://gx.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nb.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://rb.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://ze.szsharing.cn

[G13] 判断对象类型
来源：http://jo.szsharing.cn

Py:   isinstance(u, User)
来源：http://wf.yuexingan06.cn

PHP:  $u instanceof User
来源：http://um.hnjuh.cn

JS:   u instanceof User
来源：http://ts.yuexingan06.cn

TS:   u instanceof User
来源：http://ok.chemitech.net.cn

Java: u instanceof User
来源：http://gq.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pt.nszjky.cn

Ruby: u.is_a?(User)
来源：http://gq.panjiajie.cn

C#:   u is User
来源：http://ti.newstarts.cn

[G14] 数据类 / record
来源：http://jx.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vc.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ew.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ta.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://uq.9csxet.cn

Java: record User(String name, int age) {}
来源：http://xq.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://dm.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://el.colortex.cn

C#:   record User(string Name, int Age);
来源：http://qn.hahajie.cn

[G15] 枚举
来源：http://ke.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yl.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nw.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tp.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ag.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://ll.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fv.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://eq.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jw.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://us.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://me.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ux.asd995.cn

JS:   Object.entries(obj)
来源：http://zx.9csxet.cn

TS:   Object.entries(obj)
来源：http://bv.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cr.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pc.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://ae.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://aj.shtwfgs.cn

================================================================================
来源：http://cf.jctech888.com.cn

H. 异常与错误处理
来源：http://zd.hahajie.cn

================================================================================
来源：http://ab.huixiangedu.cn

[H01] try / catch 基础
来源：http://wz.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ci.9csxet.cn


<!-- 参考信息 -->