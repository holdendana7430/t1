代发 wailian999

Ruby: s.lines
来源：http://ao.gzmigu.cn

C#:   s.Split('\n')
来源：http://cy.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://zz.haigaiapp.cn

Py:   if not s:
来源：http://wp.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oz.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bm.szxytkj.cn

TS:   if (s === "") {}
来源：http://ds.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ih.huixiangedu.cn

Go:   if s == "" {}
来源：http://tm.haigaiapp.cn

Ruby: if s.empty?
来源：http://nv.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sa.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://vq.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nw.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ko.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bc.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://az.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bz.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://jd.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ud.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sn.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://jl.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://st.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wt.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wh.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xi.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ml.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qh.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://mr.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xi.newstarts.cn

================================================================================
来源：http://od.hnjuh.cn

F. 文件与目录
来源：http://ki.szxytkj.cn

================================================================================
来源：http://ry.chemitech.net.cn

[F01] 读取整个文件
来源：http://nb.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://st.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://fo.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kw.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xa.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ue.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mr.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://xi.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://rm.panjiajie.cn

[F02] 逐行读取文件
来源：http://ku.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vm.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ft.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hc.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://np.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tx.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lx.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dc.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://je.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pi.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qu.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wy.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kp.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pk.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://un.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://vo.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wl.hahajie.cn

[F04] 追加写入文件
来源：http://yp.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lr.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wh.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ce.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kh.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qz.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rk.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pt.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uf.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://id.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bb.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://sb.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://mg.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://jb.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ny.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xq.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://mu.asd995.cn

C#:   File.Exists("a.txt")
来源：http://fo.shxzukj.cn

[F06] 删除文件
来源：http://vq.huanxung.cn

Py:   os.remove("a.txt")
来源：http://ki.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://pg.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ma.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vg.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fu.asd995.cn

Go:   os.Remove("a.txt")
来源：http://rj.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://yh.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://sa.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://du.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qh.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dt.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://al.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jy.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vh.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vb.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sa.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wn.hnjuh.cn

[F08] 遍历目录
来源：http://nz.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://en.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xi.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://ra.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://xv.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wb.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zn.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://wp.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://kn.huixiangedu.cn

[F09] 获取文件大小
来源：http://rw.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ju.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://ee.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://ag.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ql.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://by.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pw.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://qg.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ty.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://su.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sf.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bh.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zi.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://yn.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cm.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://om.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jg.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ke.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://tk.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uh.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yq.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gy.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uu.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ga.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oh.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tl.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pk.shtwfgs.cn

[F12] CSV 读写
来源：http://zr.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yc.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fd.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ep.gzmigu.cn

TS:   // 同上
来源：http://pg.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lq.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dq.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ym.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gs.huixinmuqiang.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

G. 面向对象
来源：http://dr.shxzukj.cn

================================================================================
来源：http://dx.nicolike.cn

[G01] 定义类
来源：http://sl.shxzskj.cn

Py:   class User: pass
来源：http://mv.shxzukj.cn

PHP:  class User {}
来源：http://kb.hahajie.cn

JS:   class User {}
来源：http://uh.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://gi.gzmigu.cn

Java: class User {}
来源：http://zk.nszjky.cn

Go:   type User struct { Name string }
来源：http://sw.asd995.cn

Ruby: class User; end
来源：http://en.huixinmuqiang.cn

C#:   class User {}
来源：http://kv.hahajie.cn

[G02] 构造函数
来源：http://tw.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://sz.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://cb.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://vf.colortex.cn

TS:   constructor(public name: string) {}
来源：http://mh.521024.cn

Java: User(String name) { this.name = name; }
来源：http://hk.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rp.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://wa.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://dg.panjiajie.cn

[G03] 实例属性
来源：http://oj.wgjwhj.cn

Py:   self.name = "x"
来源：http://nt.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://sb.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://mn.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://kj.yuntaijiaju.cn

Java: private String name;
来源：http://nm.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hl.asd995.cn

Ruby: @name = "x"
来源：http://fj.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://pl.shxzukj.cn

[G04] 定义方法
来源：http://eh.newstarts.cn

Py:   def greet(self): return self.name
来源：http://ca.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yj.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://wm.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://kt.nicolike.cn

Java: String greet() { return name; }
来源：http://sp.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rs.nicolike.cn

Ruby: def greet; @name; end
来源：http://af.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://ow.nszjky.cn

[G05] 继承
来源：http://tp.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://nr.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ug.9csxet.cn

JS:   class Admin extends User {}
来源：http://jb.szsharing.cn

TS:   class Admin extends User {}
来源：http://ie.521024.cn

Java: class Admin extends User {}
来源：http://mu.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ta.asd995.cn

Ruby: class Admin < User; end
来源：http://nd.muxihuayi.cn

C#:   class Admin : User {}
来源：http://ew.muxihuayi.cn

[G06] 重写方法
来源：http://lx.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ok.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rm.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://bu.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ec.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://gl.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ok.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://kh.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://cu.muxihuayi.cn

[G07] 调用父类方法
来源：http://yf.shxzukj.cn

Py:   super().greet()
来源：http://tk.haigaiapp.cn

PHP:  parent::greet();
来源：http://ns.jctech888.com.cn

JS:   super.greet();
来源：http://ji.gzmigu.cn

TS:   super.greet();
来源：http://cn.huixiangedu.cn

Java: super.greet();
来源：http://rt.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lx.lnxyls.cn

Ruby: super
来源：http://zp.huixinmuqiang.cn

C#:   base.Greet();
来源：http://nu.bjjhwx.cn

[G08] 静态方法与属性
来源：http://kd.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ze.panjiajie.cn

PHP:  public static function f() {}
来源：http://dj.chemitech.net.cn

JS:   static f() {}
来源：http://ym.muxihuayi.cn

TS:   static f(): void {}
来源：http://vk.muxihuayi.cn

Java: static void f() {}
来源：http://cp.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zj.panjiajie.cn

Ruby: def self.f; end
来源：http://yd.hnjuh.cn

C#:   public static void F() {}
来源：http://hv.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://db.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://nq.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://li.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ap.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://eh.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://gx.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://gn.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ji.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://iv.chemitech.net.cn

[G10] 访问控制
来源：http://fb.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ph.shtwfgs.cn

PHP:  public / protected / private
来源：http://ui.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://sd.yuntaijiaju.cn

TS:   public / protected / private
来源：http://xk.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://kc.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://it.bjjhwx.cn

Ruby: public / protected / private
来源：http://zp.asd995.cn

C#:   public / protected / private / internal
来源：http://gn.9csxet.cn

[G11] getter / setter
来源：http://ac.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://kg.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vy.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://rb.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://jt.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://ka.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jp.asd995.cn

Ruby: attr_accessor :name
来源：http://dp.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ip.colortex.cn

[G12] 对象转字符串
来源：http://ha.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://dj.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fa.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://ut.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://pr.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://gq.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://az.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://ve.521024.cn

C#:   public override string ToString() => Name;
来源：http://fx.shtwfgs.cn

[G13] 判断对象类型
来源：http://ym.huanxung.cn

Py:   isinstance(u, User)
来源：http://jr.jctech888.com.cn

PHP:  $u instanceof User
来源：http://na.gzmigu.cn

JS:   u instanceof User
来源：http://gc.panjiajie.cn

TS:   u instanceof User
来源：http://em.huixinmuqiang.cn

Java: u instanceof User
来源：http://cb.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ra.nszjky.cn

Ruby: u.is_a?(User)
来源：http://hf.jianghongdianzi.cn

C#:   u is User
来源：http://ni.asd995.cn

[G14] 数据类 / record
来源：http://vt.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://xx.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hl.521024.cn

TS:   type User = { name: string; age: number };
来源：http://ou.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://hi.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ka.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ar.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://wj.jianghongdianzi.cn

[G15] 枚举
来源：http://os.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://la.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vb.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://za.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://st.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://wy.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xu.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://kp.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ni.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://un.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ry.asd995.cn

PHP:  get_object_vars($obj);
来源：http://cx.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://zp.9csxet.cn

TS:   Object.entries(obj)
来源：http://ww.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lk.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ch.nszjky.cn

Ruby: obj.instance_variables
来源：http://nf.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ou.yuexingan06.cn

================================================================================
来源：http://dv.shtwfgs.cn

H. 异常与错误处理
来源：http://rh.521024.cn

================================================================================
来源：http://td.bjjhwx.cn

[H01] try / catch 基础
来源：http://yt.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hr.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fq.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jd.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wr.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ku.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xy.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://db.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yo.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://vr.chemitech.net.cn


<!-- 参考信息 -->