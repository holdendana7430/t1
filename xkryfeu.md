代发 wailian999

Ruby: s.lines
来源：http://ng.gzmigu.cn

C#:   s.Split('\n')
来源：http://he.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://ek.asd995.cn

Py:   if not s:
来源：http://pk.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sk.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sl.szxytkj.cn

TS:   if (s === "") {}
来源：http://xw.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://mc.wgjwhj.cn

Go:   if s == "" {}
来源：http://ss.haigaiapp.cn

Ruby: if s.empty?
来源：http://ua.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nx.szxytkj.cn

[E21] 超长截断加省略号
来源：http://pj.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fd.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yq.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xy.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ec.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ym.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://bf.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bj.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uk.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://md.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://in.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://js.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iu.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tp.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://av.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gv.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://pc.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dt.jctech888.com.cn

================================================================================
来源：http://ls.newstarts.cn

F. 文件与目录
来源：http://cc.jctech888.com.cn

================================================================================
来源：http://mf.shtwfgs.cn

[F01] 读取整个文件
来源：http://da.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cj.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://li.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://za.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dy.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://os.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tv.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://uc.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://de.shxzskj.cn

[F02] 逐行读取文件
来源：http://pk.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nz.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nz.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mo.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ul.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gk.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cw.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vt.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ge.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://hc.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dz.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://py.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lh.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yk.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kq.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uf.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://vt.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wk.wgjwhj.cn

[F04] 追加写入文件
来源：http://dc.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://te.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kp.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uf.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ng.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zv.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hv.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wi.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gn.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://so.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zd.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://cu.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ei.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://wf.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qb.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uz.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://gp.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://jm.shxzskj.cn

[F06] 删除文件
来源：http://ek.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://as.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ne.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ie.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ul.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bb.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://um.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://en.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://dz.nicolike.cn

[F07] 创建目录（含多级）
来源：http://uu.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wt.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dt.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wd.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tk.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ap.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vj.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dz.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://af.wgjwhj.cn

[F08] 遍历目录
来源：http://jv.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eh.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hw.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://kj.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://er.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zt.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fy.szsharing.cn

Ruby: Dir.children("dir")
来源：http://en.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://zt.asd995.cn

[F09] 获取文件大小
来源：http://kw.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://ob.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://ph.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://da.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://bo.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bl.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://in.521024.cn

Ruby: File.size("a.txt")
来源：http://oo.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://vx.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://wf.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uu.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ek.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zg.szsharing.cn

TS:   path.extname("a.txt")
来源：http://gk.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gu.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bo.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zp.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uw.szxytkj.cn

[F11] 复制与移动文件
来源：http://pm.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jy.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pi.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xi.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qg.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ik.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sg.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mb.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pr.wgjwhj.cn

[F12] CSV 读写
来源：http://pv.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yo.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xi.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jg.gzmigu.cn

TS:   // 同上
来源：http://nb.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wm.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fb.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rd.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ot.yuntaijiaju.cn

================================================================================
来源：http://oy.shtwfgs.cn

G. 面向对象
来源：http://xe.jctech888.com.cn

================================================================================
来源：http://jn.haigaiapp.cn

[G01] 定义类
来源：http://hd.szxytkj.cn

Py:   class User: pass
来源：http://xg.gzmigu.cn

PHP:  class User {}
来源：http://dr.gzmigu.cn

JS:   class User {}
来源：http://ca.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ii.yuntaijiaju.cn

Java: class User {}
来源：http://vs.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://rk.hnjuh.cn

Ruby: class User; end
来源：http://nc.yuntaijiaju.cn

C#:   class User {}
来源：http://gs.shxzskj.cn

[G02] 构造函数
来源：http://xz.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://gi.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oy.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://fp.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://xp.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://jk.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pr.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://no.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://fc.yuntaijiaju.cn

[G03] 实例属性
来源：http://va.colortex.cn

Py:   self.name = "x"
来源：http://ab.hahajie.cn

PHP:  public string $name = "x";
来源：http://np.nicolike.cn

JS:   this.name = "x";
来源：http://yg.9csxet.cn

TS:   name: string = "x";
来源：http://lc.huixiangedu.cn

Java: private String name;
来源：http://ch.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yc.wgjwhj.cn

Ruby: @name = "x"
来源：http://jq.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://lf.chemitech.net.cn

[G04] 定义方法
来源：http://ss.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://fi.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zn.colortex.cn

JS:   greet() { return this.name; }
来源：http://uc.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://oo.shxzukj.cn

Java: String greet() { return name; }
来源：http://xp.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zy.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://hf.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://sa.asd995.cn

[G05] 继承
来源：http://ok.shxzukj.cn

Py:   class Admin(User): pass
来源：http://dd.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://mg.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://vc.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://gz.lnxyls.cn

Java: class Admin extends User {}
来源：http://ax.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yt.nicolike.cn

Ruby: class Admin < User; end
来源：http://tv.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://el.shtwfgs.cn

[G06] 重写方法
来源：http://ij.asd995.cn

Py:   def greet(self): return "admin"
来源：http://lh.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kf.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://vu.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://tb.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xs.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ql.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://hq.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://vr.panjiajie.cn

[G07] 调用父类方法
来源：http://ba.nicolike.cn

Py:   super().greet()
来源：http://hf.asd995.cn

PHP:  parent::greet();
来源：http://uv.haigaiapp.cn

JS:   super.greet();
来源：http://wk.jianghongdianzi.cn

TS:   super.greet();
来源：http://qw.newstarts.cn

Java: super.greet();
来源：http://pb.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zy.jianghongdianzi.cn

Ruby: super
来源：http://of.huixiangedu.cn

C#:   base.Greet();
来源：http://ew.shtwfgs.cn

[G08] 静态方法与属性
来源：http://wp.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ai.chemitech.net.cn

PHP:  public static function f() {}
来源：http://zv.haigaiapp.cn

JS:   static f() {}
来源：http://uz.jctech888.com.cn

TS:   static f(): void {}
来源：http://bp.hnjuh.cn

Java: static void f() {}
来源：http://on.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sc.hahajie.cn

Ruby: def self.f; end
来源：http://me.newstarts.cn

C#:   public static void F() {}
来源：http://rk.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://vj.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://an.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ie.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lt.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://av.nicolike.cn

Java: interface Shape { double area(); }
来源：http://ua.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://qt.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://or.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://yk.szxytkj.cn

[G10] 访问控制
来源：http://qd.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://ln.bjjhwx.cn

PHP:  public / protected / private
来源：http://oz.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://zy.shxzskj.cn

TS:   public / protected / private
来源：http://io.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://bs.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ct.hnjuh.cn

Ruby: public / protected / private
来源：http://yt.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://um.shtwfgs.cn

[G11] getter / setter
来源：http://ww.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://th.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gc.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://ro.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://ia.szsharing.cn

Java: public String getName() { return name; }
来源：http://it.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ux.asd995.cn

Ruby: attr_accessor :name
来源：http://za.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://ea.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://xa.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://wv.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ll.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://px.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://cr.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://hu.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nl.nicolike.cn

Ruby: def to_s; @name; end
来源：http://aa.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://mn.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ld.521024.cn

Py:   isinstance(u, User)
来源：http://xy.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://kf.colortex.cn

JS:   u instanceof User
来源：http://fy.szsharing.cn

TS:   u instanceof User
来源：http://zh.lnxyls.cn

Java: u instanceof User
来源：http://hr.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cq.asd995.cn

Ruby: u.is_a?(User)
来源：http://bk.yuntaijiaju.cn

C#:   u is User
来源：http://el.bookmarksfly.cn

[G14] 数据类 / record
来源：http://hd.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ar.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://si.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tg.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://cd.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://ld.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://cb.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qp.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://nb.muxihuayi.cn

[G15] 枚举
来源：http://iy.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pf.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rx.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yi.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yo.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://db.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sm.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://tu.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ox.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://br.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://az.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://vf.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ih.nicolike.cn

TS:   Object.entries(obj)
来源：http://it.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eb.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vv.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://xp.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ft.nicolike.cn

================================================================================
来源：http://bc.wgjwhj.cn

H. 异常与错误处理
来源：http://sz.shxzukj.cn

================================================================================
来源：http://mn.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://tx.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://te.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wg.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://il.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fa.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iw.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://va.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://do.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lf.nicolike.cn

[H02] finally / ensure 收尾
来源：http://wx.yuexingan06.cn


<!-- 参考信息 -->