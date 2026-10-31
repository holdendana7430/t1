代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://va.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yj.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dp.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ql.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ue.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://qf.nszjky.cn

Py:   s.splitlines()
来源：http://by.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dr.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://hy.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://fo.bookmarksfly.cn

Java: s.lines().toList()
来源：http://wk.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://aa.wgjwhj.cn

Ruby: s.lines
来源：http://rj.chemitech.net.cn

C#:   s.Split('\n')
来源：http://es.colortex.cn

[E20] 判断字符串是否为空
来源：http://aa.hahajie.cn

Py:   if not s:
来源：http://ht.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lf.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dc.haigaiapp.cn

TS:   if (s === "") {}
来源：http://cy.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://ln.huixiangedu.cn

Go:   if s == "" {}
来源：http://ed.huanxung.cn

Ruby: if s.empty?
来源：http://ai.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nt.shxzukj.cn

[E21] 超长截断加省略号
来源：http://zt.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xm.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kk.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gq.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cs.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pb.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://zj.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vx.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fc.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://mz.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gs.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ba.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xs.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vh.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ar.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pd.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://qg.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://li.huixiangedu.cn

================================================================================
来源：http://ur.jianghongdianzi.cn

F. 文件与目录
来源：http://ab.521024.cn

================================================================================
来源：http://cz.521024.cn

[F01] 读取整个文件
来源：http://xc.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gk.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://hz.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jh.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://up.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vq.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wt.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://ob.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://fl.shxzukj.cn

[F02] 逐行读取文件
来源：http://np.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fx.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hv.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tb.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vz.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aw.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kf.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dj.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xs.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://lu.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lx.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tb.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pn.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lj.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cx.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qu.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://sf.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://na.huixiangedu.cn

[F04] 追加写入文件
来源：http://jp.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iu.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yb.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ei.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ys.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gr.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ji.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eq.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://rs.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wp.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://dh.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://uj.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://pb.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ig.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sd.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://vv.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://mm.hahajie.cn

[F06] 删除文件
来源：http://uq.szsharing.cn

Py:   os.remove("a.txt")
来源：http://fr.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://zs.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://os.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iv.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jc.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://db.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://lk.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://cn.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://on.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cp.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://to.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vw.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nw.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nc.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fw.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://od.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bl.muxihuayi.cn

[F08] 遍历目录
来源：http://vp.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kc.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://on.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://gd.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://mw.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bt.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ym.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://lo.hahajie.cn

[F09] 获取文件大小
来源：http://ck.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://kb.nicolike.cn

PHP:  filesize("a.txt");
来源：http://dl.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://nr.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://lq.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ga.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cf.hahajie.cn

Ruby: File.size("a.txt")
来源：http://bz.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://dx.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://ow.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hr.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sk.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pm.asd995.cn

TS:   path.extname("a.txt")
来源：http://zp.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vy.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://br.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zr.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sz.521024.cn

[F11] 复制与移动文件
来源：http://ys.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bo.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://js.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bw.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ql.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cd.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://od.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://co.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cz.huixiangedu.cn

[F12] CSV 读写
来源：http://yf.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rj.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fn.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xk.gzmigu.cn

TS:   // 同上
来源：http://yg.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xn.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bo.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ye.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fc.521024.cn

================================================================================
来源：http://sd.haigaiapp.cn

G. 面向对象
来源：http://yh.gzmigu.cn

================================================================================
来源：http://sg.yuntaijiaju.cn

[G01] 定义类
来源：http://tu.yuntaijiaju.cn

Py:   class User: pass
来源：http://db.colortex.cn

PHP:  class User {}
来源：http://sg.newstarts.cn

JS:   class User {}
来源：http://dw.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://fg.newstarts.cn

Java: class User {}
来源：http://sa.colortex.cn

Go:   type User struct { Name string }
来源：http://vm.lnxyls.cn

Ruby: class User; end
来源：http://lf.shtwfgs.cn

C#:   class User {}
来源：http://pr.huixiangedu.cn

[G02] 构造函数
来源：http://xl.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://bo.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://kh.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://xg.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://ms.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://gf.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hp.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://cg.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://uj.nszjky.cn

[G03] 实例属性
来源：http://ov.gzmigu.cn

Py:   self.name = "x"
来源：http://yy.colortex.cn

PHP:  public string $name = "x";
来源：http://do.hahajie.cn

JS:   this.name = "x";
来源：http://ky.521024.cn

TS:   name: string = "x";
来源：http://as.panjiajie.cn

Java: private String name;
来源：http://ac.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pn.szsharing.cn

Ruby: @name = "x"
来源：http://fd.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://dc.nicolike.cn

[G04] 定义方法
来源：http://rb.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://om.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://si.9csxet.cn

JS:   greet() { return this.name; }
来源：http://ie.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://nk.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://nu.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hn.521024.cn

Ruby: def greet; @name; end
来源：http://jd.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://hr.bookmarksfly.cn

[G05] 继承
来源：http://we.lnxyls.cn

Py:   class Admin(User): pass
来源：http://nj.szsharing.cn

PHP:  class Admin extends User {}
来源：http://tu.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://ya.asd995.cn

TS:   class Admin extends User {}
来源：http://ur.szsharing.cn

Java: class Admin extends User {}
来源：http://uu.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://co.huanxung.cn

Ruby: class Admin < User; end
来源：http://kw.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://vp.szxytkj.cn

[G06] 重写方法
来源：http://hn.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://hj.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cn.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ju.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://tw.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://zb.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kq.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://aa.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ar.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://oo.bjjhwx.cn

Py:   super().greet()
来源：http://dm.jctech888.com.cn

PHP:  parent::greet();
来源：http://bn.asd995.cn

JS:   super.greet();
来源：http://ti.newstarts.cn

TS:   super.greet();
来源：http://am.nszjky.cn

Java: super.greet();
来源：http://ed.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ja.shxzskj.cn

Ruby: super
来源：http://uz.szsharing.cn

C#:   base.Greet();
来源：http://bi.jctech888.com.cn

[G08] 静态方法与属性
来源：http://vq.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ig.nicolike.cn

PHP:  public static function f() {}
来源：http://qu.yuexingan06.cn

JS:   static f() {}
来源：http://pr.hahajie.cn

TS:   static f(): void {}
来源：http://nv.asd995.cn

Java: static void f() {}
来源：http://qr.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hi.nszjky.cn

Ruby: def self.f; end
来源：http://fj.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://nt.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://ca.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://qh.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ip.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sb.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://wc.521024.cn

Java: interface Shape { double area(); }
来源：http://ik.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://am.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ou.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://sr.jctech888.com.cn

[G10] 访问控制
来源：http://xv.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://fs.hahajie.cn

PHP:  public / protected / private
来源：http://wf.huanxung.cn

JS:   #private 字段；其余公开
来源：http://at.jctech888.com.cn

TS:   public / protected / private
来源：http://je.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://pb.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gw.hahajie.cn

Ruby: public / protected / private
来源：http://hy.colortex.cn

C#:   public / protected / private / internal
来源：http://ly.nicolike.cn

[G11] getter / setter
来源：http://gj.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://vv.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iv.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://vg.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://ge.521024.cn

Java: public String getName() { return name; }
来源：http://rg.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kh.szsharing.cn

Ruby: attr_accessor :name
来源：http://sq.521024.cn

C#:   public string Name { get; set; }
来源：http://je.hnjuh.cn

[G12] 对象转字符串
来源：http://kk.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://mh.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iw.nszjky.cn

JS:   toString() { return this.name; }
来源：http://je.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://en.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://jd.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qn.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://im.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ob.asd995.cn

[G13] 判断对象类型
来源：http://ao.gzmigu.cn

Py:   isinstance(u, User)
来源：http://ue.lnxyls.cn

PHP:  $u instanceof User
来源：http://kt.haigaiapp.cn

JS:   u instanceof User
来源：http://ih.521024.cn

TS:   u instanceof User
来源：http://mf.nszjky.cn

Java: u instanceof User
来源：http://ix.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qz.newstarts.cn

Ruby: u.is_a?(User)
来源：http://sk.huixinmuqiang.cn

C#:   u is User
来源：http://bs.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://ir.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://en.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ll.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sy.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://dc.huanxung.cn

Java: record User(String name, int age) {}
来源：http://ru.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://tu.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xl.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://ik.gzmigu.cn

[G15] 枚举
来源：http://dc.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mu.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ae.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://to.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gg.521024.cn

Java: enum Color { RED, GREEN }
来源：http://cx.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://an.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://jn.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gd.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://iw.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ue.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://fd.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://ef.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://gs.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://on.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://db.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://fw.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://yn.gzmigu.cn

================================================================================
来源：http://tm.nicolike.cn


<!-- 参考信息 -->