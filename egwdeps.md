代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://om.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://hz.bjjhwx.cn

Py:   s.splitlines()
来源：http://qr.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://so.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://wy.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://qs.jctech888.com.cn

Java: s.lines().toList()
来源：http://ue.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://ev.hnjuh.cn

Ruby: s.lines
来源：http://pr.shxzskj.cn

C#:   s.Split('\n')
来源：http://rc.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://zm.asd995.cn

Py:   if not s:
来源：http://ty.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wf.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pj.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://hf.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://tj.hnjuh.cn

Go:   if s == "" {}
来源：http://uc.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://qj.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zk.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://po.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xd.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xm.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uv.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ww.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qv.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://sd.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eb.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://ha.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jj.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ub.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ac.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ub.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kz.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ug.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://my.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jz.shxzskj.cn

================================================================================
来源：http://rq.newstarts.cn

F. 文件与目录
来源：http://gy.nszjky.cn

================================================================================
来源：http://dj.huanxung.cn

[F01] 读取整个文件
来源：http://fy.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xk.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://va.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ia.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dy.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pp.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ew.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://vl.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://az.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://wa.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://en.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ji.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://io.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lg.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ij.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ov.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ep.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qc.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://tl.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lu.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dv.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ve.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uy.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sl.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oi.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://fj.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bk.shxzukj.cn

[F04] 追加写入文件
来源：http://he.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fw.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ck.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jz.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ip.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ai.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ka.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sx.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://nb.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xo.colortex.cn

PHP:  file_exists("a.txt");
来源：http://el.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://ni.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://cs.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jd.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bc.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://an.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://gu.huixiangedu.cn

[F06] 删除文件
来源：http://kc.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://ew.hahajie.cn

PHP:  unlink("a.txt");
来源：http://zg.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kd.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qq.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hd.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://to.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://cl.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://xv.asd995.cn

[F07] 创建目录（含多级）
来源：http://og.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iv.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mf.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cg.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bw.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://in.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dc.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kc.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bg.shxzskj.cn

[F08] 遍历目录
来源：http://ga.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dg.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ma.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://jn.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://wr.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yd.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vd.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://bu.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://io.panjiajie.cn

[F09] 获取文件大小
来源：http://gm.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://mf.asd995.cn

PHP:  filesize("a.txt");
来源：http://dt.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ft.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://cs.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gc.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xc.newstarts.cn

Ruby: File.size("a.txt")
来源：http://zv.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://dt.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://dc.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zg.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aw.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fw.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://sh.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nx.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://el.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dc.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pd.muxihuayi.cn

[F11] 复制与移动文件
来源：http://qh.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nn.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://av.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gm.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dk.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hq.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aq.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bs.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nz.colortex.cn

[F12] CSV 读写
来源：http://jb.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mk.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cb.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rt.nszjky.cn

TS:   // 同上
来源：http://kc.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ht.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xl.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xb.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zx.colortex.cn

================================================================================
来源：http://ua.9csxet.cn

G. 面向对象
来源：http://hl.521024.cn

================================================================================
来源：http://vj.521024.cn

[G01] 定义类
来源：http://ey.bjjhwx.cn

Py:   class User: pass
来源：http://cd.shxzskj.cn

PHP:  class User {}
来源：http://iv.nszjky.cn

JS:   class User {}
来源：http://iv.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ks.nicolike.cn

Java: class User {}
来源：http://vh.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://ik.521024.cn

Ruby: class User; end
来源：http://ic.shtwfgs.cn

C#:   class User {}
来源：http://ml.jianghongdianzi.cn

[G02] 构造函数
来源：http://dt.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://hg.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://iq.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://zv.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://yz.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://zs.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cg.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://he.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://gs.jianghongdianzi.cn

[G03] 实例属性
来源：http://bt.hnjuh.cn

Py:   self.name = "x"
来源：http://lt.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://kb.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://vw.shxzskj.cn

TS:   name: string = "x";
来源：http://hq.bjjhwx.cn

Java: private String name;
来源：http://jf.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zj.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://pr.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://jw.colortex.cn

[G04] 定义方法
来源：http://ci.huanxung.cn

Py:   def greet(self): return self.name
来源：http://sw.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lc.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://jx.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://fb.jctech888.com.cn

Java: String greet() { return name; }
来源：http://vb.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zx.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://dy.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://bb.szxytkj.cn

[G05] 继承
来源：http://pk.nicolike.cn

Py:   class Admin(User): pass
来源：http://xn.9csxet.cn

PHP:  class Admin extends User {}
来源：http://xv.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://ug.huanxung.cn

TS:   class Admin extends User {}
来源：http://vm.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://bf.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://or.nicolike.cn

Ruby: class Admin < User; end
来源：http://ng.huixiangedu.cn

C#:   class Admin : User {}
来源：http://pl.bjjhwx.cn

[G06] 重写方法
来源：http://cp.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://fu.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://db.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://qk.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://sy.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://da.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sr.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ay.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://pd.lnxyls.cn

[G07] 调用父类方法
来源：http://ki.haigaiapp.cn

Py:   super().greet()
来源：http://eg.wgjwhj.cn

PHP:  parent::greet();
来源：http://op.haigaiapp.cn

JS:   super.greet();
来源：http://cs.haigaiapp.cn

TS:   super.greet();
来源：http://bj.yuntaijiaju.cn

Java: super.greet();
来源：http://nw.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qq.yuntaijiaju.cn

Ruby: super
来源：http://du.nicolike.cn

C#:   base.Greet();
来源：http://jq.huixiangedu.cn

[G08] 静态方法与属性
来源：http://su.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ws.nszjky.cn

PHP:  public static function f() {}
来源：http://yz.huixiangedu.cn

JS:   static f() {}
来源：http://cc.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://qa.shxzskj.cn

Java: static void f() {}
来源：http://nd.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kj.panjiajie.cn

Ruby: def self.f; end
来源：http://hj.chemitech.net.cn

C#:   public static void F() {}
来源：http://vj.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://nn.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ia.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ei.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tp.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://vc.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://kq.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://jg.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sv.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://xh.hahajie.cn

[G10] 访问控制
来源：http://vz.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ua.chemitech.net.cn

PHP:  public / protected / private
来源：http://vj.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://yi.haigaiapp.cn

TS:   public / protected / private
来源：http://dl.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://fw.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jj.jctech888.com.cn

Ruby: public / protected / private
来源：http://qf.shxzskj.cn

C#:   public / protected / private / internal
来源：http://gk.shxzskj.cn

[G11] getter / setter
来源：http://nk.szsharing.cn

Py:   @property 与 @x.setter
来源：http://bp.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uc.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://xq.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://rk.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://sk.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ff.colortex.cn

Ruby: attr_accessor :name
来源：http://tk.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://yk.hnjuh.cn

[G12] 对象转字符串
来源：http://jx.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://sc.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qf.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://oj.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://fa.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://fc.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ec.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://sx.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://vu.shtwfgs.cn

[G13] 判断对象类型
来源：http://rw.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://fs.bjjhwx.cn

PHP:  $u instanceof User
来源：http://dd.huixinmuqiang.cn

JS:   u instanceof User
来源：http://ke.huixiangedu.cn

TS:   u instanceof User
来源：http://lg.newstarts.cn

Java: u instanceof User
来源：http://jn.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ww.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://rn.jctech888.com.cn

C#:   u is User
来源：http://ka.521024.cn

[G14] 数据类 / record
来源：http://gl.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mh.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://pa.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://me.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ex.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://lp.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://gw.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sn.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://pw.szsharing.cn

[G15] 枚举
来源：http://gu.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://an.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rf.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qf.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://od.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ep.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://om.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://on.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ff.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://gp.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fk.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://qi.huanxung.cn

JS:   Object.entries(obj)
来源：http://om.huanxung.cn

TS:   Object.entries(obj)
来源：http://np.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cw.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ye.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://jn.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://lg.hnjuh.cn

================================================================================
来源：http://tn.bjjhwx.cn

H. 异常与错误处理
来源：http://mi.szsharing.cn

================================================================================
来源：http://qc.huanxung.cn

[H01] try / catch 基础
来源：http://hf.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://au.chemitech.net.cn


<!-- 参考信息 -->