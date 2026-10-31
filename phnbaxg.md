代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://ig.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://yk.szxytkj.cn

Java: s.lines().toList()
来源：http://jg.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://wo.lnxyls.cn

Ruby: s.lines
来源：http://dx.lnxyls.cn

C#:   s.Split('\n')
来源：http://vf.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://lb.nicolike.cn

Py:   if not s:
来源：http://to.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xy.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ep.haigaiapp.cn

TS:   if (s === "") {}
来源：http://kr.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://qx.wgjwhj.cn

Go:   if s == "" {}
来源：http://bv.szxytkj.cn

Ruby: if s.empty?
来源：http://nm.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gb.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://dt.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ad.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nx.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yv.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hs.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cg.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://xt.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dd.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://le.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://bs.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://np.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ca.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zt.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jq.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rs.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ky.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://iv.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fb.hnjuh.cn

================================================================================
来源：http://mk.521024.cn

F. 文件与目录
来源：http://he.huanxung.cn

================================================================================
来源：http://og.szxytkj.cn

[F01] 读取整个文件
来源：http://lt.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nz.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://vo.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://av.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tw.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://is.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rr.huanxung.cn

Ruby: File.read("a.txt")
来源：http://ki.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://pe.gzmigu.cn

[F02] 逐行读取文件
来源：http://bl.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ay.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bz.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pb.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lc.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zs.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dw.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bb.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dv.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://es.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gr.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cn.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://px.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ax.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qk.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://di.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://yx.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bq.shxzskj.cn

[F04] 追加写入文件
来源：http://xa.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://db.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ef.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vw.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ro.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://es.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://su.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ij.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lf.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://av.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dx.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://ln.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://am.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://mr.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gh.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pa.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://cr.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://es.nszjky.cn

[F06] 删除文件
来源：http://wa.hahajie.cn

Py:   os.remove("a.txt")
来源：http://mr.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://gx.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gi.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zj.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pn.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://me.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://yr.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://aw.nicolike.cn

[F07] 创建目录（含多级）
来源：http://zs.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vk.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pr.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gp.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qo.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://af.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ir.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ib.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nd.haigaiapp.cn

[F08] 遍历目录
来源：http://pz.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://br.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qx.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://tj.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://ar.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qz.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sg.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://xq.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://dg.hahajie.cn

[F09] 获取文件大小
来源：http://vq.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://fh.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://dx.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://vb.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://ev.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sl.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hr.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://jz.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://hq.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://la.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vm.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://af.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ep.asd995.cn

TS:   path.extname("a.txt")
来源：http://eq.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lj.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tk.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zg.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://de.jctech888.com.cn

[F11] 复制与移动文件
来源：http://ek.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yr.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mv.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ug.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cd.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ci.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://es.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rb.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fw.szxytkj.cn

[F12] CSV 读写
来源：http://tt.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zb.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ry.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gz.szxytkj.cn

TS:   // 同上
来源：http://gw.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yh.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wj.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ih.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tt.lnxyls.cn

================================================================================
来源：http://js.yuntaijiaju.cn

G. 面向对象
来源：http://zo.newstarts.cn

================================================================================
来源：http://xc.jctech888.com.cn

[G01] 定义类
来源：http://mu.chemitech.net.cn

Py:   class User: pass
来源：http://jd.colortex.cn

PHP:  class User {}
来源：http://gz.panjiajie.cn

JS:   class User {}
来源：http://fn.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://gi.yuntaijiaju.cn

Java: class User {}
来源：http://bi.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://sp.wgjwhj.cn

Ruby: class User; end
来源：http://kd.hnjuh.cn

C#:   class User {}
来源：http://mj.521024.cn

[G02] 构造函数
来源：http://da.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://sr.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://av.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://js.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://ft.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://ed.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bn.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://lt.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://xg.shxzskj.cn

[G03] 实例属性
来源：http://ya.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://kz.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://ym.bookmarksfly.cn

JS:   this.name = "x";
来源：http://dj.nszjky.cn

TS:   name: string = "x";
来源：http://dz.yuexingan06.cn

Java: private String name;
来源：http://ai.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rk.bookmarksfly.cn

Ruby: @name = "x"
来源：http://de.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://ml.colortex.cn

[G04] 定义方法
来源：http://hv.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://hw.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mq.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://pf.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://jp.huixiangedu.cn

Java: String greet() { return name; }
来源：http://vx.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yx.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://aq.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://lq.huixinmuqiang.cn

[G05] 继承
来源：http://qg.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://bu.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://xm.hnjuh.cn

JS:   class Admin extends User {}
来源：http://qx.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://ke.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://xs.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fk.asd995.cn

Ruby: class Admin < User; end
来源：http://le.chemitech.net.cn

C#:   class Admin : User {}
来源：http://na.haigaiapp.cn

[G06] 重写方法
来源：http://uv.521024.cn

Py:   def greet(self): return "admin"
来源：http://xz.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pu.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://tj.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ga.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://bz.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xe.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://zj.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://hr.bjjhwx.cn

[G07] 调用父类方法
来源：http://ok.muxihuayi.cn

Py:   super().greet()
来源：http://ts.szxytkj.cn

PHP:  parent::greet();
来源：http://uh.nszjky.cn

JS:   super.greet();
来源：http://hm.jctech888.com.cn

TS:   super.greet();
来源：http://sj.muxihuayi.cn

Java: super.greet();
来源：http://cx.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zx.szxytkj.cn

Ruby: super
来源：http://qs.shtwfgs.cn

C#:   base.Greet();
来源：http://sr.huanxung.cn

[G08] 静态方法与属性
来源：http://gv.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wf.hahajie.cn

PHP:  public static function f() {}
来源：http://oo.szsharing.cn

JS:   static f() {}
来源：http://pk.szxytkj.cn

TS:   static f(): void {}
来源：http://kg.bookmarksfly.cn

Java: static void f() {}
来源：http://df.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yn.lnxyls.cn

Ruby: def self.f; end
来源：http://rs.newstarts.cn

C#:   public static void F() {}
来源：http://tg.521024.cn

[G09] 接口 / 抽象类
来源：http://xy.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://vn.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gz.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dh.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://ko.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://nw.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ip.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yz.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://kb.jianghongdianzi.cn

[G10] 访问控制
来源：http://vi.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://cf.szxytkj.cn

PHP:  public / protected / private
来源：http://bx.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://oo.nszjky.cn

TS:   public / protected / private
来源：http://nh.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://pz.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wr.haigaiapp.cn

Ruby: public / protected / private
来源：http://yk.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://lb.lnxyls.cn

[G11] getter / setter
来源：http://ol.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://rr.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sx.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ww.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://ig.huanxung.cn

Java: public String getName() { return name; }
来源：http://hu.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wj.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://zp.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://qm.newstarts.cn

[G12] 对象转字符串
来源：http://bi.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://rh.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xh.colortex.cn

JS:   toString() { return this.name; }
来源：http://be.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://pk.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://hm.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hx.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://dr.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://sb.nicolike.cn

[G13] 判断对象类型
来源：http://jq.521024.cn

Py:   isinstance(u, User)
来源：http://gk.huixiangedu.cn

PHP:  $u instanceof User
来源：http://zg.huixinmuqiang.cn

JS:   u instanceof User
来源：http://cp.jctech888.com.cn

TS:   u instanceof User
来源：http://bs.hnjuh.cn

Java: u instanceof User
来源：http://vt.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lp.521024.cn

Ruby: u.is_a?(User)
来源：http://gx.jianghongdianzi.cn

C#:   u is User
来源：http://qd.lnxyls.cn

[G14] 数据类 / record
来源：http://bn.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zi.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://xp.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xz.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://rv.nszjky.cn

Java: record User(String name, int age) {}
来源：http://jt.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://yi.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eg.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://kf.nszjky.cn

[G15] 枚举
来源：http://pc.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ao.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pm.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://id.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://na.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://wt.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tu.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://sq.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yn.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://fj.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ce.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://tj.asd995.cn

JS:   Object.entries(obj)
来源：http://rx.9csxet.cn

TS:   Object.entries(obj)
来源：http://ue.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iz.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hf.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://jx.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://of.gzmigu.cn

================================================================================
来源：http://ba.9csxet.cn

H. 异常与错误处理
来源：http://qf.hahajie.cn

================================================================================
来源：http://mk.panjiajie.cn

[H01] try / catch 基础
来源：http://dw.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pm.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rw.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oi.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tc.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qk.jianghongdianzi.cn


<!-- 参考信息 -->