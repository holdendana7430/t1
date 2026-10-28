代发 wailian999

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtnewvfsne.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gtmfktjeqk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtvxzdqfoc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258.top/gtwddrwnjg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtwqcujtrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtfeztcayn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtqaizujze.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gtopboelpg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtrgqqjsjo.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtwzovnabj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtsfqgccvi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dashuyun.cn/gtanbruxci.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtxvtopiex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtsaovghoj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtbhjcpilc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtdvagqnmz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtdglbasny.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gttfjlgxvx.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtdydzvxhr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtnhiedwvt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtuxtckhyu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtbunopgfm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtywugulce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtjoqpxvqu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtnmkihdye.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtjudmcvhb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtuaskrzal.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtfyrvrzhq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtixmalqln.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtatgvrsok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtsukaxaxb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtqaehrmyu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yongpay.top/gtzwcolckw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtoyrikbpq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtobwszqtr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gtvcyqefnq.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtzvgcrkpg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtowdfonby.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtgjzeiwur.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtfpjzmqqc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.bjfxy.top/gtgwapeuvv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtbvthwpah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jlsjyb.cn/gtftkrwmxt.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtwbdnynxm.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtxoarkrck.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtqxnonfex.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtpnpntwju.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtzeuphpmb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtysbjlebn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtscgvdxlc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtwvfewbyb.html

Go:   os.Remove("a.txt")
来源：http://hz.yanxiufei.cn/gtewaopxbf.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gttnzvoqib.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtmadgalvc.html

[F07] 创建目录（含多级）
来源：http://hz.jqgfzy.top/gtbfffbyjr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gthqbqkupj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtrdrxuany.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtdarpbklt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtzqnbleyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtxuhlkjdl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenjidiqi.icu/gtiyfkklsc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtckinzfro.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gteryrrzyo.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtebajecsy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hongshengwenyu.top/gtrbovcqoj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtvrheinbl.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtmsclkglq.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtbsjmtupf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtvuqwrceu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtoxgwdnoy.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtbjvhiqhv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtivzlqtbh.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtlxmeqzyz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuanzx.com/gtddrqyjzy.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtwsyatqck.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtofezagge.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtpxhbmdoa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtonnkclyt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtltqfwcbf.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtlxyoajib.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.vqdsnc.cn/gtduiafsnz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gtbpxadtly.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gthittywrk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtibhlfojf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtrfkvnxfx.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtauayxnwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jianghu66.top/gtzumrkpnc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dianchejie.cn/gtayekddbq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtynispbae.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtbvirpeua.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtchrjwzcj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtaaymztvk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtpzcmhrbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtnsskooez.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtmgjyxyzp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.quarkkingdee.top/gtgdrfdtcc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtvregdiwz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtiuwhjlct.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtoukbcgrk.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtiofesxwx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtwhwslgiy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gogol.net.cn/gtbgppbdlf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yongpay.top/gtfrlabyza.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtjctycxks.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtzntegvgg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.iojbl.cn/gtglihoumv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gtnjtthuun.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtblrwwybk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcrablcll.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtihxjtsve.html

================================================================================
来源：http://hz.c1oappe.top/gthktjiuuh.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtncvnwlrh.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtcuthzufh.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gtafrirpxv.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtiyzwumoz.html

TS:   class User { name: string = ""; }
来源：http://hz.chenlongwang.top/gtyoaullej.html

Java: class User {}
来源：http://hz.haohaochexian.top/gtrlzmjlzi.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtgzilvzbz.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtnuvmasgj.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtapujwpgg.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtyyypstnt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gtcohujifj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtotxmdsdk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtvyhchclq.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtgcrkvrvp.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtsktfxssc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtplqavmcb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtdszyzleg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sxryk.cn/gtdogbiehe.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtxkgbslod.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtbmmawege.html

PHP:  public string $name = "x";
来源：http://hz.ywan-chungtsiang.top/gtzwjsewru.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtcmmqtqxv.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtzcopcniy.html

Java: private String name;
来源：http://hz.yj20258888.top/gtphohvbtf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtoftxurio.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtughqdmgs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtcqjmunas.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtjwbhbclj.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtaoohguvk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtahzpvoft.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtsppncguq.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtttihyhrq.html

Java: String greet() { return name; }
来源：http://hz.hfpthk.cn/gtfilbmjej.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.havefunace.top/gtmxrykwpk.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtfaacxdfk.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtpztkidmt.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtnlpuqhaf.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtrbdahwvo.html

PHP:  class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtpxuvujou.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtvlinfovb.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtvpvhzhvm.html

Java: class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtjpevaezg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtfymsojyb.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtssfaqblb.html

C#:   class Admin : User {}
来源：http://hz.jqgufenzy.top/gtxyoucxml.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtjmwbfwsr.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtzxikasbb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtfkjktkrd.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtqfrjghgk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtavbdlrhf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtpiuljkem.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtaccjvhxu.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtbrpairfv.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtildossby.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gtjlzxrhep.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtnvuuzeok.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtqjbkcsdu.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtennickpk.html

TS:   super.greet();
来源：http://hz.hammf.cn/gthciqylls.html

Java: super.greet();
来源：http://hz.cucudq.cn/gtbtkscwpq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtgnsansta.html

Ruby: super
来源：http://hz.meibo888.top/gtdopvkzem.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtsvshcvyg.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtzgwodrwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtfsgevyyj.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtvcqdaxjc.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtykkclayz.html

TS:   static f(): void {}
来源：http://hz.dianchejie.cn/gtcrfukwmg.html

Java: static void f() {}
来源：http://hz.ydzc1.top/gtdynhtscj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cqqwz.cn/gtbhrjbgop.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtwpbcqpkb.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtcreiqspu.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtqgtqksnv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtzueewuex.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtdnldrruz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtcexsussd.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gthbuuwhxb.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtuenzqtxd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gtxesbsaln.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtiaccrpsz.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtasqsgips.html

[G10] 访问控制
来源：http://hz.yueranfly.top/gtdxbfdezn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtbvatduwa.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtdrqfdqsl.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtjhbywgow.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gttfugeeea.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtunljxsjo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gttatnjrdr.html

Ruby: public / protected / private
来源：http://hz.gogol.net.cn/gtozrwhhue.html

C#:   public / protected / private / internal
来源：http://hz.yongpay.top/gtwdickihj.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtkuxnxrto.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtyrglgmix.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtaqruoqly.html

JS:   get name() { return this._name; }
来源：http://hz.zycfv.cn/gtsgkatpdz.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtcvhjnyst.html

Java: public String getName() { return name; }
来源：http://hz.jianghu66.top/gtyiabkkuz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtkdhcjzea.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtiwsmfgla.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtlufdwlan.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtstoiqxhy.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtsbmiethg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtejidvdrh.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtaglksscl.html

TS:   toString(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtrgkkvssn.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gtxuqvruvx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gthvlyqene.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtksgbiueg.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtosqbvdcr.html

[G13] 判断对象类型
来源：http://hz.iojbl.cn/gtalouyboz.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtiikrpdmo.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gthncnjolm.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtxsfbmyhg.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtnxfbajzc.html

Java: u instanceof User
来源：http://hz.pycfn.com/gtgbtnyuho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gttbaxtwuy.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtizwbiuql.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gtsvlxlomn.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtplbzpodq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtmyswhpic.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gthgfgqein.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gthlgyrnsq.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gtwpwbtcju.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtlgejsyii.html

Go:   type User struct { Name string; Age int }
来源：http://hz.andypj.xyz/gtolfrvnrb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.vqdsnc.cn/gtwtnzbspn.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtytjnqizh.html

[G15] 枚举
来源：http://hz.yj20258.top/gtdvvyydgi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtfiibrsxe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtqlhbtjim.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gttttopyoj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtmngesnjk.html

Java: enum Color { RED, GREEN }
来源：http://hz.cdnleiting.top/gtayvbrmms.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sysykeji.top/gteoyspfbt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gtekpmcpfr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtbdqqxfnl.html

[G16] 对象转数组 / 字典
来源：http://hz.hfpthk.cn/gtedxwrmsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gthltwcgkk.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtqwzlnahh.html

JS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtssmcbddp.html

TS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtinqpaeuo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtpowhhphw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtvkgsddkq.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtbpuclhyp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtskkuqdyc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtewotxkvm.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtucfyedht.html

================================================================================
来源：http://hz.tanke756.top/gtwtmohmpq.html

[H01] try / catch 基础
来源：http://hz.hammf.cn/gtpkrcqjqk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtykpuicmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtgjjndxoh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtspskbapk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fengsongda.top/gttqkorvfm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtyuoqcpvg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtpzfcpwog.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtshkaalhw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ppjwa.cn/gtixfmsprd.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtuhboecid.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gtrtrryedi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtqqymguyv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtwieupymr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtjtcubhiz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gttlzvmepm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtsqzcmujp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtkpdmeyuq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtslmmztvu.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtkrafmmvr.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtklvixqwu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtegrqhnrd.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtbfloidfi.html

TS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtbyaqljlx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtgbirouoj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cdnleiting.top/gtnrpcdvam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtmrxsarvw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtadnhtuyv.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gtxkpuoarx.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtkgutxaog.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtzhntosvy.html

JS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtjzloqnpz.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtjjkjqipa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtywhpimmr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gtjdrmwpex.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtnsajlyrv.html

C#:   class MyException : Exception {}
来源：http://hz.yuanzhike.top/gtboxjyyzc.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtpncjxtgi.html

Py:   except ValueError as e:
来源：http://hz.daxiang520.top/gtfzolrlrt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtinybvedm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtxtzxuxff.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtvwhnkirm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gtufszlnjf.html


<!-- 参考信息 -->