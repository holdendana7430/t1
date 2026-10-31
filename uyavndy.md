代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ly.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://op.shxzskj.cn

TS:   if (s === "") {}
来源：http://eo.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://xx.huanxung.cn

Go:   if s == "" {}
来源：http://hp.hnjuh.cn

Ruby: if s.empty?
来源：http://mf.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sr.nicolike.cn

[E21] 超长截断加省略号
来源：http://mg.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kw.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ly.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rb.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qa.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yp.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://fm.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xq.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cp.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://hk.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wi.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lu.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ex.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ac.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mr.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://ir.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lj.wgjwhj.cn

================================================================================
来源：http://ay.huanxung.cn

F. 文件与目录
来源：http://cp.szsharing.cn

================================================================================
来源：http://uz.panjiajie.cn

[F01] 读取整个文件
来源：http://yc.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sn.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://zd.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ra.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ax.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://di.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://la.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://ky.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://zf.gzmigu.cn

[F02] 逐行读取文件
来源：http://it.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wt.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ar.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ne.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ic.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pl.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ur.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xs.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kv.asd995.cn

[F03] 写入文件（覆盖）
来源：http://dk.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ml.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ri.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nn.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gv.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ba.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uc.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ld.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ki.gzmigu.cn

[F04] 追加写入文件
来源：http://by.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oo.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fm.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oq.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mj.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://at.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cv.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xf.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://te.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://dw.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pa.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://oz.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://xd.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://oy.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kn.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mt.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://oq.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://qu.asd995.cn

[F06] 删除文件
来源：http://tz.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://uh.colortex.cn

PHP:  unlink("a.txt");
来源：http://mx.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ih.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gc.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qd.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ax.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://cl.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://sm.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://iv.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oh.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sc.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nn.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ic.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ym.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zu.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ac.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ym.panjiajie.cn

[F08] 遍历目录
来源：http://qm.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pe.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xe.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://yq.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://de.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jc.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pl.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://pr.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://xd.panjiajie.cn

[F09] 获取文件大小
来源：http://bi.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://kj.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://id.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://oi.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://nn.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ov.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rf.asd995.cn

Ruby: File.size("a.txt")
来源：http://zn.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://qs.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://vb.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dm.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://in.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gk.nicolike.cn

TS:   path.extname("a.txt")
来源：http://vv.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://re.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ov.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tz.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vc.huanxung.cn

[F11] 复制与移动文件
来源：http://mc.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kz.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nt.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ux.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lj.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cx.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://re.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bl.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yd.jctech888.com.cn

[F12] CSV 读写
来源：http://rt.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lm.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sc.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wo.bjjhwx.cn

TS:   // 同上
来源：http://kc.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uj.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jn.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mh.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jt.lnxyls.cn

================================================================================
来源：http://it.huixiangedu.cn

G. 面向对象
来源：http://jo.panjiajie.cn

================================================================================
来源：http://rs.huixinmuqiang.cn

[G01] 定义类
来源：http://xk.szxytkj.cn

Py:   class User: pass
来源：http://zt.hnjuh.cn

PHP:  class User {}
来源：http://nl.nicolike.cn

JS:   class User {}
来源：http://hw.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://ew.jctech888.com.cn

Java: class User {}
来源：http://zg.9csxet.cn

Go:   type User struct { Name string }
来源：http://dn.9csxet.cn

Ruby: class User; end
来源：http://af.szsharing.cn

C#:   class User {}
来源：http://ku.wgjwhj.cn

[G02] 构造函数
来源：http://la.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://zj.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://eo.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://bs.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://ql.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://hp.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fk.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://uf.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://zd.shtwfgs.cn

[G03] 实例属性
来源：http://bl.bookmarksfly.cn

Py:   self.name = "x"
来源：http://mj.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://os.newstarts.cn

JS:   this.name = "x";
来源：http://cp.jctech888.com.cn

TS:   name: string = "x";
来源：http://pm.chemitech.net.cn

Java: private String name;
来源：http://hh.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pd.shxzukj.cn

Ruby: @name = "x"
来源：http://sr.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://fb.asd995.cn

[G04] 定义方法
来源：http://yd.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://jp.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pi.asd995.cn

JS:   greet() { return this.name; }
来源：http://il.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://km.jctech888.com.cn

Java: String greet() { return name; }
来源：http://vo.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cs.lnxyls.cn

Ruby: def greet; @name; end
来源：http://jj.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://jh.jianghongdianzi.cn

[G05] 继承
来源：http://bb.szxytkj.cn

Py:   class Admin(User): pass
来源：http://cd.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://bx.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://yn.lnxyls.cn

TS:   class Admin extends User {}
来源：http://li.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://wv.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ln.hnjuh.cn

Ruby: class Admin < User; end
来源：http://fg.newstarts.cn

C#:   class Admin : User {}
来源：http://jt.jianghongdianzi.cn

[G06] 重写方法
来源：http://zw.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://oq.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ng.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://hg.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://zq.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ju.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hc.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://dc.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://rz.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://eu.panjiajie.cn

Py:   super().greet()
来源：http://pt.huanxung.cn

PHP:  parent::greet();
来源：http://iq.bookmarksfly.cn

JS:   super.greet();
来源：http://qu.muxihuayi.cn

TS:   super.greet();
来源：http://vd.lnxyls.cn

Java: super.greet();
来源：http://hs.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ya.huixiangedu.cn

Ruby: super
来源：http://eq.jctech888.com.cn

C#:   base.Greet();
来源：http://lv.yuexingan06.cn

[G08] 静态方法与属性
来源：http://lj.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yh.jctech888.com.cn

PHP:  public static function f() {}
来源：http://pw.gzmigu.cn

JS:   static f() {}
来源：http://et.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://qc.hahajie.cn

Java: static void f() {}
来源：http://im.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://md.shxzskj.cn

Ruby: def self.f; end
来源：http://tm.szxytkj.cn

C#:   public static void F() {}
来源：http://sh.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://nb.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://kx.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zf.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xq.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://na.nicolike.cn

Java: interface Shape { double area(); }
来源：http://wc.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ge.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pl.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://aa.szsharing.cn

[G10] 访问控制
来源：http://en.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kq.shxzskj.cn

PHP:  public / protected / private
来源：http://ug.colortex.cn

JS:   #private 字段；其余公开
来源：http://uh.yuntaijiaju.cn

TS:   public / protected / private
来源：http://nz.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://cf.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ud.nszjky.cn

Ruby: public / protected / private
来源：http://md.huanxung.cn

C#:   public / protected / private / internal
来源：http://rl.shxzukj.cn

[G11] getter / setter
来源：http://rv.nicolike.cn

Py:   @property 与 @x.setter
来源：http://zs.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ja.colortex.cn

JS:   get name() { return this._name; }
来源：http://tx.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ek.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://cp.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://de.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://zl.huanxung.cn

C#:   public string Name { get; set; }
来源：http://qd.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://tp.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://jr.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kt.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://sz.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://un.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://ij.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ew.nszjky.cn

Ruby: def to_s; @name; end
来源：http://hn.521024.cn

C#:   public override string ToString() => Name;
来源：http://qv.haigaiapp.cn

[G13] 判断对象类型
来源：http://ix.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://tq.asd995.cn

PHP:  $u instanceof User
来源：http://dy.huanxung.cn

JS:   u instanceof User
来源：http://jw.wgjwhj.cn

TS:   u instanceof User
来源：http://gy.521024.cn

Java: u instanceof User
来源：http://mp.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cc.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://qb.szsharing.cn

C#:   u is User
来源：http://df.shxzskj.cn

[G14] 数据类 / record
来源：http://au.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rh.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jk.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ys.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://jq.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://ae.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://uw.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qa.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://cm.szxytkj.cn

[G15] 枚举
来源：http://rf.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ow.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hc.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rf.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ja.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://bu.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rk.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://xo.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wv.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://ww.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://je.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://bt.asd995.cn

JS:   Object.entries(obj)
来源：http://om.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://gx.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bo.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zk.nicolike.cn

Ruby: obj.instance_variables
来源：http://ne.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://wb.shtwfgs.cn

================================================================================
来源：http://dc.bookmarksfly.cn

H. 异常与错误处理
来源：http://px.jctech888.com.cn

================================================================================
来源：http://vx.huanxung.cn

[H01] try / catch 基础
来源：http://uc.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ew.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mm.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ua.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xo.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tj.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wz.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hg.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lw.szsharing.cn

[H02] finally / ensure 收尾
来源：http://bb.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yi.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lh.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ts.szxytkj.cn


<!-- 参考信息 -->