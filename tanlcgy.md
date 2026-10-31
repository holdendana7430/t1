代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://nj.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://bu.colortex.cn

Java: s.lines().toList()
来源：http://wa.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ht.shxzskj.cn

Ruby: s.lines
来源：http://pu.hahajie.cn

C#:   s.Split('\n')
来源：http://ga.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://ux.muxihuayi.cn

Py:   if not s:
来源：http://yo.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wr.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dg.szxytkj.cn

TS:   if (s === "") {}
来源：http://oa.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://oj.huanxung.cn

Go:   if s == "" {}
来源：http://kc.yuexingan06.cn

Ruby: if s.empty?
来源：http://pa.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cx.521024.cn

[E21] 超长截断加省略号
来源：http://pg.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gn.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qv.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wf.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kn.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ns.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://wu.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ce.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xg.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ns.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ff.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ea.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://il.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kc.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qz.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lp.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://fq.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sq.shtwfgs.cn

================================================================================
来源：http://ks.hahajie.cn

F. 文件与目录
来源：http://es.newstarts.cn

================================================================================
来源：http://sm.hahajie.cn

[F01] 读取整个文件
来源：http://ur.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vg.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://mv.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hh.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pv.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kj.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tu.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://rw.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://nr.lnxyls.cn

[F02] 逐行读取文件
来源：http://ow.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sg.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eg.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ga.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gw.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jf.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eo.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jq.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hg.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://oj.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kd.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eh.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xv.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ll.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fx.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uk.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://kk.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mp.haigaiapp.cn

[F04] 追加写入文件
来源：http://ko.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mt.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iq.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ec.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mi.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://by.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jl.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gy.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ti.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://dy.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ee.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://kg.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://gj.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://kd.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ce.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zz.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://ff.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://cq.521024.cn

[F06] 删除文件
来源：http://bx.szsharing.cn

Py:   os.remove("a.txt")
来源：http://az.hahajie.cn

PHP:  unlink("a.txt");
来源：http://fc.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uo.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aw.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gc.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://ak.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://vi.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://rm.hahajie.cn

[F07] 创建目录（含多级）
来源：http://jo.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ey.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yk.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lu.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ti.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bj.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ol.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vc.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cb.jianghongdianzi.cn

[F08] 遍历目录
来源：http://nb.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jj.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xh.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://sz.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://xu.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://of.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jz.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://tu.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://yl.colortex.cn

[F09] 获取文件大小
来源：http://fp.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://ah.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://nd.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ne.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tt.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ka.nicolike.cn

Ruby: File.size("a.txt")
来源：http://kx.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://oa.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://nn.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fn.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ma.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ma.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://kt.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nh.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qa.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hw.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rl.shtwfgs.cn

[F11] 复制与移动文件
来源：http://mc.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qy.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wo.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pe.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ow.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ii.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uk.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iu.newstarts.cn

[F12] CSV 读写
来源：http://xd.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ki.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dv.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vm.bookmarksfly.cn

TS:   // 同上
来源：http://lp.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ge.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ua.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cy.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lf.9csxet.cn

================================================================================
来源：http://ge.haigaiapp.cn

G. 面向对象
来源：http://rb.jianghongdianzi.cn

================================================================================
来源：http://fp.shxzukj.cn

[G01] 定义类
来源：http://xh.shxzskj.cn

Py:   class User: pass
来源：http://gp.yuntaijiaju.cn

PHP:  class User {}
来源：http://ng.panjiajie.cn

JS:   class User {}
来源：http://os.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://zi.huanxung.cn

Java: class User {}
来源：http://mm.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://vc.szsharing.cn

Ruby: class User; end
来源：http://rh.huixiangedu.cn

C#:   class User {}
来源：http://xb.szsharing.cn

[G02] 构造函数
来源：http://bk.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://wx.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://ca.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://sz.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://mm.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://gh.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pp.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://kd.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://us.shxzukj.cn

[G03] 实例属性
来源：http://ds.szxytkj.cn

Py:   self.name = "x"
来源：http://uw.newstarts.cn

PHP:  public string $name = "x";
来源：http://yn.hnjuh.cn

JS:   this.name = "x";
来源：http://sw.chemitech.net.cn

TS:   name: string = "x";
来源：http://df.9csxet.cn

Java: private String name;
来源：http://av.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://it.9csxet.cn

Ruby: @name = "x"
来源：http://mn.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://kd.hnjuh.cn

[G04] 定义方法
来源：http://hi.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://oq.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jt.newstarts.cn

JS:   greet() { return this.name; }
来源：http://ld.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ui.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://us.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pz.nszjky.cn

Ruby: def greet; @name; end
来源：http://vd.nicolike.cn

C#:   public string Greet() => Name;
来源：http://wt.gzmigu.cn

[G05] 继承
来源：http://bg.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://lw.colortex.cn

PHP:  class Admin extends User {}
来源：http://qj.521024.cn

JS:   class Admin extends User {}
来源：http://lk.huanxung.cn

TS:   class Admin extends User {}
来源：http://vp.haigaiapp.cn

Java: class Admin extends User {}
来源：http://ae.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ng.panjiajie.cn

Ruby: class Admin < User; end
来源：http://jb.newstarts.cn

C#:   class Admin : User {}
来源：http://pj.panjiajie.cn

[G06] 重写方法
来源：http://yg.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://zc.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tc.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://gm.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://zr.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://qt.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ki.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://wm.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ny.chemitech.net.cn

[G07] 调用父类方法
来源：http://he.yuntaijiaju.cn

Py:   super().greet()
来源：http://hq.muxihuayi.cn

PHP:  parent::greet();
来源：http://mj.shtwfgs.cn

JS:   super.greet();
来源：http://di.jianghongdianzi.cn

TS:   super.greet();
来源：http://yg.panjiajie.cn

Java: super.greet();
来源：http://tl.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ak.wgjwhj.cn

Ruby: super
来源：http://jf.huanxung.cn

C#:   base.Greet();
来源：http://ew.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://ot.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bv.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://sb.yuexingan06.cn

JS:   static f() {}
来源：http://oc.jctech888.com.cn

TS:   static f(): void {}
来源：http://mt.hahajie.cn

Java: static void f() {}
来源：http://gp.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cx.haigaiapp.cn

Ruby: def self.f; end
来源：http://in.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://da.9csxet.cn

[G09] 接口 / 抽象类
来源：http://yj.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://fb.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tg.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jb.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://ef.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://te.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://br.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://za.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://ah.521024.cn

[G10] 访问控制
来源：http://za.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://vs.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://kc.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://we.nszjky.cn

TS:   public / protected / private
来源：http://or.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ni.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dk.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://nn.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://pk.panjiajie.cn

[G11] getter / setter
来源：http://id.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ch.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qc.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://rc.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://tt.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://gr.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bt.colortex.cn

Ruby: attr_accessor :name
来源：http://gn.nicolike.cn

C#:   public string Name { get; set; }
来源：http://za.nszjky.cn

[G12] 对象转字符串
来源：http://kn.521024.cn

Py:   def __str__(self): return self.name
来源：http://io.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yx.nszjky.cn

JS:   toString() { return this.name; }
来源：http://zx.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://qr.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://va.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uo.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://iv.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://de.521024.cn

[G13] 判断对象类型
来源：http://ad.nszjky.cn

Py:   isinstance(u, User)
来源：http://qo.gzmigu.cn

PHP:  $u instanceof User
来源：http://dx.nszjky.cn

JS:   u instanceof User
来源：http://ps.nszjky.cn

TS:   u instanceof User
来源：http://pf.bookmarksfly.cn

Java: u instanceof User
来源：http://ki.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bd.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ak.newstarts.cn

C#:   u is User
来源：http://ke.shxzskj.cn

[G14] 数据类 / record
来源：http://bb.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ie.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://ts.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fv.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://nd.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://dp.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://et.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ht.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://hk.nszjky.cn

[G15] 枚举
来源：http://ap.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://og.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pp.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yo.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sp.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://to.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hq.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://bb.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ca.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://xj.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jl.asd995.cn

PHP:  get_object_vars($obj);
来源：http://es.hnjuh.cn

JS:   Object.entries(obj)
来源：http://mu.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://ay.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jw.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lj.colortex.cn

Ruby: obj.instance_variables
来源：http://wv.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://mo.newstarts.cn

================================================================================
来源：http://cp.wgjwhj.cn

H. 异常与错误处理
来源：http://js.jianghongdianzi.cn

================================================================================
来源：http://ej.yuexingan06.cn

[H01] try / catch 基础
来源：http://or.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pv.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jt.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yh.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://up.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ww.huixinmuqiang.cn


<!-- 参考信息 -->