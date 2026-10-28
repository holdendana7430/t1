代发 wailian999

[F01] 读取整个文件
来源：http://hz.yanxiufei.cn/gtfxzyhxgv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtshkcjwsv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.svipenyu.cn/gtwferhyxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.smart0.xyz/gtirbbefvp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtputlblst.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtnexbptub.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtqezyhyrd.html

Ruby: File.read("a.txt")
来源：http://hz.cheryme.top/gtqefqrbtn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtrepkxcei.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtnnlwvqkj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.snrcjt.cn/gttfkogukj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtvfptfxwo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtpbhctjxe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gtunjqntow.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtmkzcjkxc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtevvnielq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gotoacloud.top/gtbqqdrthf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtckyqupwl.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtvwwnmkfy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.andypj.xyz/gtypiqryru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtglrkxqlz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtkdihzjcy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtxviroyqg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ivvv.top/gtsejljrqe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gttoxvllyj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuetiantiany.cn/gtqsuhrvpo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gtjgktdsoq.html

[F04] 追加写入文件
来源：http://hz.zhengqikj.top/gtaswebrio.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtsegyoppl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtgylbqejl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtlcmramor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtzdqrwxfa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenlongwang.top/gtlhdcilnb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gtzcsjfycs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtmnroteza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtkpcehcys.html

[F05] 判断文件或目录是否存在
来源：http://hz.dashuyun.cn/gtaamujdfz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gttauegakk.html

PHP:  file_exists("a.txt");
来源：http://hz.snrcjt.cn/gtmdducwrp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtbxtqhgzn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtmtpeawxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtimndcheo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xziqi.cn/gtbgpevzpd.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtscyntrgh.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gthgugoygm.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtvovqefqo.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtnmqjjpju.html

PHP:  unlink("a.txt");
来源：http://hz.yongpay.top/gtamsjqifj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gtvxjweiqe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtmcgfmpvh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtuqfktcgu.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtvfqoanje.html

Ruby: File.delete("a.txt")
来源：http://hz.aibaodan.cn/gtnztccfkr.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gtsrpqymnc.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtexlvpaeq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtndbpwplu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj202588.top/gtfmurjcbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtykjzjekh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtnrrmwcqh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtxgexctzc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xinyue.icu/gtesirchiw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangdashe.top/gttrgrqurv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtuikapaln.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtmcoqlevt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtaggvvssq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtytxtgbtl.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtgxdguqvl.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtpwjcrlch.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtxehfvzul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtttprayrx.html

Ruby: Dir.children("dir")
来源：http://hz.yvedp.cn/gtslaevvpu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtlqkudbpr.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtlihwhgnh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtudtvnman.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtxvzgobha.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gthscbxfkr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtmfnbemcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtuuhtpxqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtvjhkkbrq.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigfzy.top/gtuwsjvhuc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtkcfswzeb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtmufjwajo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtcvwssqjr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtfvssgzbg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtaribzwde.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gttcrrgfjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtelwrvolv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtamawauid.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtlhcvprhz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtqwwipvrj.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtzucrlvtd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtgnvwlpxz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtpqtnlfpl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtrogdrgmv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtcqqcbtfu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigfzy.top/gthvvrwsia.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ppjwa.cn/gtaddjobac.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtblqntttw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gteyjbnklj.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtjttpkpfb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtoikymsvs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtcetwwndu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shuidangran.top/gtoilaairr.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gthvgjzuel.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ivvv.top/gthvqrawsi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtfgwcaign.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tanke756.top/gtozbkqqpi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtwblqdlmp.html

================================================================================
来源：http://hz.jinqigufen.top/gtdmebtpbj.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtbuxudlzb.html

================================================================================
来源：http://hz.havefunace.top/gtyngkubjh.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gtevgnnguc.html

Py:   class User: pass
来源：http://hz.yuxming.cn/gtfztkxjah.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gtakplqrkt.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtigdghklf.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtnuwxlhyw.html

Java: class User {}
来源：http://hz.andypj.xyz/gtotnablxm.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtxqattuug.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtpfxnhpya.html

C#:   class User {}
来源：http://hz.yj20258.top/gtnkpbhnuf.html

[G02] 构造函数
来源：http://hz.cucudq.cn/gtefbnmjyc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtxievgbca.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtfzpjeuir.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtpsqpaovo.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangkeji.top/gtukpdxlce.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtnhhvfxwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtestrritz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtdkjgifoi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtobcduphi.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtwfeckrdq.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtiuicavmt.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtnpyqfhta.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtedtypzoa.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtzzopljfw.html

Java: private String name;
来源：http://hz.jianghu66.top/gtpmmuwgga.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gthvgbxgso.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtauxqsitd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gturjhzmwa.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtuluigfcj.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtdsyzngww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtslbptfeu.html

JS:   greet() { return this.name; }
来源：http://hz.9152youxi.cn/gttloskqlt.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtokeqosxh.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gtzfggjjtc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtvnuyrqrg.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtxmigrqtz.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gttseexgko.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtemufgkua.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtqauzqciz.html

PHP:  class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtycheoxkj.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gthzdnvsdl.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtisorsxxa.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtvoztybhk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtgflpejli.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gttgyjuqst.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gtgfuaxoyn.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtoxujlhmj.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtelzwfbir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtktsgwjqj.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtfrzafltw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtnzjobekb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtqjlvgolw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gtblxzzqrm.html

Ruby: def greet; "admin"; end
来源：http://hz.0kj1m.cn/gtxbwypmqo.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtsrbnzdnz.html

[G07] 调用父类方法
来源：http://hz.redwolf501.top/gtwqblhmsi.html

Py:   super().greet()
来源：http://hz.pycfn.com/gtrvnynjsr.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gteckwageg.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtlktacddz.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtgxczkkee.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtdprvnxwl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hysaishi.cn/gtbiqzoysv.html

Ruby: super
来源：http://hz.andypj.xyz/gtxyyvskjk.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtrpxbjplh.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtzyggbqoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtbheyqqeb.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtdgpuhqaa.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtzhykhjpg.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtgrfztvma.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtokyuuxdo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtcltapwmd.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtplfaolhu.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtqftuhltt.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtmdnfxzjd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtdugjycum.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.quarkkingdee.top/gtvedqhdrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtzetfyffm.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtpavjltso.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtkcrnbtvs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtfkzeadnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtssvptnsd.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtzvoldavc.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtixbukksz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtsknfunjc.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtyyebufqs.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtlkomvlng.html

TS:   public / protected / private
来源：http://hz.zhiwuduotai.top/gtzymixzvg.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtkkpwzvre.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtvopszovt.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtetrkfwtz.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtngymtvdu.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gthtcefjkz.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gtzgmelwzw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtkxrgrxyp.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtvqzonmgb.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gtongynmiq.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtakcxezlu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtmywfajvb.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtyticycyi.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtszfmwiyt.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtmxfnvxga.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtxzvdfmpf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtyndnhhtw.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtwtoziucn.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtiryiyxga.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtswoaxsjo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtdmesxtun.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtqvtowycm.html

C#:   public override string ToString() => Name;
来源：http://hz.wangdashe.top/gtswkaosub.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gthdkyymtt.html

Py:   isinstance(u, User)
来源：http://hz.zhongyouzk.top/gtmeqwwtlo.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtpgktfmrz.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gteqilqnqq.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtpigqnvkd.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtciqtwmgu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jlsjyb.cn/gtwfjyscuf.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtgqtefyub.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtztejidzo.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtkykekrfh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtllsqlpei.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtoztbxkgq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtasqnadbe.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtormdiqcm.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gtzxhwmxee.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtngiqkdbx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ywan-chungtsiang.top/gteubouxil.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtobkrcyfv.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtmqeddflq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gttdsrvrtd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtnglspozn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtystzfbbd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gthwmsgmdp.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gttztoupdp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtmcczyobd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtftpxklmt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtodnawale.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgufenzy.top/gtihtglkjb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtsjrjhdeh.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtvejqkuiu.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtaqskoowo.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtwfjvquxb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gtwnazhwvg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtskjmoxzx.html

Ruby: obj.instance_variables
来源：http://hz.ydjk.org.cn/gtboxmzvfj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gthhadycad.html

================================================================================
来源：http://hz.fzhhl.top/gtziblivre.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtvxjopqjx.html

================================================================================
来源：http://hz.yonumen.top/gtrkbswoeo.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtcbxstjmm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gtjmzhpsoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtlfsverhn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtjjavswhz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtubtkavue.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtyzhozhlo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtgfvoglkg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtlhbqtlya.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtjylcfffq.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtbuxekwaf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtgllbrvhe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtzxjxmkwx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtjqqibrpe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtkzricgkc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtpqijhkem.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtvplyjajg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guowangkeji.top/gtyikjbjxg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtysurhkka.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtjfusjnew.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtuekdpcqf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gthokwiewo.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtecitihws.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtndadrrbj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtzyaiibds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yangfankeji.com/gtqzttjjjm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtmjjrrlsk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtvpwntywc.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtznzwbevv.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtammuotjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtdezahprc.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtxsvrdxia.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtxgtgdxzl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtgbtpsttb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtrmosbvax.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtydlnfpoi.html

C#:   class MyException : Exception {}
来源：http://hz.tianlin.xyz/gtydcafnzk.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtsanzzpij.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtbciwycbd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtgjcoushp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtjzapnedy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtjetxglqq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtvezcgesp.html


<!-- 参考信息 -->