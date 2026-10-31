代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://et.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vb.panjiajie.cn

TS:   if (s === "") {}
来源：http://lm.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://zr.chemitech.net.cn

Go:   if s == "" {}
来源：http://cw.9csxet.cn

Ruby: if s.empty?
来源：http://fz.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vh.szsharing.cn

[E21] 超长截断加省略号
来源：http://gt.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wt.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sy.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hq.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lo.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iq.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://or.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ko.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ir.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://lu.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hy.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vf.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fi.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lq.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ha.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://vu.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oz.shtwfgs.cn

================================================================================
来源：http://up.huixinmuqiang.cn

F. 文件与目录
来源：http://jt.yuexingan06.cn

================================================================================
来源：http://vq.jctech888.com.cn

[F01] 读取整个文件
来源：http://yi.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tn.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://dh.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ns.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cv.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jb.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cq.newstarts.cn

Ruby: File.read("a.txt")
来源：http://rq.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://li.hnjuh.cn

[F02] 逐行读取文件
来源：http://al.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uo.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kr.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vs.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aj.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ux.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xq.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vl.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ag.521024.cn

[F03] 写入文件（覆盖）
来源：http://ek.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mc.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sn.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gd.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jl.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aw.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wf.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://st.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kk.9csxet.cn

[F04] 追加写入文件
来源：http://fl.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ko.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nc.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bh.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yk.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fg.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hk.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uf.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://kr.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eq.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://hs.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ir.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://pi.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ej.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bi.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://bt.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://xz.shxzskj.cn

[F06] 删除文件
来源：http://jx.521024.cn

Py:   os.remove("a.txt")
来源：http://me.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://xq.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vc.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://et.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vo.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://za.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://th.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://pa.9csxet.cn

[F07] 创建目录（含多级）
来源：http://ba.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aa.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://or.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pt.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fs.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ii.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kq.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tf.nicolike.cn

[F08] 遍历目录
来源：http://oc.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wo.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gx.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://wm.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://th.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bm.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gj.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://nl.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://rg.asd995.cn

[F09] 获取文件大小
来源：http://qw.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://ey.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://qf.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://zk.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://zp.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sq.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ds.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://rg.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://tu.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://kb.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pa.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ds.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://je.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://hf.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://af.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kr.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hn.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ie.shtwfgs.cn

[F11] 复制与移动文件
来源：http://jr.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fl.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ik.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cy.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zt.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mt.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jg.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://av.shtwfgs.cn

[F12] CSV 读写
来源：http://sx.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bc.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://no.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fq.shxzskj.cn

TS:   // 同上
来源：http://tv.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ui.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rk.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://km.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kj.panjiajie.cn

================================================================================
来源：http://aj.hnjuh.cn

G. 面向对象
来源：http://by.wgjwhj.cn

================================================================================
来源：http://ya.colortex.cn

[G01] 定义类
来源：http://zf.lnxyls.cn

Py:   class User: pass
来源：http://vw.szxytkj.cn

PHP:  class User {}
来源：http://ju.9csxet.cn

JS:   class User {}
来源：http://jl.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://sm.bjjhwx.cn

Java: class User {}
来源：http://pb.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://ua.szxytkj.cn

Ruby: class User; end
来源：http://bz.wgjwhj.cn

C#:   class User {}
来源：http://fh.nicolike.cn

[G02] 构造函数
来源：http://vk.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://yu.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://we.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://mo.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://te.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://rd.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mt.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://to.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://va.newstarts.cn

[G03] 实例属性
来源：http://wz.gzmigu.cn

Py:   self.name = "x"
来源：http://vc.panjiajie.cn

PHP:  public string $name = "x";
来源：http://ef.muxihuayi.cn

JS:   this.name = "x";
来源：http://pk.bjjhwx.cn

TS:   name: string = "x";
来源：http://qh.szsharing.cn

Java: private String name;
来源：http://zw.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gv.hnjuh.cn

Ruby: @name = "x"
来源：http://ei.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://jm.szsharing.cn

[G04] 定义方法
来源：http://lm.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ov.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iq.9csxet.cn

JS:   greet() { return this.name; }
来源：http://pf.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://to.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://sp.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hu.szxytkj.cn

Ruby: def greet; @name; end
来源：http://ky.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://qu.yuexingan06.cn

[G05] 继承
来源：http://xm.hnjuh.cn

Py:   class Admin(User): pass
来源：http://gf.nicolike.cn

PHP:  class Admin extends User {}
来源：http://lw.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://lc.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://xm.9csxet.cn

Java: class Admin extends User {}
来源：http://ur.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ha.newstarts.cn

Ruby: class Admin < User; end
来源：http://yp.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://vu.bjjhwx.cn

[G06] 重写方法
来源：http://tz.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://oo.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jg.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://hg.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://py.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oo.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sz.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://vs.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://hh.huixiangedu.cn

[G07] 调用父类方法
来源：http://tm.hnjuh.cn

Py:   super().greet()
来源：http://wq.colortex.cn

PHP:  parent::greet();
来源：http://is.bjjhwx.cn

JS:   super.greet();
来源：http://ep.jianghongdianzi.cn

TS:   super.greet();
来源：http://cl.huanxung.cn

Java: super.greet();
来源：http://vh.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vg.huanxung.cn

Ruby: super
来源：http://pd.chemitech.net.cn

C#:   base.Greet();
来源：http://eh.gzmigu.cn

[G08] 静态方法与属性
来源：http://qu.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cx.haigaiapp.cn

PHP:  public static function f() {}
来源：http://sb.newstarts.cn

JS:   static f() {}
来源：http://hg.szsharing.cn

TS:   static f(): void {}
来源：http://wb.huanxung.cn

Java: static void f() {}
来源：http://nl.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hr.haigaiapp.cn

Ruby: def self.f; end
来源：http://wp.jctech888.com.cn

C#:   public static void F() {}
来源：http://ga.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://co.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://mp.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yu.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ok.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://hv.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://pu.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://jm.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gl.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://se.shxzskj.cn

[G10] 访问控制
来源：http://lh.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ov.shxzskj.cn

PHP:  public / protected / private
来源：http://lf.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://tv.huanxung.cn

TS:   public / protected / private
来源：http://is.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://di.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fl.jctech888.com.cn

Ruby: public / protected / private
来源：http://up.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://fw.9csxet.cn

[G11] getter / setter
来源：http://it.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://wi.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fr.huanxung.cn

JS:   get name() { return this._name; }
来源：http://zs.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://yt.lnxyls.cn

Java: public String getName() { return name; }
来源：http://fh.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ur.lnxyls.cn

Ruby: attr_accessor :name
来源：http://pc.colortex.cn

C#:   public string Name { get; set; }
来源：http://ma.bjjhwx.cn

[G12] 对象转字符串
来源：http://uj.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://sp.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tb.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://lp.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://oi.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://hj.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wh.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://tf.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://cu.521024.cn

[G13] 判断对象类型
来源：http://rn.szsharing.cn

Py:   isinstance(u, User)
来源：http://zw.colortex.cn

PHP:  $u instanceof User
来源：http://om.szsharing.cn

JS:   u instanceof User
来源：http://dc.huixinmuqiang.cn

TS:   u instanceof User
来源：http://hk.yuexingan06.cn

Java: u instanceof User
来源：http://dk.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wp.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://tf.nicolike.cn

C#:   u is User
来源：http://od.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://ox.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tp.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://qm.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ko.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://jp.asd995.cn

Java: record User(String name, int age) {}
来源：http://mv.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://th.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uo.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://vd.panjiajie.cn

[G15] 枚举
来源：http://at.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uo.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wp.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cn.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hv.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://vq.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://om.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://yy.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nq.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://cb.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://af.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://dv.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://xe.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://cf.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://su.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xq.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://qx.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://wa.jctech888.com.cn

H. 异常与错误处理
来源：http://qy.asd995.cn

================================================================================
来源：http://jo.wgjwhj.cn

[H01] try / catch 基础
来源：http://hp.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://it.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://px.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fh.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://is.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bw.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cq.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rh.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ld.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://fk.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uo.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sw.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ah.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://id.chemitech.net.cn


<!-- 参考信息 -->