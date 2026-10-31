代发 wailian999

Ruby: s.lines
来源：http://zt.panjiajie.cn

C#:   s.Split('\n')
来源：http://an.asd995.cn

[E20] 判断字符串是否为空
来源：http://mj.gzmigu.cn

Py:   if not s:
来源：http://xs.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://di.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hc.nicolike.cn

TS:   if (s === "") {}
来源：http://ma.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://ad.bookmarksfly.cn

Go:   if s == "" {}
来源：http://pl.jctech888.com.cn

Ruby: if s.empty?
来源：http://io.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eg.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://fr.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ii.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vj.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hi.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kr.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://qy.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sm.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mi.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://oj.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uy.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cw.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ow.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ft.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dp.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oj.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://gc.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://om.shtwfgs.cn

================================================================================
来源：http://nx.colortex.cn

F. 文件与目录
来源：http://zx.shxzukj.cn

================================================================================
来源：http://vw.bookmarksfly.cn

[F01] 读取整个文件
来源：http://jc.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://or.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ba.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cd.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zi.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tf.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xa.colortex.cn

Ruby: File.read("a.txt")
来源：http://bi.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://su.hahajie.cn

[F02] 逐行读取文件
来源：http://aq.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kn.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jy.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nc.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ev.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gm.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lk.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ti.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uh.521024.cn

[F03] 写入文件（覆盖）
来源：http://tm.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kn.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ja.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ld.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ri.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jf.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://ho.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tk.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://ok.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oy.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gl.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bo.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ap.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dk.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://du.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ef.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hy.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://xd.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jb.asd995.cn

PHP:  file_exists("a.txt");
来源：http://oq.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://zs.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://fj.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gr.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ot.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://tu.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://xn.colortex.cn

[F06] 删除文件
来源：http://db.hahajie.cn

Py:   os.remove("a.txt")
来源：http://kw.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://dp.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fd.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sm.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://by.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://mt.asd995.cn

Ruby: File.delete("a.txt")
来源：http://hg.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://xo.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://od.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yg.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vx.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qd.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mu.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sk.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fj.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gn.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jc.521024.cn

[F08] 遍历目录
来源：http://pr.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ti.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ue.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://cy.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://yg.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yq.szsharing.cn

Ruby: Dir.children("dir")
来源：http://tw.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://fk.521024.cn

[F09] 获取文件大小
来源：http://rd.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://ox.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://pa.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://au.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ja.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fn.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wu.newstarts.cn

Ruby: File.size("a.txt")
来源：http://lx.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://zc.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://ir.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ns.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sb.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rv.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://rq.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dc.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lw.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qb.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wv.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://ia.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xo.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ip.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zj.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://an.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gs.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://og.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vg.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://px.yuexingan06.cn

[F12] CSV 读写
来源：http://sl.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kd.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vm.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cj.newstarts.cn

TS:   // 同上
来源：http://in.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cj.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fc.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bw.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hl.9csxet.cn

================================================================================
来源：http://tn.bjjhwx.cn

G. 面向对象
来源：http://ld.bookmarksfly.cn

================================================================================
来源：http://fs.lnxyls.cn

[G01] 定义类
来源：http://xp.hahajie.cn

Py:   class User: pass
来源：http://yu.nszjky.cn

PHP:  class User {}
来源：http://ni.wgjwhj.cn

JS:   class User {}
来源：http://aa.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://ni.yuexingan06.cn

Java: class User {}
来源：http://jy.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://yx.huixiangedu.cn

Ruby: class User; end
来源：http://ys.hnjuh.cn

C#:   class User {}
来源：http://xr.huixinmuqiang.cn

[G02] 构造函数
来源：http://xl.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://im.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://yy.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ak.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://vq.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://ge.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ez.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://lb.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ak.jianghongdianzi.cn

[G03] 实例属性
来源：http://ei.9csxet.cn

Py:   self.name = "x"
来源：http://qu.szsharing.cn

PHP:  public string $name = "x";
来源：http://qv.panjiajie.cn

JS:   this.name = "x";
来源：http://nb.newstarts.cn

TS:   name: string = "x";
来源：http://jb.nszjky.cn

Java: private String name;
来源：http://dp.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://va.lnxyls.cn

Ruby: @name = "x"
来源：http://sj.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://bu.muxihuayi.cn

[G04] 定义方法
来源：http://xv.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://am.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ie.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://zo.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ts.muxihuayi.cn

Java: String greet() { return name; }
来源：http://wy.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nu.521024.cn

Ruby: def greet; @name; end
来源：http://mu.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://tw.shtwfgs.cn

[G05] 继承
来源：http://gm.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://tn.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://tl.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://xo.szxytkj.cn

TS:   class Admin extends User {}
来源：http://th.haigaiapp.cn

Java: class Admin extends User {}
来源：http://tw.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ch.panjiajie.cn

Ruby: class Admin < User; end
来源：http://gt.colortex.cn

C#:   class Admin : User {}
来源：http://ik.haigaiapp.cn

[G06] 重写方法
来源：http://mt.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://hr.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://im.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://nm.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://ps.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://ms.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pe.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://sx.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://un.haigaiapp.cn

[G07] 调用父类方法
来源：http://ry.asd995.cn

Py:   super().greet()
来源：http://hd.shxzukj.cn

PHP:  parent::greet();
来源：http://qc.haigaiapp.cn

JS:   super.greet();
来源：http://rv.shtwfgs.cn

TS:   super.greet();
来源：http://mi.nicolike.cn

Java: super.greet();
来源：http://cs.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jc.9csxet.cn

Ruby: super
来源：http://yi.hnjuh.cn

C#:   base.Greet();
来源：http://co.yuexingan06.cn

[G08] 静态方法与属性
来源：http://ji.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tn.nicolike.cn

PHP:  public static function f() {}
来源：http://dm.9csxet.cn

JS:   static f() {}
来源：http://lz.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://fe.hahajie.cn

Java: static void f() {}
来源：http://wy.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ui.wgjwhj.cn

Ruby: def self.f; end
来源：http://qa.nicolike.cn

C#:   public static void F() {}
来源：http://ph.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://bp.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://kr.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kg.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ye.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://vd.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://lk.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://it.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://im.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://zy.szxytkj.cn

[G10] 访问控制
来源：http://af.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://ad.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://uu.huanxung.cn

JS:   #private 字段；其余公开
来源：http://ka.newstarts.cn

TS:   public / protected / private
来源：http://fx.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://ds.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tm.szsharing.cn

Ruby: public / protected / private
来源：http://fh.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://ss.newstarts.cn

[G11] getter / setter
来源：http://ms.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://al.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ba.asd995.cn

JS:   get name() { return this._name; }
来源：http://wp.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://iz.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://fq.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kg.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://og.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://rh.panjiajie.cn

[G12] 对象转字符串
来源：http://hq.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://ru.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gm.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://ui.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://df.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://uq.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mh.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://ki.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://jg.chemitech.net.cn

[G13] 判断对象类型
来源：http://ez.nszjky.cn

Py:   isinstance(u, User)
来源：http://jy.jctech888.com.cn

PHP:  $u instanceof User
来源：http://yv.huanxung.cn

JS:   u instanceof User
来源：http://vf.asd995.cn

TS:   u instanceof User
来源：http://bw.gzmigu.cn

Java: u instanceof User
来源：http://wj.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pe.szsharing.cn

Ruby: u.is_a?(User)
来源：http://dk.521024.cn

C#:   u is User
来源：http://zx.muxihuayi.cn

[G14] 数据类 / record
来源：http://ch.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nv.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://nk.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yr.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://en.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://jr.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://qx.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gc.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://ws.shxzukj.cn

[G15] 枚举
来源：http://ha.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ma.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ym.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tt.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vx.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://xw.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jq.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://oe.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pt.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://bd.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xk.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://rk.szxytkj.cn

JS:   Object.entries(obj)
来源：http://dv.newstarts.cn

TS:   Object.entries(obj)
来源：http://ws.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ii.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zd.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://zf.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ex.jctech888.com.cn

================================================================================
来源：http://kl.colortex.cn

H. 异常与错误处理
来源：http://rg.hahajie.cn

================================================================================
来源：http://yt.asd995.cn

[H01] try / catch 基础
来源：http://xp.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rh.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vv.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aa.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fl.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nk.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://db.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vb.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://al.521024.cn

[H02] finally / ensure 收尾
来源：http://my.nicolike.cn


<!-- 参考信息 -->