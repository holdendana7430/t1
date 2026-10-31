代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fq.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://fo.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://xm.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nt.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://wz.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://je.colortex.cn

Java: s.lines().toList()
来源：http://bj.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://iy.haigaiapp.cn

Ruby: s.lines
来源：http://ap.9csxet.cn

C#:   s.Split('\n')
来源：http://ts.hahajie.cn

[E20] 判断字符串是否为空
来源：http://pl.szxytkj.cn

Py:   if not s:
来源：http://fp.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cm.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bf.szxytkj.cn

TS:   if (s === "") {}
来源：http://ti.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://qs.szsharing.cn

Go:   if s == "" {}
来源：http://pr.wgjwhj.cn

Ruby: if s.empty?
来源：http://zq.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fa.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://td.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vd.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ny.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eo.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cp.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gh.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://et.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://az.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ie.nszjky.cn

[E22] 字节长度与字符长度
来源：http://jv.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lr.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oc.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qx.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ro.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://er.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hy.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://fc.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yl.wgjwhj.cn

================================================================================
来源：http://yy.9csxet.cn

F. 文件与目录
来源：http://ul.521024.cn

================================================================================
来源：http://tq.hnjuh.cn

[F01] 读取整个文件
来源：http://rk.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rd.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://ko.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bi.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gc.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xs.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rq.newstarts.cn

Ruby: File.read("a.txt")
来源：http://jv.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://cp.hahajie.cn

[F02] 逐行读取文件
来源：http://ar.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hk.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ed.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jz.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ig.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://im.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nz.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nw.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uz.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://tx.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fk.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://os.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rm.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wq.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://za.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://hy.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cc.szsharing.cn

[F04] 追加写入文件
来源：http://ne.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zn.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xf.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ay.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cj.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ju.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://da.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sq.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://nw.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nr.asd995.cn

PHP:  file_exists("a.txt");
来源：http://kp.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://bo.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://lg.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bp.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kl.521024.cn

Ruby: File.exist?("a.txt")
来源：http://vi.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://aj.haigaiapp.cn

[F06] 删除文件
来源：http://dq.asd995.cn

Py:   os.remove("a.txt")
来源：http://sr.szsharing.cn

PHP:  unlink("a.txt");
来源：http://kg.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eb.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jm.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mr.colortex.cn

Go:   os.Remove("a.txt")
来源：http://hx.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://sa.colortex.cn

C#:   File.Delete("a.txt");
来源：http://ov.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ya.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ye.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ak.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://za.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kh.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pp.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gt.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tn.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ur.nszjky.cn

[F08] 遍历目录
来源：http://ie.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qn.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nv.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://sw.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://ix.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ex.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yb.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://rq.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://ih.521024.cn

[F09] 获取文件大小
来源：http://op.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://qu.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://eq.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://rl.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://vs.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kp.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lx.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://fo.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://du.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://em.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zv.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vy.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zq.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://wu.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://li.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://af.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://va.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yo.gzmigu.cn

[F11] 复制与移动文件
来源：http://zy.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dv.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fg.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zs.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sm.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kv.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kc.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://my.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ly.shxzukj.cn

[F12] CSV 读写
来源：http://um.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fj.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qs.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zm.jctech888.com.cn

TS:   // 同上
来源：http://rv.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cy.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iy.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oc.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ch.newstarts.cn

================================================================================
来源：http://ee.asd995.cn

G. 面向对象
来源：http://ai.9csxet.cn

================================================================================
来源：http://yk.asd995.cn

[G01] 定义类
来源：http://lk.shtwfgs.cn

Py:   class User: pass
来源：http://vy.yuntaijiaju.cn

PHP:  class User {}
来源：http://fd.wgjwhj.cn

JS:   class User {}
来源：http://ik.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://kx.huixinmuqiang.cn

Java: class User {}
来源：http://ve.521024.cn

Go:   type User struct { Name string }
来源：http://kj.lnxyls.cn

Ruby: class User; end
来源：http://qz.hnjuh.cn

C#:   class User {}
来源：http://wy.colortex.cn

[G02] 构造函数
来源：http://vi.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ql.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://vi.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://or.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://tz.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://cx.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rh.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://se.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://ro.bjjhwx.cn

[G03] 实例属性
来源：http://xw.jctech888.com.cn

Py:   self.name = "x"
来源：http://it.newstarts.cn

PHP:  public string $name = "x";
来源：http://nj.newstarts.cn

JS:   this.name = "x";
来源：http://tp.panjiajie.cn

TS:   name: string = "x";
来源：http://pv.jctech888.com.cn

Java: private String name;
来源：http://gh.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dh.huanxung.cn

Ruby: @name = "x"
来源：http://ka.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://qm.gzmigu.cn

[G04] 定义方法
来源：http://vn.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://jz.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kj.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://bp.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://lg.huanxung.cn

Java: String greet() { return name; }
来源：http://rl.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vn.panjiajie.cn

Ruby: def greet; @name; end
来源：http://yo.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ta.shxzskj.cn

[G05] 继承
来源：http://jj.szsharing.cn

Py:   class Admin(User): pass
来源：http://qd.asd995.cn

PHP:  class Admin extends User {}
来源：http://vk.shxzukj.cn

JS:   class Admin extends User {}
来源：http://bs.hnjuh.cn

TS:   class Admin extends User {}
来源：http://vw.wgjwhj.cn

Java: class Admin extends User {}
来源：http://tl.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ql.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://kh.chemitech.net.cn

C#:   class Admin : User {}
来源：http://ll.hahajie.cn

[G06] 重写方法
来源：http://sg.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://kk.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sq.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://sy.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hs.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://pd.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xh.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://be.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://zo.panjiajie.cn

[G07] 调用父类方法
来源：http://fo.hnjuh.cn

Py:   super().greet()
来源：http://bm.gzmigu.cn

PHP:  parent::greet();
来源：http://ek.hnjuh.cn

JS:   super.greet();
来源：http://rc.muxihuayi.cn

TS:   super.greet();
来源：http://hu.jctech888.com.cn

Java: super.greet();
来源：http://xn.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tz.shtwfgs.cn

Ruby: super
来源：http://td.haigaiapp.cn

C#:   base.Greet();
来源：http://xm.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://fw.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mc.muxihuayi.cn

PHP:  public static function f() {}
来源：http://fu.huanxung.cn

JS:   static f() {}
来源：http://bl.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ac.yuexingan06.cn

Java: static void f() {}
来源：http://ks.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://az.chemitech.net.cn

Ruby: def self.f; end
来源：http://ts.muxihuayi.cn

C#:   public static void F() {}
来源：http://cv.asd995.cn

[G09] 接口 / 抽象类
来源：http://os.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://wc.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eh.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tn.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://pw.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://gd.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://zf.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sp.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://rp.yuntaijiaju.cn

[G10] 访问控制
来源：http://di.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://xg.gzmigu.cn

PHP:  public / protected / private
来源：http://dh.szsharing.cn

JS:   #private 字段；其余公开
来源：http://yb.bjjhwx.cn

TS:   public / protected / private
来源：http://oo.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://zh.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tc.gzmigu.cn

Ruby: public / protected / private
来源：http://wh.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://eg.hnjuh.cn

[G11] getter / setter
来源：http://af.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://zp.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qm.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://dc.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://cs.lnxyls.cn

Java: public String getName() { return name; }
来源：http://cg.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wv.szxytkj.cn

Ruby: attr_accessor :name
来源：http://ss.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://we.shxzskj.cn

[G12] 对象转字符串
来源：http://mi.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://ne.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pf.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://au.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://fn.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://fk.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zt.nicolike.cn

Ruby: def to_s; @name; end
来源：http://tf.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://si.colortex.cn

[G13] 判断对象类型
来源：http://nh.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://ma.nszjky.cn

PHP:  $u instanceof User
来源：http://lv.muxihuayi.cn

JS:   u instanceof User
来源：http://hy.9csxet.cn

TS:   u instanceof User
来源：http://mp.bjjhwx.cn

Java: u instanceof User
来源：http://er.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kr.newstarts.cn

Ruby: u.is_a?(User)
来源：http://nc.szsharing.cn

C#:   u is User
来源：http://hx.hnjuh.cn

[G14] 数据类 / record
来源：http://rl.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zf.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://hj.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cb.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ek.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://pr.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://ak.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://er.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://st.chemitech.net.cn

[G15] 枚举
来源：http://ri.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ca.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://it.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cf.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ae.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://zd.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ba.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://tf.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tu.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://mg.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pm.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://aq.szxytkj.cn

JS:   Object.entries(obj)
来源：http://hr.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://cb.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yi.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yg.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://mk.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://dl.shxzskj.cn

================================================================================
来源：http://yj.colortex.cn

H. 异常与错误处理
来源：http://fq.bjjhwx.cn

================================================================================
来源：http://sy.lnxyls.cn

[H01] try / catch 基础
来源：http://kx.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bj.panjiajie.cn


<!-- 参考信息 -->