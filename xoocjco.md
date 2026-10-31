代发 wailian999

Ruby: s.lines
来源：http://ax.bjjhwx.cn

C#:   s.Split('\n')
来源：http://br.asd995.cn

[E20] 判断字符串是否为空
来源：http://nq.bjjhwx.cn

Py:   if not s:
来源：http://kh.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ku.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vk.szsharing.cn

TS:   if (s === "") {}
来源：http://rc.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://xk.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://jm.szxytkj.cn

Ruby: if s.empty?
来源：http://ur.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rw.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://zb.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wl.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xj.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rn.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qd.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://at.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://cd.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oi.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://si.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://yj.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fk.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vb.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ff.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ii.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vi.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uk.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://fd.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ww.szsharing.cn

================================================================================
来源：http://gc.nszjky.cn

F. 文件与目录
来源：http://mn.shxzukj.cn

================================================================================
来源：http://av.colortex.cn

[F01] 读取整个文件
来源：http://vo.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lb.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://lv.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vd.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pf.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oo.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cw.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ne.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://tf.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://hw.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gv.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sl.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ii.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pv.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gl.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dk.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vn.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gu.asd995.cn

[F03] 写入文件（覆盖）
来源：http://sc.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://py.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lr.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ts.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pn.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iy.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cc.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ve.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://la.muxihuayi.cn

[F04] 追加写入文件
来源：http://ku.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sl.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mc.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yb.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vx.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xz.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wq.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tu.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://co.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://db.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://cn.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://lb.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://za.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oe.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kn.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://xa.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://zt.nszjky.cn

[F06] 删除文件
来源：http://hc.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://xw.newstarts.cn

PHP:  unlink("a.txt");
来源：http://zx.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rj.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://da.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ji.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://pb.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://nw.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://kp.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://va.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tt.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zk.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gu.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zj.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mc.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bv.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wf.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gi.bjjhwx.cn

[F08] 遍历目录
来源：http://ig.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hf.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://er.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://hu.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://pi.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eh.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rb.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://bo.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://pl.szsharing.cn

[F09] 获取文件大小
来源：http://xd.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://xw.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://jz.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://mr.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://fx.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jl.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://as.newstarts.cn

Ruby: File.size("a.txt")
来源：http://cc.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://bh.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://jx.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rk.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ve.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gf.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://uq.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mf.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mg.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fd.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zf.haigaiapp.cn

[F11] 复制与移动文件
来源：http://cr.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://az.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://na.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qf.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xq.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zt.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vm.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ce.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cn.lnxyls.cn

[F12] CSV 读写
来源：http://eh.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bt.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qr.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ab.jctech888.com.cn

TS:   // 同上
来源：http://ft.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mv.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pk.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lm.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oa.bookmarksfly.cn

================================================================================
来源：http://tu.hahajie.cn

G. 面向对象
来源：http://oe.chemitech.net.cn

================================================================================
来源：http://ib.yuexingan06.cn

[G01] 定义类
来源：http://bo.wgjwhj.cn

Py:   class User: pass
来源：http://nz.szsharing.cn

PHP:  class User {}
来源：http://ro.newstarts.cn

JS:   class User {}
来源：http://xj.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://wy.szxytkj.cn

Java: class User {}
来源：http://gm.asd995.cn

Go:   type User struct { Name string }
来源：http://th.shxzskj.cn

Ruby: class User; end
来源：http://hc.lnxyls.cn

C#:   class User {}
来源：http://na.hnjuh.cn

[G02] 构造函数
来源：http://jy.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://zt.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://we.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://el.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://rw.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ix.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://po.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://mz.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://lh.nicolike.cn

[G03] 实例属性
来源：http://mz.hnjuh.cn

Py:   self.name = "x"
来源：http://mz.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://kh.jctech888.com.cn

JS:   this.name = "x";
来源：http://yl.hahajie.cn

TS:   name: string = "x";
来源：http://es.shxzukj.cn

Java: private String name;
来源：http://ca.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://or.huanxung.cn

Ruby: @name = "x"
来源：http://kp.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://rh.muxihuayi.cn

[G04] 定义方法
来源：http://yt.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://ra.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ny.9csxet.cn

JS:   greet() { return this.name; }
来源：http://um.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://rj.chemitech.net.cn

Java: String greet() { return name; }
来源：http://pe.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ur.gzmigu.cn

Ruby: def greet; @name; end
来源：http://tp.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://xy.shxzukj.cn

[G05] 继承
来源：http://xl.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://zp.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://in.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://qk.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://rn.asd995.cn

Java: class Admin extends User {}
来源：http://zn.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fh.panjiajie.cn

Ruby: class Admin < User; end
来源：http://gj.huixiangedu.cn

C#:   class Admin : User {}
来源：http://ci.nicolike.cn

[G06] 重写方法
来源：http://wc.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://mv.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://at.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://ap.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://hq.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://tn.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fh.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://ym.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://gc.521024.cn

[G07] 调用父类方法
来源：http://br.yuntaijiaju.cn

Py:   super().greet()
来源：http://ma.jctech888.com.cn

PHP:  parent::greet();
来源：http://vv.jianghongdianzi.cn

JS:   super.greet();
来源：http://sy.asd995.cn

TS:   super.greet();
来源：http://ar.asd995.cn

Java: super.greet();
来源：http://xu.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cd.yuntaijiaju.cn

Ruby: super
来源：http://wp.nszjky.cn

C#:   base.Greet();
来源：http://wt.yuexingan06.cn

[G08] 静态方法与属性
来源：http://vu.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lq.jctech888.com.cn

PHP:  public static function f() {}
来源：http://kg.shtwfgs.cn

JS:   static f() {}
来源：http://pz.newstarts.cn

TS:   static f(): void {}
来源：http://yo.9csxet.cn

Java: static void f() {}
来源：http://wk.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pa.huanxung.cn

Ruby: def self.f; end
来源：http://ub.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://yt.nicolike.cn

[G09] 接口 / 抽象类
来源：http://xk.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kj.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cs.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ao.521024.cn

TS:   interface Shape { area(): number; }
来源：http://lo.newstarts.cn

Java: interface Shape { double area(); }
来源：http://jr.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://sp.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ra.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://sz.gzmigu.cn

[G10] 访问控制
来源：http://mm.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://cy.9csxet.cn

PHP:  public / protected / private
来源：http://zg.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://oh.shtwfgs.cn

TS:   public / protected / private
来源：http://cz.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://fv.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hp.lnxyls.cn

Ruby: public / protected / private
来源：http://ue.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://nk.shxzukj.cn

[G11] getter / setter
来源：http://ef.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://qi.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nv.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://ag.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://jz.shxzukj.cn

Java: public String getName() { return name; }
来源：http://rg.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fs.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://el.colortex.cn

C#:   public string Name { get; set; }
来源：http://we.newstarts.cn

[G12] 对象转字符串
来源：http://xf.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://bt.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oo.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://kz.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://js.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://oj.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://op.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://me.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://pj.szxytkj.cn

[G13] 判断对象类型
来源：http://fh.newstarts.cn

Py:   isinstance(u, User)
来源：http://dq.bjjhwx.cn

PHP:  $u instanceof User
来源：http://go.hnjuh.cn

JS:   u instanceof User
来源：http://et.521024.cn

TS:   u instanceof User
来源：http://em.nicolike.cn

Java: u instanceof User
来源：http://pn.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ic.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ei.szxytkj.cn

C#:   u is User
来源：http://nl.haigaiapp.cn

[G14] 数据类 / record
来源：http://zd.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ot.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://cy.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ou.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://yf.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://vg.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ls.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://un.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://pg.bookmarksfly.cn

[G15] 枚举
来源：http://ji.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xv.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://el.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pu.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eh.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://on.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zl.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://uw.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cq.521024.cn

[G16] 对象转数组 / 字典
来源：http://aa.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cs.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://ga.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://oe.shxzukj.cn

TS:   Object.entries(obj)
来源：http://ue.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pk.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qw.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://yp.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://ex.huanxung.cn

================================================================================
来源：http://zi.muxihuayi.cn

H. 异常与错误处理
来源：http://lg.yuexingan06.cn

================================================================================
来源：http://gs.bjjhwx.cn

[H01] try / catch 基础
来源：http://ax.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dd.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xf.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jo.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nb.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dp.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://da.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://td.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hq.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://gq.hahajie.cn


<!-- 参考信息 -->