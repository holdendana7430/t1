代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pf.asd995.cn

[E19] 多行文本按行拆分
来源：http://np.shtwfgs.cn

Py:   s.splitlines()
来源：http://nq.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gb.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://bi.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://uq.szxytkj.cn

Java: s.lines().toList()
来源：http://hn.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://cn.haigaiapp.cn

Ruby: s.lines
来源：http://by.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://he.asd995.cn

[E20] 判断字符串是否为空
来源：http://ah.muxihuayi.cn

Py:   if not s:
来源：http://zv.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kq.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qc.szxytkj.cn

TS:   if (s === "") {}
来源：http://jv.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://yn.wgjwhj.cn

Go:   if s == "" {}
来源：http://aa.colortex.cn

Ruby: if s.empty?
来源：http://wu.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kt.9csxet.cn

[E21] 超长截断加省略号
来源：http://xj.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cx.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ur.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mx.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cj.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ej.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://yt.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jq.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iq.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://cj.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eu.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zx.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pn.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nf.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ej.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://vm.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ip.lnxyls.cn

================================================================================
来源：http://zf.shxzukj.cn

F. 文件与目录
来源：http://xn.huixinmuqiang.cn

================================================================================
来源：http://vb.9csxet.cn

[F01] 读取整个文件
来源：http://rm.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eu.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://pd.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yi.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xq.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cn.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gz.nszjky.cn

Ruby: File.read("a.txt")
来源：http://rc.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://ok.haigaiapp.cn

[F02] 逐行读取文件
来源：http://df.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ht.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qn.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ex.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qt.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ew.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aq.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://aj.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dh.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nf.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gh.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xo.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yj.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rs.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://oe.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://er.hnjuh.cn

[F04] 追加写入文件
来源：http://tu.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hq.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hn.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tm.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gy.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qc.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jq.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kt.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://lz.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qd.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://js.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://uv.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://ua.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hg.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bm.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://yc.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://se.chemitech.net.cn

[F06] 删除文件
来源：http://gc.huanxung.cn

Py:   os.remove("a.txt")
来源：http://pc.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://cj.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cn.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mg.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hu.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://lv.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://hp.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://bh.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ad.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wc.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wg.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kb.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sk.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nv.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pc.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zc.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wm.muxihuayi.cn

[F08] 遍历目录
来源：http://zi.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sh.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rg.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://se.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://pg.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nv.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ub.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://kj.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://yb.chemitech.net.cn

[F09] 获取文件大小
来源：http://co.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://pj.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://gc.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://ad.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://vk.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cf.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nz.asd995.cn

Ruby: File.size("a.txt")
来源：http://ii.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://mb.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://sa.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hr.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rj.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ur.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://wm.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xa.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hi.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wl.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xh.521024.cn

[F11] 复制与移动文件
来源：http://oy.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tr.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iq.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fm.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lb.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ge.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hv.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ld.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qo.szxytkj.cn

[F12] CSV 读写
来源：http://oz.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hy.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xg.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ur.yuexingan06.cn

TS:   // 同上
来源：http://hb.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dr.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zl.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fh.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://no.huixinmuqiang.cn

================================================================================
来源：http://gc.szxytkj.cn

G. 面向对象
来源：http://zy.yuntaijiaju.cn

================================================================================
来源：http://kb.huixiangedu.cn

[G01] 定义类
来源：http://lq.szxytkj.cn

Py:   class User: pass
来源：http://fn.hnjuh.cn

PHP:  class User {}
来源：http://xl.9csxet.cn

JS:   class User {}
来源：http://yb.521024.cn

TS:   class User { name: string = ""; }
来源：http://uh.huanxung.cn

Java: class User {}
来源：http://wg.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://cw.jianghongdianzi.cn

Ruby: class User; end
来源：http://mh.szsharing.cn

C#:   class User {}
来源：http://kz.521024.cn

[G02] 构造函数
来源：http://dp.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ls.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://cf.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ku.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://cv.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://py.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lq.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://ke.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ip.jianghongdianzi.cn

[G03] 实例属性
来源：http://om.wgjwhj.cn

Py:   self.name = "x"
来源：http://tl.9csxet.cn

PHP:  public string $name = "x";
来源：http://xc.nszjky.cn

JS:   this.name = "x";
来源：http://nl.haigaiapp.cn

TS:   name: string = "x";
来源：http://me.nicolike.cn

Java: private String name;
来源：http://tp.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tn.muxihuayi.cn

Ruby: @name = "x"
来源：http://ky.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://hk.chemitech.net.cn

[G04] 定义方法
来源：http://pd.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://nx.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nw.newstarts.cn

JS:   greet() { return this.name; }
来源：http://bc.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://by.bjjhwx.cn

Java: String greet() { return name; }
来源：http://fp.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nk.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://iy.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://fd.jianghongdianzi.cn

[G05] 继承
来源：http://ic.asd995.cn

Py:   class Admin(User): pass
来源：http://oi.huanxung.cn

PHP:  class Admin extends User {}
来源：http://hh.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://hj.huanxung.cn

TS:   class Admin extends User {}
来源：http://kq.jctech888.com.cn

Java: class Admin extends User {}
来源：http://qq.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nk.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ir.bjjhwx.cn

C#:   class Admin : User {}
来源：http://tl.jianghongdianzi.cn

[G06] 重写方法
来源：http://mh.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://dx.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wf.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://nj.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://ha.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://gk.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oo.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://po.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://mx.panjiajie.cn

[G07] 调用父类方法
来源：http://nq.asd995.cn

Py:   super().greet()
来源：http://kh.haigaiapp.cn

PHP:  parent::greet();
来源：http://bt.jctech888.com.cn

JS:   super.greet();
来源：http://by.521024.cn

TS:   super.greet();
来源：http://yx.chemitech.net.cn

Java: super.greet();
来源：http://kz.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fg.newstarts.cn

Ruby: super
来源：http://ej.521024.cn

C#:   base.Greet();
来源：http://db.hnjuh.cn

[G08] 静态方法与属性
来源：http://ok.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ke.9csxet.cn

PHP:  public static function f() {}
来源：http://zr.szxytkj.cn

JS:   static f() {}
来源：http://pm.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://yz.panjiajie.cn

Java: static void f() {}
来源：http://mu.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zk.chemitech.net.cn

Ruby: def self.f; end
来源：http://lj.szsharing.cn

C#:   public static void F() {}
来源：http://sq.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://qz.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://zz.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nk.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://um.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://sq.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://ah.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://tj.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sg.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://hp.shxzukj.cn

[G10] 访问控制
来源：http://si.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://sx.bookmarksfly.cn

PHP:  public / protected / private
来源：http://rm.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://br.jianghongdianzi.cn

TS:   public / protected / private
来源：http://dc.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://us.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ci.asd995.cn

Ruby: public / protected / private
来源：http://ow.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://oy.yuntaijiaju.cn

[G11] getter / setter
来源：http://rt.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://id.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://er.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ib.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://bn.nszjky.cn

Java: public String getName() { return name; }
来源：http://ez.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vk.huanxung.cn

Ruby: attr_accessor :name
来源：http://mi.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://sa.bookmarksfly.cn

[G12] 对象转字符串
来源：http://xo.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://gp.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cy.newstarts.cn

JS:   toString() { return this.name; }
来源：http://rp.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://ob.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://rv.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bf.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://ef.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://vk.colortex.cn

[G13] 判断对象类型
来源：http://wf.szxytkj.cn

Py:   isinstance(u, User)
来源：http://sf.szsharing.cn

PHP:  $u instanceof User
来源：http://kq.szxytkj.cn

JS:   u instanceof User
来源：http://sd.chemitech.net.cn

TS:   u instanceof User
来源：http://tt.muxihuayi.cn

Java: u instanceof User
来源：http://xf.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qy.huanxung.cn

Ruby: u.is_a?(User)
来源：http://eh.jianghongdianzi.cn

C#:   u is User
来源：http://kh.huanxung.cn

[G14] 数据类 / record
来源：http://pa.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mn.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://sv.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://md.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://ky.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://hm.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://qg.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ao.521024.cn

C#:   record User(string Name, int Age);
来源：http://fv.shtwfgs.cn

[G15] 枚举
来源：http://gz.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ym.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://at.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bd.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eq.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://ak.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zc.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://rm.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yd.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://fb.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eu.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://aj.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://dy.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://mc.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ft.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ol.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://kq.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://yl.newstarts.cn

================================================================================
来源：http://ww.hahajie.cn

H. 异常与错误处理
来源：http://ia.shtwfgs.cn

================================================================================
来源：http://ol.huanxung.cn

[H01] try / catch 基础
来源：http://sf.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sk.gzmigu.cn


<!-- 参考信息 -->