代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://lj.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://qw.lnxyls.cn

Java: s.lines().toList()
来源：http://ca.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://lu.chemitech.net.cn

Ruby: s.lines
来源：http://jb.yuexingan06.cn

C#:   s.Split('\n')
来源：http://so.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://nr.muxihuayi.cn

Py:   if not s:
来源：http://hn.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ou.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ga.lnxyls.cn

TS:   if (s === "") {}
来源：http://mi.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://dr.bjjhwx.cn

Go:   if s == "" {}
来源：http://jh.hnjuh.cn

Ruby: if s.empty?
来源：http://ce.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://df.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://dx.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pc.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yw.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kv.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://db.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nc.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zi.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bz.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hp.9csxet.cn

[E22] 字节长度与字符长度
来源：http://em.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://du.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://er.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bp.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bm.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rw.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://uo.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xj.asd995.cn

================================================================================
来源：http://ja.bjjhwx.cn

F. 文件与目录
来源：http://cz.chemitech.net.cn

================================================================================
来源：http://qa.bjjhwx.cn

[F01] 读取整个文件
来源：http://yb.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qj.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://gu.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ki.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://az.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rb.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dl.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://yo.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://lb.wgjwhj.cn

[F02] 逐行读取文件
来源：http://hw.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kc.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zp.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ag.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ia.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yq.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ah.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ty.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ng.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://qq.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hm.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zp.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ya.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vh.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xm.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qx.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://hz.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vq.wgjwhj.cn

[F04] 追加写入文件
来源：http://gb.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jq.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jv.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yb.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cx.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ut.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cb.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ud.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://od.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://nr.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yj.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://tv.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://sd.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://im.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zt.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cj.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://zv.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://xu.panjiajie.cn

[F06] 删除文件
来源：http://fr.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://zc.hahajie.cn

PHP:  unlink("a.txt");
来源：http://yn.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oj.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xg.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mb.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://fw.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://jw.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://bf.szsharing.cn

[F07] 创建目录（含多级）
来源：http://es.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qe.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ye.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yu.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zk.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cw.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hr.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://td.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pv.chemitech.net.cn

[F08] 遍历目录
来源：http://sy.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kw.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ho.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://km.521024.cn

TS:   fs.readdirSync("dir")
来源：http://rf.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vl.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ol.nicolike.cn

Ruby: Dir.children("dir")
来源：http://ak.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://xt.chemitech.net.cn

[F09] 获取文件大小
来源：http://zh.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://mn.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://qf.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://th.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://pl.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dk.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://be.9csxet.cn

Ruby: File.size("a.txt")
来源：http://rz.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://vo.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://ak.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xw.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ku.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pe.nicolike.cn

TS:   path.extname("a.txt")
来源：http://uo.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://co.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sf.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ac.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qj.newstarts.cn

[F11] 复制与移动文件
来源：http://il.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cf.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yk.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yc.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nx.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://af.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fe.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ae.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bk.yuntaijiaju.cn

[F12] CSV 读写
来源：http://af.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ua.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qk.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cr.shtwfgs.cn

TS:   // 同上
来源：http://rz.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vg.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ty.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pe.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lh.bjjhwx.cn

================================================================================
来源：http://nk.szxytkj.cn

G. 面向对象
来源：http://yj.huixinmuqiang.cn

================================================================================
来源：http://es.jctech888.com.cn

[G01] 定义类
来源：http://rf.yuexingan06.cn

Py:   class User: pass
来源：http://uw.muxihuayi.cn

PHP:  class User {}
来源：http://vs.bookmarksfly.cn

JS:   class User {}
来源：http://na.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://dd.szxytkj.cn

Java: class User {}
来源：http://dt.huanxung.cn

Go:   type User struct { Name string }
来源：http://ia.huixiangedu.cn

Ruby: class User; end
来源：http://jg.bjjhwx.cn

C#:   class User {}
来源：http://tu.hahajie.cn

[G02] 构造函数
来源：http://wk.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ux.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://la.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://nj.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://pl.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://dl.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bp.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://tl.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://al.521024.cn

[G03] 实例属性
来源：http://pi.shxzskj.cn

Py:   self.name = "x"
来源：http://un.shxzskj.cn

PHP:  public string $name = "x";
来源：http://vv.hahajie.cn

JS:   this.name = "x";
来源：http://ow.szxytkj.cn

TS:   name: string = "x";
来源：http://jh.521024.cn

Java: private String name;
来源：http://bw.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xc.huanxung.cn

Ruby: @name = "x"
来源：http://jv.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://li.bookmarksfly.cn

[G04] 定义方法
来源：http://db.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ef.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zx.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://vh.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://pb.newstarts.cn

Java: String greet() { return name; }
来源：http://iu.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lr.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://tt.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://uj.wgjwhj.cn

[G05] 继承
来源：http://hl.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://fv.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://iz.panjiajie.cn

JS:   class Admin extends User {}
来源：http://gq.gzmigu.cn

TS:   class Admin extends User {}
来源：http://la.szsharing.cn

Java: class Admin extends User {}
来源：http://lw.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mn.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://zb.hahajie.cn

C#:   class Admin : User {}
来源：http://nj.bookmarksfly.cn

[G06] 重写方法
来源：http://bv.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://ec.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lm.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://na.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://fx.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://br.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wi.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://je.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://aa.lnxyls.cn

[G07] 调用父类方法
来源：http://te.huanxung.cn

Py:   super().greet()
来源：http://vk.gzmigu.cn

PHP:  parent::greet();
来源：http://ru.huixinmuqiang.cn

JS:   super.greet();
来源：http://iw.asd995.cn

TS:   super.greet();
来源：http://dj.hahajie.cn

Java: super.greet();
来源：http://wr.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rm.colortex.cn

Ruby: super
来源：http://rh.szxytkj.cn

C#:   base.Greet();
来源：http://sk.huixiangedu.cn

[G08] 静态方法与属性
来源：http://ik.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oc.9csxet.cn

PHP:  public static function f() {}
来源：http://hs.chemitech.net.cn

JS:   static f() {}
来源：http://fd.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://bi.panjiajie.cn

Java: static void f() {}
来源：http://hx.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fr.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://gx.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://bl.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://rg.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://uc.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hv.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://af.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://zi.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ip.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ql.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://px.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://kh.szsharing.cn

[G10] 访问控制
来源：http://ww.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://kn.hahajie.cn

PHP:  public / protected / private
来源：http://xn.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://fb.hnjuh.cn

TS:   public / protected / private
来源：http://qp.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://ie.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ho.9csxet.cn

Ruby: public / protected / private
来源：http://bz.asd995.cn

C#:   public / protected / private / internal
来源：http://by.chemitech.net.cn

[G11] getter / setter
来源：http://gh.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://wl.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ca.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://am.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://rj.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://xg.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ms.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://fa.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://gr.chemitech.net.cn

[G12] 对象转字符串
来源：http://ff.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://qo.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ms.hahajie.cn

JS:   toString() { return this.name; }
来源：http://kj.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://pj.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://rh.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cg.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://dk.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://pq.szxytkj.cn

[G13] 判断对象类型
来源：http://sa.hnjuh.cn

Py:   isinstance(u, User)
来源：http://gv.gzmigu.cn

PHP:  $u instanceof User
来源：http://vl.szxytkj.cn

JS:   u instanceof User
来源：http://tc.9csxet.cn

TS:   u instanceof User
来源：http://rs.colortex.cn

Java: u instanceof User
来源：http://lt.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gl.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ii.panjiajie.cn

C#:   u is User
来源：http://kf.nicolike.cn

[G14] 数据类 / record
来源：http://he.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yf.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ok.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vq.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://er.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://fs.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://bu.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eb.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://do.panjiajie.cn

[G15] 枚举
来源：http://is.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pq.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gi.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fg.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dy.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://wy.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zf.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://zl.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ju.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://tj.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sq.521024.cn

PHP:  get_object_vars($obj);
来源：http://uz.hahajie.cn

JS:   Object.entries(obj)
来源：http://qz.gzmigu.cn

TS:   Object.entries(obj)
来源：http://kn.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qi.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yk.hahajie.cn

Ruby: obj.instance_variables
来源：http://vw.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://pr.jianghongdianzi.cn

================================================================================
来源：http://ps.hnjuh.cn

H. 异常与错误处理
来源：http://dk.jctech888.com.cn

================================================================================
来源：http://bu.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://qe.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kg.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qn.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nq.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mp.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kb.szxytkj.cn


<!-- 参考信息 -->