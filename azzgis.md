代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gthrujwkwp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinyuanbaomall.cn/gtkinvkigr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtlqadgyqb.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtdifxzhsc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhengqikj.top/gttsaxfntd.html

================================================================================
来源：http://hz.sufxvd.cn/gtiqnqezss.html

F. 文件与目录
来源：http://hz.c1oappe.top/gtpnkazazb.html

================================================================================
来源：http://hz.sufxvd.cn/gtspizphzw.html

[F01] 读取整个文件
来源：http://hz.sufxvd.cn/gtltwafzqx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gtoofyrtjr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtquhbyrcl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtmhfbaktv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtxzqmnclf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtczwghbzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtavtikfhc.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtzmscgqki.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtjjeluicm.html

[F02] 逐行读取文件
来源：http://hz.chenjidiqi.icu/gttlqnzrob.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtfcadfdva.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtxebzxrxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtdrwxbsgn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gttxntqbjg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtmqcnvqmk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gturcuhdyx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gttmdsacio.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtrdbiovks.html

[F03] 写入文件（覆盖）
来源：http://hz.jlsjyb.cn/gtrytkttvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtnhdwgcht.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtxhbgmbrg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtjtxnhmrp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtmisanifz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtnebhhpac.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtlpgiridu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtcphyhjkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtvqcqiwwg.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtuvzujfdm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gthcixsneg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtpscaxhoi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtirujsjcy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtxatwmnpx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtngfyroni.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinyuanbaomall.cn/gtzswkypej.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtxoqnupvk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gttuezwppr.html

[F05] 判断文件或目录是否存在
来源：http://hz.jyoumei.cn/gtkkqbymkk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhaomingkeji.xyz/gtbfvooppx.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtwjzlkqcd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtifpztwmd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gttowghjmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtlbbvjapy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtsgkfvwpx.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtthsvszuv.html

C#:   File.Exists("a.txt")
来源：http://hz.wangdashe.top/gtkedztdwp.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gtolyppmhw.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtahulwxrw.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtspmgccfh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtokjuxmqq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtjqnusmuq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtkrucjyfz.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtqxzkonln.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gtqpgtiahp.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtfgjyexgz.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtnihmkleb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtftzlbaje.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gtuqtwhfmm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtxjtjmcqy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtnzodrjqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtentefvhh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pycfn.com/gtbvwvsmpf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtxjpxhuev.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.birdmap.top/gtudofgcyz.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gtojneqjgd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ehwqpu.com/gthjoojpqj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtdmqucfdu.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtftrpddzh.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtiffdbxlj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtwacpqdip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtnyqjbnrs.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtkafjjerz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtxchgstwd.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtbhigfgwj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gtgohgwfvw.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gtiscadolk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtyomcsyih.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtfljmgghp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gthivikimb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yvedp.cn/gtxbizuheh.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtgpiofdag.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fzhhl.top/gtqbtkxbtn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtfmlquqki.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtupxiovuu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtoyuvowhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtvkeotqzn.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtemfqntdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtacbpyznb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtnxrmbbws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtjjysrscl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yonumen.top/gtsajakstv.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtrwcstlic.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtqhgjolww.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtavdfgapn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtmzncysmk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtbgzhnhkl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtlevlhptv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtxdohjnat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtastdovwe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gttnembypb.html

[F12] CSV 读写
来源：http://hz.quarkkingdee.top/gtyejweyiu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtxwnkfiuk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gteljoxest.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtfbsyxfcg.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtsmqkiquj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.iojbl.cn/gthtwkodqb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtvozcubhl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxinkj.top/gtzghqksri.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtjluibczj.html

================================================================================
来源：http://hz.daria6918.cn/gtxcpyettv.html

G. 面向对象
来源：http://hz.zycfv.cn/gtuytborvj.html

================================================================================
来源：http://hz.yongpay.top/gtwxwipbap.html

[G01] 定义类
来源：http://hz.havefunace.top/gttscbbcxp.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gttrtiiuao.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtrauxabyj.html

JS:   class User {}
来源：http://hz.sweek.top/gtwejepekj.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtgydjyauj.html

Java: class User {}
来源：http://hz.havefunace.top/gtyplyppky.html

Go:   type User struct { Name string }
来源：http://hz.vqdsnc.cn/gtxicbxmnv.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtipxpsztx.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gtdbxwxykg.html

[G02] 构造函数
来源：http://hz.jiagoushi.top/gtxnzsyfxf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sxryk.cn/gtnvbsncyl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtkekwgkmu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtshqayyri.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtcuqgwwlp.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtftuetxpf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtydcnsqrj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtvulmbaad.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtawomhnyd.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtcixxjuli.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gtnqhqlcxy.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtnmctsyry.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtwxojotpd.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtlbfoftuj.html

Java: private String name;
来源：http://hz.gotoacloud.top/gtzmqudgaz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtyylghpqf.html

Ruby: @name = "x"
来源：http://hz.c1oappe.top/gtlcyohzme.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gthvsbyoiz.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtkkcebdsb.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtpaeyoqxa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtxpgkvohr.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gtrojahqia.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtavlfogqw.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gthwawvlel.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtgijdgoal.html

Ruby: def greet; @name; end
来源：http://hz.ywan-chungtsiang.top/gtljnuyegj.html

C#:   public string Greet() => Name;
来源：http://hz.yuanzhike.top/gtvbemrfdy.html

[G05] 继承
来源：http://hz.ivvv.top/gtfstejigz.html

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtmsalyfrx.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtjvascnwc.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtdbqkqrdk.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtpxtmjxcu.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtvuvruykw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtzgudcrrr.html

Ruby: class Admin < User; end
来源：http://hz.bjfxy.top/gtwkyszdoy.html

C#:   class Admin : User {}
来源：http://hz.jlsjyb.cn/gtepfugaqj.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtrmygdmwp.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtmuipujze.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtsmvhnxdv.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtdslkrlat.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtropjovkv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtnavundbt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtofmqgndh.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtdjwuexap.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtriijiclc.html

[G07] 调用父类方法
来源：http://hz.cheryme.top/gtzzhmagbc.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtxuodhmil.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtfgncubju.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gttbqavmlk.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtbuejevcy.html

Java: super.greet();
来源：http://hz.pycfn.com/gtwglsgrir.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtgzisbzlb.html

Ruby: super
来源：http://hz.chenjidiqi.icu/gtemiecfwx.html

C#:   base.Greet();
来源：http://hz.shuidangran.top/gthcjvzcgy.html

[G08] 静态方法与属性
来源：http://hz.xuanzx.com/gtxtuflgts.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtvxqilhcw.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtixyiypti.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtmjlsvfxn.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtwrgurpnj.html

Java: static void f() {}
来源：http://hz.guowangkeji.top/gtqnllrqae.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtzryepngq.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gtgwlegvyx.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gtqkwbezkl.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtubtvbphm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gaohongyu789.top/gtxvnkbels.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtxnfcwohv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtbbcnoabi.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gtggzkvhje.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtcihiiqcn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tianlin.xyz/gtnoognsmh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gttpkguxgb.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtrvrnqvuq.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtvvkvzbpe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtwuzfvrba.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gtzegoblpe.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtoaajmtjh.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtefikehaz.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtwkvmikop.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gthgjcutvf.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtzhcipcko.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtrnlfxckx.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtyztvoeaf.html

Py:   @property 与 @x.setter
来源：http://hz.sysykeji.top/gtpmsiwoqw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtkbzqbbne.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtauzkxsuh.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtltxaykzx.html

Java: public String getName() { return name; }
来源：http://hz.jqgfzy.top/gtgzxulwhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtdmdmgips.html

Ruby: attr_accessor :name
来源：http://hz.jinqigfzy.top/gtzoiipvyc.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtvwqremda.html

[G12] 对象转字符串
来源：http://hz.nanxuanxn.top/gtgamfdiyp.html

Py:   def __str__(self): return self.name
来源：http://hz.wangdashe.top/gtviarfuta.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtcmbxakbe.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtwthizzaj.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtkldbyjrk.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtconnbaen.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtgorhzicj.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtmjmzajjj.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gthesmwrax.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtwbqucjdz.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtuvotrhtn.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gtytpxixeo.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtfdmrkyfa.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtroovcgnw.html

Java: u instanceof User
来源：http://hz.c1oappe.top/gtlepymalm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtjeqzlfzn.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtekeatfgi.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtoqaivtff.html

[G14] 数据类 / record
来源：http://hz.cucudq.cn/gtbinvryfz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtzxhknlof.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtbhbyzdkv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtbzzlywme.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtgoalnqkt.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtmobhwegj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gthoeajwpn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtrsrmetbr.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gttehfbxnu.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtqclaoima.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhixingplan.top/gtrhlhzgnj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtxlkdnkgf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtptsjumau.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtbshhyimu.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtuselvvij.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtmujiwhtu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtutpduocx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtrpivmdnv.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtxkujebyr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtoucjmyja.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtrgtzfsli.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtdiimhhpa.html

TS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gtfwumdiyv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtykcijtyz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtdutoywfc.html

Ruby: obj.instance_variables
来源：http://hz.yanxiufei.cn/gtprcdghth.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtobkmnwqp.html

================================================================================
来源：http://hz.guannengcc.top/gtwihcheea.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtcrvezmqx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmluucnje.html

[H01] try / catch 基础
来源：http://hz.sxryk.cn/gtqdjqlnox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtebdlhmnq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtmgwqsvij.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtexsxrbqc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gzhubu.top/gtunlscerf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtvmjizhbx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtpimwokmt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cdnleiting.top/gtmbxsmvoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtgyrbkevd.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtlkorkudu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtetcvpwbt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gthuzyyoeg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtwurxqwpe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtlsevapwb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtdsjoauin.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtqifrroeo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtztkvwjkw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtzsrmkgzp.html

[H03] 主动抛出异常
来源：http://hz.zhengqikj.top/gtbvcnknoi.html

Py:   raise ValueError("错误信息")
来源：http://hz.haohaochexian.top/gthsshvnak.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtzbelzrpa.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtngnpkpsu.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtvnaaqtrn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtrohkcsiy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtzqrhbafv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtdeowtdrg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtkaznbkrj.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtqppxbiks.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtlvmpvjao.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtqugguynh.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtvujscncl.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtunxysbjl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gtjyvttoef.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtvmdkpfas.html


<!-- 参考信息 -->