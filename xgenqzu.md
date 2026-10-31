代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yr.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wk.yuexingan06.cn

TS:   if (s === "") {}
来源：http://zh.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://tf.nszjky.cn

Go:   if s == "" {}
来源：http://up.newstarts.cn

Ruby: if s.empty?
来源：http://qt.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sa.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://fh.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ni.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hu.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ak.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qp.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gr.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://qs.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wk.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jj.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://it.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://no.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sl.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ef.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ad.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nz.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://db.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tl.haigaiapp.cn

================================================================================
来源：http://vh.jctech888.com.cn

F. 文件与目录
来源：http://lv.bjjhwx.cn

================================================================================
来源：http://vg.haigaiapp.cn

[F01] 读取整个文件
来源：http://nz.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tk.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://lz.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ip.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://va.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oz.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vv.asd995.cn

Ruby: File.read("a.txt")
来源：http://ws.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://mm.nszjky.cn

[F02] 逐行读取文件
来源：http://fi.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eb.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qf.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rf.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ow.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jt.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oa.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cp.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lc.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://iy.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xg.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fp.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ug.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rl.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fg.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ul.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rb.shxzukj.cn

[F04] 追加写入文件
来源：http://wv.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jd.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jh.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jb.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://im.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://an.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ap.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ks.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ec.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://by.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://as.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://we.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://nl.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://bt.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kc.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ky.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://rg.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://wx.szxytkj.cn

[F06] 删除文件
来源：http://rs.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://hr.huanxung.cn

PHP:  unlink("a.txt");
来源：http://xp.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fx.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yj.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ro.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://fh.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://yk.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://sa.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://dc.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xi.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hj.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ej.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aw.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wc.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://io.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jk.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gf.gzmigu.cn

[F08] 遍历目录
来源：http://mv.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jh.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ha.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://kl.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://ts.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uq.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kw.huanxung.cn

Ruby: Dir.children("dir")
来源：http://kd.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://jx.9csxet.cn

[F09] 获取文件大小
来源：http://of.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://fy.huanxung.cn

PHP:  filesize("a.txt");
来源：http://er.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://mm.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://en.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sz.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ol.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ql.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://we.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ht.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qi.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ph.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ou.521024.cn

TS:   path.extname("a.txt")
来源：http://rp.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bs.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://di.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://on.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gb.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://bk.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mx.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vl.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bn.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vh.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xs.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pd.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hv.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wl.szxytkj.cn

[F12] CSV 读写
来源：http://ec.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qv.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yh.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.szsharing.cn

TS:   // 同上
来源：http://aj.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uy.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sj.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wx.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nb.asd995.cn

================================================================================
来源：http://dq.yuexingan06.cn

G. 面向对象
来源：http://xq.huanxung.cn

================================================================================
来源：http://jc.9csxet.cn

[G01] 定义类
来源：http://vj.szxytkj.cn

Py:   class User: pass
来源：http://oc.hahajie.cn

PHP:  class User {}
来源：http://zv.wgjwhj.cn

JS:   class User {}
来源：http://gx.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://fm.yuntaijiaju.cn

Java: class User {}
来源：http://ru.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://yg.jianghongdianzi.cn

Ruby: class User; end
来源：http://bk.nszjky.cn

C#:   class User {}
来源：http://kj.huixinmuqiang.cn

[G02] 构造函数
来源：http://pq.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://hf.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://om.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://uu.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://an.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://qt.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://di.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://cm.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://za.shxzukj.cn

[G03] 实例属性
来源：http://yz.shxzskj.cn

Py:   self.name = "x"
来源：http://dd.newstarts.cn

PHP:  public string $name = "x";
来源：http://ss.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://eo.muxihuayi.cn

TS:   name: string = "x";
来源：http://ud.nicolike.cn

Java: private String name;
来源：http://gw.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dm.nicolike.cn

Ruby: @name = "x"
来源：http://dx.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://uf.lnxyls.cn

[G04] 定义方法
来源：http://hm.hahajie.cn

Py:   def greet(self): return self.name
来源：http://jn.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://up.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://ck.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://vw.521024.cn

Java: String greet() { return name; }
来源：http://gt.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xd.hahajie.cn

Ruby: def greet; @name; end
来源：http://fn.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ps.szxytkj.cn

[G05] 继承
来源：http://bs.nszjky.cn

Py:   class Admin(User): pass
来源：http://sn.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://rq.lnxyls.cn

JS:   class Admin extends User {}
来源：http://rb.gzmigu.cn

TS:   class Admin extends User {}
来源：http://gp.newstarts.cn

Java: class Admin extends User {}
来源：http://jt.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://io.nszjky.cn

Ruby: class Admin < User; end
来源：http://hl.9csxet.cn

C#:   class Admin : User {}
来源：http://mb.asd995.cn

[G06] 重写方法
来源：http://cy.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://ot.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jb.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://pq.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://zw.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://oj.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zf.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://lj.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://yy.jctech888.com.cn

[G07] 调用父类方法
来源：http://pm.muxihuayi.cn

Py:   super().greet()
来源：http://tx.9csxet.cn

PHP:  parent::greet();
来源：http://ha.bjjhwx.cn

JS:   super.greet();
来源：http://ci.szsharing.cn

TS:   super.greet();
来源：http://cu.jctech888.com.cn

Java: super.greet();
来源：http://hy.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://st.nicolike.cn

Ruby: super
来源：http://il.haigaiapp.cn

C#:   base.Greet();
来源：http://vp.shtwfgs.cn

[G08] 静态方法与属性
来源：http://oo.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gh.gzmigu.cn

PHP:  public static function f() {}
来源：http://xw.lnxyls.cn

JS:   static f() {}
来源：http://zx.panjiajie.cn

TS:   static f(): void {}
来源：http://eo.newstarts.cn

Java: static void f() {}
来源：http://nk.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qq.panjiajie.cn

Ruby: def self.f; end
来源：http://zq.hahajie.cn

C#:   public static void F() {}
来源：http://jz.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://hw.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://kh.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xd.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zc.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://tg.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://zp.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://he.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nh.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://hs.bookmarksfly.cn

[G10] 访问控制
来源：http://ua.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://su.shtwfgs.cn

PHP:  public / protected / private
来源：http://nn.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://zv.shxzukj.cn

TS:   public / protected / private
来源：http://vo.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://ep.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://az.szsharing.cn

Ruby: public / protected / private
来源：http://ie.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://bc.hahajie.cn

[G11] getter / setter
来源：http://ro.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://ey.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://je.hahajie.cn

JS:   get name() { return this._name; }
来源：http://bu.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://rz.szsharing.cn

Java: public String getName() { return name; }
来源：http://tg.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jo.asd995.cn

Ruby: attr_accessor :name
来源：http://hf.newstarts.cn

C#:   public string Name { get; set; }
来源：http://th.huixiangedu.cn

[G12] 对象转字符串
来源：http://kt.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://dj.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nu.newstarts.cn

JS:   toString() { return this.name; }
来源：http://mu.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ns.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://pc.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nm.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://it.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://gs.nszjky.cn

[G13] 判断对象类型
来源：http://nk.521024.cn

Py:   isinstance(u, User)
来源：http://oy.colortex.cn

PHP:  $u instanceof User
来源：http://zy.chemitech.net.cn

JS:   u instanceof User
来源：http://hy.nszjky.cn

TS:   u instanceof User
来源：http://ic.nicolike.cn

Java: u instanceof User
来源：http://vz.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fv.hahajie.cn

Ruby: u.is_a?(User)
来源：http://uq.shxzskj.cn

C#:   u is User
来源：http://ll.9csxet.cn

[G14] 数据类 / record
来源：http://fl.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ov.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://eh.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cp.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://hm.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://jx.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://yq.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rx.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://uz.asd995.cn

[G15] 枚举
来源：http://eq.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ho.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zs.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://za.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fc.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://ei.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qt.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://xi.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lx.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://va.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vt.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://sx.lnxyls.cn

JS:   Object.entries(obj)
来源：http://pf.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://bw.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rr.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yz.szsharing.cn

Ruby: obj.instance_variables
来源：http://ca.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ys.szxytkj.cn

================================================================================
来源：http://bm.nszjky.cn

H. 异常与错误处理
来源：http://gw.nszjky.cn

================================================================================
来源：http://iu.newstarts.cn

[H01] try / catch 基础
来源：http://rq.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lu.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pq.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wg.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cd.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ty.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vv.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://an.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bb.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://kz.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iz.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ku.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qu.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oe.chemitech.net.cn


<!-- 参考信息 -->