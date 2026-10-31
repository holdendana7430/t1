代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://im.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://hb.nicolike.cn

Java: s.lines().toList()
来源：http://pm.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://pu.haigaiapp.cn

Ruby: s.lines
来源：http://ro.9csxet.cn

C#:   s.Split('\n')
来源：http://ly.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://tn.shxzukj.cn

Py:   if not s:
来源：http://dx.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fk.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ch.bjjhwx.cn

TS:   if (s === "") {}
来源：http://su.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://so.yuexingan06.cn

Go:   if s == "" {}
来源：http://wr.szxytkj.cn

Ruby: if s.empty?
来源：http://qy.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gb.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://jc.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wt.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iz.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wv.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wn.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pb.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://bt.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yf.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gn.hahajie.cn

[E22] 字节长度与字符长度
来源：http://bc.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gb.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gm.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gh.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://br.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rx.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://ck.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yr.huixinmuqiang.cn

================================================================================
来源：http://bc.colortex.cn

F. 文件与目录
来源：http://pt.521024.cn

================================================================================
来源：http://oz.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ak.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://os.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://mw.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oy.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mc.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kv.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sr.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://wf.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://gg.haigaiapp.cn

[F02] 逐行读取文件
来源：http://uw.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uv.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ej.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://go.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://us.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zi.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://km.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://in.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rs.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://sj.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ht.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fx.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dp.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wp.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dz.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ka.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://zy.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://me.huanxung.cn

[F04] 追加写入文件
来源：http://jh.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ze.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ar.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sh.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://au.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fv.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://da.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ln.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dd.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://ve.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xh.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://rb.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://op.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://mm.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pn.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qn.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://yw.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ta.asd995.cn

[F06] 删除文件
来源：http://ig.521024.cn

Py:   os.remove("a.txt")
来源：http://sp.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ue.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ix.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eu.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mn.colortex.cn

Go:   os.Remove("a.txt")
来源：http://uj.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ey.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://hh.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://lq.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fl.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pm.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qp.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cd.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xz.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tj.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zo.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iv.shxzukj.cn

[F08] 遍历目录
来源：http://vm.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bu.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gy.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://cm.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://vx.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xa.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gf.asd995.cn

Ruby: Dir.children("dir")
来源：http://zv.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://jc.9csxet.cn

[F09] 获取文件大小
来源：http://fr.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://hu.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://vu.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://cp.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ee.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zm.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sc.hahajie.cn

Ruby: File.size("a.txt")
来源：http://tg.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://ka.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://vn.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qx.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ag.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cm.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://bc.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yw.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jm.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wk.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dg.chemitech.net.cn

[F11] 复制与移动文件
来源：http://pl.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ec.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kd.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://un.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gj.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://be.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://et.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ha.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ue.shtwfgs.cn

[F12] CSV 读写
来源：http://jj.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iw.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mv.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zj.521024.cn

TS:   // 同上
来源：http://wr.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://me.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ks.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nm.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oz.hahajie.cn

================================================================================
来源：http://oy.jctech888.com.cn

G. 面向对象
来源：http://ak.bookmarksfly.cn

================================================================================
来源：http://mh.yuexingan06.cn

[G01] 定义类
来源：http://ke.shxzskj.cn

Py:   class User: pass
来源：http://di.nszjky.cn

PHP:  class User {}
来源：http://mq.shxzukj.cn

JS:   class User {}
来源：http://ly.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://jm.bjjhwx.cn

Java: class User {}
来源：http://wo.asd995.cn

Go:   type User struct { Name string }
来源：http://aw.bookmarksfly.cn

Ruby: class User; end
来源：http://qm.yuexingan06.cn

C#:   class User {}
来源：http://hq.shtwfgs.cn

[G02] 构造函数
来源：http://yk.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://pc.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://fr.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://ez.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://mt.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://aa.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ew.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://xy.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://xl.9csxet.cn

[G03] 实例属性
来源：http://pf.gzmigu.cn

Py:   self.name = "x"
来源：http://xm.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ri.521024.cn

JS:   this.name = "x";
来源：http://xe.chemitech.net.cn

TS:   name: string = "x";
来源：http://gs.shtwfgs.cn

Java: private String name;
来源：http://ty.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yx.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://zl.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ob.hahajie.cn

[G04] 定义方法
来源：http://qb.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://tt.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vq.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://ic.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://pw.shxzskj.cn

Java: String greet() { return name; }
来源：http://ba.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ad.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://wt.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://lb.shtwfgs.cn

[G05] 继承
来源：http://dg.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://pp.521024.cn

PHP:  class Admin extends User {}
来源：http://xt.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://ik.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://ft.nszjky.cn

Java: class Admin extends User {}
来源：http://kn.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ag.nicolike.cn

Ruby: class Admin < User; end
来源：http://ff.gzmigu.cn

C#:   class Admin : User {}
来源：http://nw.bjjhwx.cn

[G06] 重写方法
来源：http://et.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://fd.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://te.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://hs.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://tf.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://br.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hn.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://gs.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://hm.hahajie.cn

[G07] 调用父类方法
来源：http://hv.jianghongdianzi.cn

Py:   super().greet()
来源：http://iq.shtwfgs.cn

PHP:  parent::greet();
来源：http://vk.shxzskj.cn

JS:   super.greet();
来源：http://ed.shtwfgs.cn

TS:   super.greet();
来源：http://zl.jctech888.com.cn

Java: super.greet();
来源：http://xt.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lx.shxzskj.cn

Ruby: super
来源：http://aq.jctech888.com.cn

C#:   base.Greet();
来源：http://uo.szsharing.cn

[G08] 静态方法与属性
来源：http://vd.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zp.wgjwhj.cn

PHP:  public static function f() {}
来源：http://ak.nicolike.cn

JS:   static f() {}
来源：http://co.panjiajie.cn

TS:   static f(): void {}
来源：http://uf.9csxet.cn

Java: static void f() {}
来源：http://zw.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bq.521024.cn

Ruby: def self.f; end
来源：http://ul.shxzskj.cn

C#:   public static void F() {}
来源：http://za.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ss.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://mx.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tb.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ov.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ql.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://fq.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://qz.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vz.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://in.yuntaijiaju.cn

[G10] 访问控制
来源：http://qp.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://mu.9csxet.cn

PHP:  public / protected / private
来源：http://cs.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://cu.bookmarksfly.cn

TS:   public / protected / private
来源：http://hj.asd995.cn

Java: public / protected / private / 默认包级
来源：http://in.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://po.lnxyls.cn

Ruby: public / protected / private
来源：http://un.hahajie.cn

C#:   public / protected / private / internal
来源：http://ig.521024.cn

[G11] getter / setter
来源：http://xp.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://xt.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dl.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://gf.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://ty.9csxet.cn

Java: public String getName() { return name; }
来源：http://ly.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hr.szsharing.cn

Ruby: attr_accessor :name
来源：http://lk.hahajie.cn

C#:   public string Name { get; set; }
来源：http://sp.huixiangedu.cn

[G12] 对象转字符串
来源：http://tg.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://ar.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wh.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://ci.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://mw.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://fb.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bi.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://bt.asd995.cn

C#:   public override string ToString() => Name;
来源：http://il.szsharing.cn

[G13] 判断对象类型
来源：http://te.colortex.cn

Py:   isinstance(u, User)
来源：http://aq.bjjhwx.cn

PHP:  $u instanceof User
来源：http://yj.yuntaijiaju.cn

JS:   u instanceof User
来源：http://ag.shxzukj.cn

TS:   u instanceof User
来源：http://zh.jianghongdianzi.cn

Java: u instanceof User
来源：http://dn.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mf.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ub.huanxung.cn

C#:   u is User
来源：http://fm.haigaiapp.cn

[G14] 数据类 / record
来源：http://ud.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wo.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ha.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://of.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://rp.colortex.cn

Java: record User(String name, int age) {}
来源：http://ip.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://my.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lu.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://pb.jctech888.com.cn

[G15] 枚举
来源：http://lo.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fe.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lr.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sq.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hb.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://qo.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yz.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://ab.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zv.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://pn.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qv.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://gz.hnjuh.cn

JS:   Object.entries(obj)
来源：http://pl.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://yn.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zb.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zl.lnxyls.cn

Ruby: obj.instance_variables
来源：http://ix.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://um.hahajie.cn

================================================================================
来源：http://np.hahajie.cn

H. 异常与错误处理
来源：http://hw.gzmigu.cn

================================================================================
来源：http://gv.wgjwhj.cn

[H01] try / catch 基础
来源：http://tc.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jv.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wy.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lf.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hd.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gp.szxytkj.cn


<!-- 参考信息 -->