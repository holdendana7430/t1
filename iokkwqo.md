代发 wailian999

Ruby: s.lines
来源：http://fl.hnjuh.cn

C#:   s.Split('\n')
来源：http://yx.asd995.cn

[E20] 判断字符串是否为空
来源：http://ep.yuexingan06.cn

Py:   if not s:
来源：http://ry.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gz.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mg.haigaiapp.cn

TS:   if (s === "") {}
来源：http://bw.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://wm.haigaiapp.cn

Go:   if s == "" {}
来源：http://kc.9csxet.cn

Ruby: if s.empty?
来源：http://rr.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rq.asd995.cn

[E21] 超长截断加省略号
来源：http://wn.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://js.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tu.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rg.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nj.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://de.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ta.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://do.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fr.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://ow.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hs.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hv.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dg.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qt.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://od.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xs.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://em.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://co.muxihuayi.cn

================================================================================
来源：http://bb.muxihuayi.cn

F. 文件与目录
来源：http://lw.huanxung.cn

================================================================================
来源：http://jf.gzmigu.cn

[F01] 读取整个文件
来源：http://bm.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ab.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://qv.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://co.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ts.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ce.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bw.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ii.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://to.muxihuayi.cn

[F02] 逐行读取文件
来源：http://xp.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cx.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vh.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ze.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://im.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://re.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kj.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gc.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://nr.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ef.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://up.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xq.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vj.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qf.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yp.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://kg.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xd.szxytkj.cn

[F04] 追加写入文件
来源：http://wj.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tc.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fk.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dn.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://le.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ky.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fn.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ks.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tq.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://jm.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://km.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ef.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://hx.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://jg.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ib.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://an.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://ck.colortex.cn

C#:   File.Exists("a.txt")
来源：http://id.hahajie.cn

[F06] 删除文件
来源：http://pa.colortex.cn

Py:   os.remove("a.txt")
来源：http://gw.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://tt.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://of.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lk.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jh.asd995.cn

Go:   os.Remove("a.txt")
来源：http://vi.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://ij.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://jf.nicolike.cn

[F07] 创建目录（含多级）
来源：http://ab.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rp.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sw.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://by.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oz.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wk.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bn.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wq.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qy.shxzukj.cn

[F08] 遍历目录
来源：http://fe.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hl.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wp.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://eh.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://kd.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yg.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yp.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://jm.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://yk.shxzukj.cn

[F09] 获取文件大小
来源：http://mz.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://vh.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ic.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ys.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://vt.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tl.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://el.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://nf.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://oo.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://xa.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yp.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ia.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gg.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://xx.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qx.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dy.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pc.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eb.nszjky.cn

[F11] 复制与移动文件
来源：http://li.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pl.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gr.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mg.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lt.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mt.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qv.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://we.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://td.bjjhwx.cn

[F12] CSV 读写
来源：http://vt.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uk.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yr.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yt.colortex.cn

TS:   // 同上
来源：http://nr.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yk.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lq.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uw.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ya.jctech888.com.cn

================================================================================
来源：http://jn.newstarts.cn

G. 面向对象
来源：http://mk.jctech888.com.cn

================================================================================
来源：http://lp.wgjwhj.cn

[G01] 定义类
来源：http://fv.jctech888.com.cn

Py:   class User: pass
来源：http://na.haigaiapp.cn

PHP:  class User {}
来源：http://xt.jianghongdianzi.cn

JS:   class User {}
来源：http://or.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://ph.hnjuh.cn

Java: class User {}
来源：http://jc.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://nu.szxytkj.cn

Ruby: class User; end
来源：http://qf.521024.cn

C#:   class User {}
来源：http://dh.nicolike.cn

[G02] 构造函数
来源：http://rp.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://rx.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://xa.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://al.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://vg.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://cs.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zw.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://sd.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ys.haigaiapp.cn

[G03] 实例属性
来源：http://yq.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://ya.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ni.wgjwhj.cn

JS:   this.name = "x";
来源：http://nn.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://bp.shtwfgs.cn

Java: private String name;
来源：http://vz.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rf.huixiangedu.cn

Ruby: @name = "x"
来源：http://aw.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://tp.chemitech.net.cn

[G04] 定义方法
来源：http://ea.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://et.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xa.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://uw.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://qq.huixiangedu.cn

Java: String greet() { return name; }
来源：http://mk.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gl.szsharing.cn

Ruby: def greet; @name; end
来源：http://nh.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://pm.szxytkj.cn

[G05] 继承
来源：http://fe.shxzukj.cn

Py:   class Admin(User): pass
来源：http://xt.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://mz.hahajie.cn

JS:   class Admin extends User {}
来源：http://zr.shxzskj.cn

TS:   class Admin extends User {}
来源：http://iy.shxzskj.cn

Java: class Admin extends User {}
来源：http://ws.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ov.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://ug.muxihuayi.cn

C#:   class Admin : User {}
来源：http://lf.hnjuh.cn

[G06] 重写方法
来源：http://lw.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://kt.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mr.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ii.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://sg.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://fl.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ns.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://rj.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://jk.wgjwhj.cn

[G07] 调用父类方法
来源：http://nu.bookmarksfly.cn

Py:   super().greet()
来源：http://le.newstarts.cn

PHP:  parent::greet();
来源：http://rx.asd995.cn

JS:   super.greet();
来源：http://gt.szxytkj.cn

TS:   super.greet();
来源：http://zs.gzmigu.cn

Java: super.greet();
来源：http://om.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ah.asd995.cn

Ruby: super
来源：http://qu.hnjuh.cn

C#:   base.Greet();
来源：http://cm.panjiajie.cn

[G08] 静态方法与属性
来源：http://os.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zf.haigaiapp.cn

PHP:  public static function f() {}
来源：http://sr.newstarts.cn

JS:   static f() {}
来源：http://dh.chemitech.net.cn

TS:   static f(): void {}
来源：http://ji.szxytkj.cn

Java: static void f() {}
来源：http://bw.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kd.colortex.cn

Ruby: def self.f; end
来源：http://mk.chemitech.net.cn

C#:   public static void F() {}
来源：http://vw.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://mk.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xh.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ho.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wq.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://gj.nszjky.cn

Java: interface Shape { double area(); }
来源：http://yo.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ly.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uv.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://vy.shtwfgs.cn

[G10] 访问控制
来源：http://cd.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://qp.jctech888.com.cn

PHP:  public / protected / private
来源：http://nn.newstarts.cn

JS:   #private 字段；其余公开
来源：http://ie.szxytkj.cn

TS:   public / protected / private
来源：http://nu.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://mb.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pi.colortex.cn

Ruby: public / protected / private
来源：http://bg.gzmigu.cn

C#:   public / protected / private / internal
来源：http://fy.huixiangedu.cn

[G11] getter / setter
来源：http://bh.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://pb.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sy.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://pe.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ce.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://as.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gf.szxytkj.cn

Ruby: attr_accessor :name
来源：http://ho.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://lp.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://tk.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://sw.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://py.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://qm.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://pr.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://rf.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://he.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://kt.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://nv.hnjuh.cn

[G13] 判断对象类型
来源：http://ya.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://ne.bjjhwx.cn

PHP:  $u instanceof User
来源：http://yw.huanxung.cn

JS:   u instanceof User
来源：http://kg.huixiangedu.cn

TS:   u instanceof User
来源：http://rj.szxytkj.cn

Java: u instanceof User
来源：http://tg.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vh.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://zr.szxytkj.cn

C#:   u is User
来源：http://re.hnjuh.cn

[G14] 数据类 / record
来源：http://pf.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ci.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://vh.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zn.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://wd.nicolike.cn

Java: record User(String name, int age) {}
来源：http://ks.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://bz.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ei.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://uk.bjjhwx.cn

[G15] 枚举
来源：http://fl.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gq.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zt.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eg.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kj.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://bz.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yf.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://zb.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cj.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://vy.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lj.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ic.9csxet.cn

JS:   Object.entries(obj)
来源：http://dm.521024.cn

TS:   Object.entries(obj)
来源：http://sk.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jd.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dm.521024.cn

Ruby: obj.instance_variables
来源：http://xh.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://bj.colortex.cn

================================================================================
来源：http://hc.nicolike.cn

H. 异常与错误处理
来源：http://ea.jctech888.com.cn

================================================================================
来源：http://rz.jctech888.com.cn

[H01] try / catch 基础
来源：http://ud.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ma.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lk.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://op.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ko.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dz.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hy.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hx.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://si.colortex.cn

[H02] finally / ensure 收尾
来源：http://fu.szxytkj.cn


<!-- 参考信息 -->