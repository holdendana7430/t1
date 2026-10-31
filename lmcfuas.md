代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://eq.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://hw.bjjhwx.cn

Java: s.lines().toList()
来源：http://jw.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://ca.colortex.cn

Ruby: s.lines
来源：http://xn.lnxyls.cn

C#:   s.Split('\n')
来源：http://ln.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ma.lnxyls.cn

Py:   if not s:
来源：http://it.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ac.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cn.hnjuh.cn

TS:   if (s === "") {}
来源：http://xq.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ts.huanxung.cn

Go:   if s == "" {}
来源：http://ru.szsharing.cn

Ruby: if s.empty?
来源：http://ij.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://be.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://yc.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wb.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vj.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ol.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qm.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ax.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://lv.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wh.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sk.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://os.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hs.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qb.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://br.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ny.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ko.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://gr.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ci.nicolike.cn

================================================================================
来源：http://dw.haigaiapp.cn

F. 文件与目录
来源：http://fk.newstarts.cn

================================================================================
来源：http://lz.szsharing.cn

[F01] 读取整个文件
来源：http://ut.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wv.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://br.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ie.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ux.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jw.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ka.asd995.cn

Ruby: File.read("a.txt")
来源：http://ow.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://ls.lnxyls.cn

[F02] 逐行读取文件
来源：http://bj.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pr.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xf.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gc.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fr.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gq.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sj.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://as.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mm.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://gu.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yj.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aq.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xd.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fh.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mr.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ev.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://ff.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tc.521024.cn

[F04] 追加写入文件
来源：http://nm.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uz.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jj.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cy.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xj.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://no.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oj.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yq.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hl.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://jx.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tv.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://gy.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://yh.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://rw.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://me.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gx.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://gy.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://gg.nszjky.cn

[F06] 删除文件
来源：http://le.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://vm.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://qp.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hk.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rh.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hf.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://an.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://st.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://hw.521024.cn

[F07] 创建目录（含多级）
来源：http://js.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nv.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://if.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wq.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ck.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://om.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ev.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qo.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vc.muxihuayi.cn

[F08] 遍历目录
来源：http://hc.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ee.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mk.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://ok.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://wj.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lv.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jv.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://si.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://ws.gzmigu.cn

[F09] 获取文件大小
来源：http://mr.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://br.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://ug.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://as.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ms.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ka.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ar.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://se.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://bm.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://yk.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ji.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ns.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sd.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://yt.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ct.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rt.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wk.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fl.shtwfgs.cn

[F11] 复制与移动文件
来源：http://sb.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bq.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vz.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ii.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bx.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cn.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qu.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dy.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hl.wgjwhj.cn

[F12] CSV 读写
来源：http://lt.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yh.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ar.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bl.szxytkj.cn

TS:   // 同上
来源：http://ny.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ww.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://si.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ew.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kp.bookmarksfly.cn

================================================================================
来源：http://wu.shxzskj.cn

G. 面向对象
来源：http://ae.lnxyls.cn

================================================================================
来源：http://ja.nszjky.cn

[G01] 定义类
来源：http://pg.wgjwhj.cn

Py:   class User: pass
来源：http://jd.shxzskj.cn

PHP:  class User {}
来源：http://op.lnxyls.cn

JS:   class User {}
来源：http://nw.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ol.szsharing.cn

Java: class User {}
来源：http://yk.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://uf.shtwfgs.cn

Ruby: class User; end
来源：http://im.521024.cn

C#:   class User {}
来源：http://sy.hahajie.cn

[G02] 构造函数
来源：http://gs.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://wo.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://mo.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://bu.asd995.cn

TS:   constructor(public name: string) {}
来源：http://zx.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://mt.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xc.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://tq.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://ct.jctech888.com.cn

[G03] 实例属性
来源：http://ct.shxzskj.cn

Py:   self.name = "x"
来源：http://ov.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://yn.colortex.cn

JS:   this.name = "x";
来源：http://du.nszjky.cn

TS:   name: string = "x";
来源：http://vn.chemitech.net.cn

Java: private String name;
来源：http://hq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cn.asd995.cn

Ruby: @name = "x"
来源：http://ho.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://iu.panjiajie.cn

[G04] 定义方法
来源：http://bz.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://ji.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nv.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://cu.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://lw.chemitech.net.cn

Java: String greet() { return name; }
来源：http://nq.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lx.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://sz.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://wl.wgjwhj.cn

[G05] 继承
来源：http://gz.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://jz.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://wh.shxzskj.cn

JS:   class Admin extends User {}
来源：http://vk.colortex.cn

TS:   class Admin extends User {}
来源：http://pq.muxihuayi.cn

Java: class Admin extends User {}
来源：http://ar.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://is.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://oq.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ac.haigaiapp.cn

[G06] 重写方法
来源：http://ps.colortex.cn

Py:   def greet(self): return "admin"
来源：http://oa.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dk.521024.cn

JS:   greet() { return "admin"; }
来源：http://st.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://zl.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://nv.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oq.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://kx.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://wa.huanxung.cn

[G07] 调用父类方法
来源：http://ki.yuntaijiaju.cn

Py:   super().greet()
来源：http://ag.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://bo.9csxet.cn

JS:   super.greet();
来源：http://ix.huanxung.cn

TS:   super.greet();
来源：http://cz.shxzukj.cn

Java: super.greet();
来源：http://pg.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yl.bookmarksfly.cn

Ruby: super
来源：http://ps.jianghongdianzi.cn

C#:   base.Greet();
来源：http://yf.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ui.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qz.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://le.chemitech.net.cn

JS:   static f() {}
来源：http://sh.szsharing.cn

TS:   static f(): void {}
来源：http://iu.jctech888.com.cn

Java: static void f() {}
来源：http://em.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hq.nszjky.cn

Ruby: def self.f; end
来源：http://ko.bookmarksfly.cn

C#:   public static void F() {}
来源：http://zm.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://vf.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://da.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://af.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://br.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://uu.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://la.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://jp.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uy.521024.cn

C#:   interface IShape { double Area(); }
来源：http://rz.szxytkj.cn

[G10] 访问控制
来源：http://ll.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://zs.newstarts.cn

PHP:  public / protected / private
来源：http://wx.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://lj.gzmigu.cn

TS:   public / protected / private
来源：http://qe.colortex.cn

Java: public / protected / private / 默认包级
来源：http://xl.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xk.huixiangedu.cn

Ruby: public / protected / private
来源：http://lx.nszjky.cn

C#:   public / protected / private / internal
来源：http://zf.szsharing.cn

[G11] getter / setter
来源：http://eh.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://da.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bd.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://li.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://dw.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://qt.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xh.nszjky.cn

Ruby: attr_accessor :name
来源：http://gb.huanxung.cn

C#:   public string Name { get; set; }
来源：http://gu.hahajie.cn

[G12] 对象转字符串
来源：http://lp.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://ih.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ye.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://rs.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://xd.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://cu.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pu.asd995.cn

Ruby: def to_s; @name; end
来源：http://wn.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://sv.huixiangedu.cn

[G13] 判断对象类型
来源：http://xp.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ot.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ru.yuntaijiaju.cn

JS:   u instanceof User
来源：http://cc.huanxung.cn

TS:   u instanceof User
来源：http://mm.yuntaijiaju.cn

Java: u instanceof User
来源：http://vz.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ff.nicolike.cn

Ruby: u.is_a?(User)
来源：http://nw.wgjwhj.cn

C#:   u is User
来源：http://ae.jctech888.com.cn

[G14] 数据类 / record
来源：http://gc.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nd.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://cg.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lw.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://sm.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://hn.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://fj.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://io.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://xr.bookmarksfly.cn

[G15] 枚举
来源：http://pk.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://at.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xd.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xt.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hs.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://vh.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tu.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://er.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kb.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://dk.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eq.colortex.cn

PHP:  get_object_vars($obj);
来源：http://wk.lnxyls.cn

JS:   Object.entries(obj)
来源：http://wp.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://wk.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xk.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cw.szxytkj.cn

Ruby: obj.instance_variables
来源：http://ta.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://kd.huixiangedu.cn

================================================================================
来源：http://td.521024.cn

H. 异常与错误处理
来源：http://jt.9csxet.cn

================================================================================
来源：http://cu.chemitech.net.cn

[H01] try / catch 基础
来源：http://es.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ab.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dc.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bt.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://br.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wg.521024.cn


<!-- 参考信息 -->