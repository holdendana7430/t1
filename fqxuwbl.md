代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://nl.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jr.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qb.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dn.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yo.nszjky.cn

[E19] 多行文本按行拆分
来源：http://lu.521024.cn

Py:   s.splitlines()
来源：http://tw.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ey.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://mr.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://ne.521024.cn

Java: s.lines().toList()
来源：http://zc.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://wr.shxzskj.cn

Ruby: s.lines
来源：http://jt.nszjky.cn

C#:   s.Split('\n')
来源：http://mn.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://bm.nszjky.cn

Py:   if not s:
来源：http://ol.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wx.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rc.521024.cn

TS:   if (s === "") {}
来源：http://rc.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://pz.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://xj.chemitech.net.cn

Ruby: if s.empty?
来源：http://hb.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fp.colortex.cn

[E21] 超长截断加省略号
来源：http://kv.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cc.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jl.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wz.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lj.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uf.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://nm.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dw.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pe.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://be.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rv.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tm.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ro.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hj.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jn.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://de.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://sh.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://an.lnxyls.cn

================================================================================
来源：http://cx.huixinmuqiang.cn

F. 文件与目录
来源：http://rs.nszjky.cn

================================================================================
来源：http://lj.wgjwhj.cn

[F01] 读取整个文件
来源：http://pl.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dq.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://kj.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jx.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://po.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hs.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zd.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://ul.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://cg.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://zj.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jr.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xf.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rn.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ci.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://my.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://az.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://os.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yw.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://qv.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ql.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mx.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oy.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bc.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bn.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yf.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://gz.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uq.9csxet.cn

[F04] 追加写入文件
来源：http://ga.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wb.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bn.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oh.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vv.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ve.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ky.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yb.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uq.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://jf.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rs.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://tf.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://wp.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://dj.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gk.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qq.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://ah.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ua.szsharing.cn

[F06] 删除文件
来源：http://nv.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://zq.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://tr.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ql.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://al.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qs.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://bk.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://eo.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://pr.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://xb.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://la.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fp.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gy.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nn.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uy.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fg.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rh.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pw.huixinmuqiang.cn

[F08] 遍历目录
来源：http://tx.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cy.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nm.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://vy.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://nf.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nl.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jo.colortex.cn

Ruby: Dir.children("dir")
来源：http://wt.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://tg.hahajie.cn

[F09] 获取文件大小
来源：http://zd.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ao.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://dz.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://lz.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://wy.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ud.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ws.521024.cn

Ruby: File.size("a.txt")
来源：http://sc.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://bm.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://yr.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gz.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://go.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lt.colortex.cn

TS:   path.extname("a.txt")
来源：http://ai.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ux.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lk.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gl.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zf.nszjky.cn

[F11] 复制与移动文件
来源：http://sx.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cr.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wu.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ql.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ol.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xz.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gi.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vp.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://au.jianghongdianzi.cn

[F12] CSV 读写
来源：http://xz.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jv.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ju.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vy.bjjhwx.cn

TS:   // 同上
来源：http://bs.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bt.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hi.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://or.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://db.szsharing.cn

================================================================================
来源：http://ep.haigaiapp.cn

G. 面向对象
来源：http://vm.hahajie.cn

================================================================================
来源：http://ea.shxzskj.cn

[G01] 定义类
来源：http://ua.bookmarksfly.cn

Py:   class User: pass
来源：http://if.szsharing.cn

PHP:  class User {}
来源：http://fc.hahajie.cn

JS:   class User {}
来源：http://fw.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://vj.chemitech.net.cn

Java: class User {}
来源：http://mc.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://lx.hahajie.cn

Ruby: class User; end
来源：http://zv.shxzukj.cn

C#:   class User {}
来源：http://dr.haigaiapp.cn

[G02] 构造函数
来源：http://hs.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://lc.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://cj.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://jf.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://zx.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://fm.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mw.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ye.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://wb.shxzskj.cn

[G03] 实例属性
来源：http://cs.chemitech.net.cn

Py:   self.name = "x"
来源：http://ob.newstarts.cn

PHP:  public string $name = "x";
来源：http://wr.newstarts.cn

JS:   this.name = "x";
来源：http://pc.shxzukj.cn

TS:   name: string = "x";
来源：http://cs.nszjky.cn

Java: private String name;
来源：http://zu.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fv.asd995.cn

Ruby: @name = "x"
来源：http://wq.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://uq.hahajie.cn

[G04] 定义方法
来源：http://yl.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://iy.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rd.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://zy.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://bg.yuexingan06.cn

Java: String greet() { return name; }
来源：http://iw.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dg.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://uf.521024.cn

C#:   public string Greet() => Name;
来源：http://se.szxytkj.cn

[G05] 继承
来源：http://dy.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://mq.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://hd.shxzukj.cn

JS:   class Admin extends User {}
来源：http://yt.shxzskj.cn

TS:   class Admin extends User {}
来源：http://oj.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://mh.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://on.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://mb.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ej.yuexingan06.cn

[G06] 重写方法
来源：http://pk.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://hu.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nk.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://qd.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://tt.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://uk.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://re.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://nw.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://wj.bjjhwx.cn

[G07] 调用父类方法
来源：http://dp.shxzskj.cn

Py:   super().greet()
来源：http://hv.nszjky.cn

PHP:  parent::greet();
来源：http://xn.9csxet.cn

JS:   super.greet();
来源：http://vf.newstarts.cn

TS:   super.greet();
来源：http://dk.shxzskj.cn

Java: super.greet();
来源：http://ih.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tw.yuexingan06.cn

Ruby: super
来源：http://kt.shxzukj.cn

C#:   base.Greet();
来源：http://oq.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://pe.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://js.shxzukj.cn

PHP:  public static function f() {}
来源：http://rs.nicolike.cn

JS:   static f() {}
来源：http://qc.shxzskj.cn

TS:   static f(): void {}
来源：http://xv.9csxet.cn

Java: static void f() {}
来源：http://cg.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ly.bookmarksfly.cn

Ruby: def self.f; end
来源：http://pr.szxytkj.cn

C#:   public static void F() {}
来源：http://ux.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://rd.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://bf.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nb.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oh.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://aa.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://ev.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://tr.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://af.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://uc.yuexingan06.cn

[G10] 访问控制
来源：http://le.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://qy.szsharing.cn

PHP:  public / protected / private
来源：http://zu.colortex.cn

JS:   #private 字段；其余公开
来源：http://st.gzmigu.cn

TS:   public / protected / private
来源：http://xp.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://ke.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zr.huixiangedu.cn

Ruby: public / protected / private
来源：http://oz.huanxung.cn

C#:   public / protected / private / internal
来源：http://pr.yuexingan06.cn

[G11] getter / setter
来源：http://ow.9csxet.cn

Py:   @property 与 @x.setter
来源：http://km.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://os.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://cj.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://oj.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://rz.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hb.colortex.cn

Ruby: attr_accessor :name
来源：http://sa.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://et.shtwfgs.cn

[G12] 对象转字符串
来源：http://hp.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://xl.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dq.huanxung.cn

JS:   toString() { return this.name; }
来源：http://lp.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://jo.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://px.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ql.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://za.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://ro.wgjwhj.cn

[G13] 判断对象类型
来源：http://fs.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://jk.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://na.nszjky.cn

JS:   u instanceof User
来源：http://hf.lnxyls.cn

TS:   u instanceof User
来源：http://sv.panjiajie.cn

Java: u instanceof User
来源：http://nu.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xb.521024.cn

Ruby: u.is_a?(User)
来源：http://at.521024.cn

C#:   u is User
来源：http://ds.haigaiapp.cn

[G14] 数据类 / record
来源：http://cq.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://or.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ks.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cc.521024.cn

TS:   type User = { name: string; age: number };
来源：http://cx.colortex.cn

Java: record User(String name, int age) {}
来源：http://yt.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ij.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qc.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://id.szsharing.cn

[G15] 枚举
来源：http://vm.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ih.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jy.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ip.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tc.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://ei.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zd.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://ml.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qs.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://dg.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dx.asd995.cn

PHP:  get_object_vars($obj);
来源：http://zn.asd995.cn

JS:   Object.entries(obj)
来源：http://kj.newstarts.cn

TS:   Object.entries(obj)
来源：http://ki.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kf.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gt.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://is.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ny.szsharing.cn

================================================================================
来源：http://su.huixiangedu.cn


<!-- 参考信息 -->