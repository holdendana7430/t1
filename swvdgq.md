代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtjgzqhpey.html

[F02] 逐行读取文件
来源：http://hz.guowangkeji.top/gtrxkwqtnt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtexkxczuh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hysaishi.cn/gtcjfgjgny.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtfrcpeqlu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtvisolbvu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtlcjqnoyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nwbrower.top/gtbalxijer.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuanzx.com/gtoljsgpat.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.0kj1m.cn/gtppttgotk.html

[F03] 写入文件（覆盖）
来源：http://hz.sxryk.cn/gtisertscd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtugwjzjxg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtovbidlfj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gthinnkdpt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtiradvmol.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shangyingyoupin.top/gtkqpiueuf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gthucqemip.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtqezunqhw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtlzwfegkx.html

[F04] 追加写入文件
来源：http://hz.gzhubu.top/gtumwhcnhg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.9152youxi.cn/gtyqkdupih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtgsycnrxf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtbgbgvpru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtbzuvvxll.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.feifeiyinyue.top/gtapgayzml.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtzkjbofog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.feifeiyinyue.top/gtavnpkfpe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuetiantiany.cn/gtgmplouwi.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gttblwchlk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258.top/gtbstiylrx.html

PHP:  file_exists("a.txt");
来源：http://hz.wangshuangyany.cn/gtlsdyiqfw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gteuvbuufb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtygxvxgrh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gthtdtrhfw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtkrbftcll.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtsddnyriw.html

C#:   File.Exists("a.txt")
来源：http://hz.dianchejie.cn/gthhhfbzbn.html

[F06] 删除文件
来源：http://hz.hammf.cn/gttgqxsesx.html

Py:   os.remove("a.txt")
来源：http://hz.sweek.top/gtwjzapbrs.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gtqlbmyuug.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtbfuhtkex.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtkmxknzff.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtlyyynfbl.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtgxnjzcou.html

Ruby: File.delete("a.txt")
来源：http://hz.zdqjudy.top/gtapfbeszy.html

C#:   File.Delete("a.txt");
来源：http://hz.yonumen.top/gthkuhoblk.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtnwucxgmo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtxtvykwxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtoktztblw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtlpieqfkv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtltkgoihd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gthyiwlrst.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtgczaitab.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtgaurqdly.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gzhubu.top/gtdnmxizju.html

[F08] 遍历目录
来源：http://hz.hfpthk.cn/gtirnekaoe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtghauksac.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtuyqkscae.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtlzvifoxa.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtrywyyhst.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtnvefaouc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yueranfly.top/gtzlipbyor.html

Ruby: Dir.children("dir")
来源：http://hz.316326.xyz/gttzcsjvkd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ppjwa.cn/gtakpnorhk.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtxtkwaxar.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtflygsfye.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gtdshzcmva.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtrygywifx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtunsiqulu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtwsueabxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gotoacloud.top/gtwskcxbwt.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtwkpgouyl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gteyhdyqos.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtjdmrwcci.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtfwwppmiq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtdeifarfd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtffkrckfy.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtrcihmidm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtvhladxvb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtktsmcfaq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtpdtwebdu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtycosocdt.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtcicloxqc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtemglhevv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtlwmucyft.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtdicnhkcp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtpetzrqnq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhaomingkeji.xyz/gtqhqeibpb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtxevtuyyt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtbojxwmzl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zdqjudy.top/gtzzlsyype.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtvrxmfkjn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtrewcfxak.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gttlrvmcea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtpqraovar.html

TS:   // 同上
来源：http://hz.smart0.xyz/gthqjucqrz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangkeji.top/gtgrqujdec.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtrxdipmoi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtvvmfeooq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtxhlyutzy.html

================================================================================
来源：http://hz.cdnleiting.top/gtrjunhqmf.html

G. 面向对象
来源：http://hz.cashguo.top/gtveovyjtr.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdhmmefqw.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtabzlxmwy.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gttqphwzbn.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtymripips.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtlisaoycc.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtihcojtuy.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtjepmkexy.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtsmguryno.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtolpexnkj.html

C#:   class User {}
来源：http://hz.chenjidiqi.icu/gtggbiwaay.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtboaddxhq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtznvfjtxx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtkjazpwew.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtyslllulw.html

TS:   constructor(public name: string) {}
来源：http://hz.jyoumei.cn/gtkigzndqz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtmqmjsozz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtjynbwoat.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtsnfwvcrh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtxrbcqcaz.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtayyovgro.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtxnqjfexg.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtixpckthy.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtdedndpno.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gttukinkap.html

Java: private String name;
来源：http://hz.sxryk.cn/gthtlzznkr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenlongwang.top/gtirznjhhe.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtporrmkhi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gtvabuetgc.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gttedaqfuw.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtttinlqdn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtxcuhxjay.html

JS:   greet() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtesgydplb.html

TS:   greet(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtpsohllgl.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtzodgcnxp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtepkdzeig.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtqtpvxqck.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtgyhvkjxr.html

[G05] 继承
来源：http://hz.smart0.xyz/gtakvioqky.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtaywhfntu.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gttkbtefrv.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtxkterews.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gttvkaksmi.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtjlfpezpz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtdzwdxxqz.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtwcladklv.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtbuvcurqt.html

[G06] 重写方法
来源：http://hz.yongpay.top/gthikxjanl.html

Py:   def greet(self): return "admin"
来源：http://hz.feifeiyinyue.top/gtevzbbvao.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtimfuwckq.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtseednkoi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtlbwbfqmz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtqcrnvrrp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtpkqoetcp.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtqmdehcbr.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gttzxulmox.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gtotqrxsap.html

Py:   super().greet()
来源：http://hz.sysykeji.top/gtmtbfercn.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtbylgcjjk.html

JS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtzgpwwoys.html

TS:   super.greet();
来源：http://hz.xylfe.cn/gtiqzxrptk.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gthnefbkiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtadpytjfd.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtxbbfhxdg.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtrxlscqzo.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtrojiziom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtkbhprlyx.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtyjzhterp.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtybykvegv.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtpwyzhppn.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtdxotacqy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gtmymtjxma.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtffowhito.html

C#:   public static void F() {}
来源：http://hz.chenlongwang.top/gtmkmwiyrr.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtnfmifeue.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtanquqpyi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtzdqjqryo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.birdmap.top/gtrzcqpmaq.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtboqrvhdx.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtfxayihhm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigufen.top/gtedcdeejn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtfaywzjbt.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtqpkcoivg.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtfrzpbgcm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gtefagpgxx.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtqjvdncls.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gtskrmxebt.html

TS:   public / protected / private
来源：http://hz.yongpay.top/gtlomiataa.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtbiskvbte.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtfycgssfi.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtojqpjqdi.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtozaqslxe.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtvlpgewsi.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtwjshjvbr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gtctoxipid.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtampvlocl.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gthmvxebpj.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtrdcibbfp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xziqi.cn/gteoalnwss.html

Ruby: attr_accessor :name
来源：http://hz.jinghuilouyu.cn/gtpswrzkcj.html

C#:   public string Name { get; set; }
来源：http://hz.hywenlv.cn/gtxoowwdya.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtsqztctjr.html

Py:   def __str__(self): return self.name
来源：http://hz.jianghu66.top/gtxbwwuzoh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtcxfzspwi.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gthxqawedy.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtauiuurbc.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtnsnjtutf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gtlfiekwdb.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gtsdauqcaj.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtkucnfrvv.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtimndiokm.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtnoujsdmo.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtxgqjirjk.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtlxnriioa.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gteccffbdp.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtndlkotbp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gttdabuxoj.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtjypcpelj.html

C#:   u is User
来源：http://hz.birdmap.top/gtroykuknf.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtzmjpgdrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.52xcode.cn/gtodngsxzf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtgkntmxyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtlooyigri.html

TS:   type User = { name: string; age: number };
来源：http://hz.shzxlz.cn/gtoovrnebq.html

Java: record User(String name, int age) {}
来源：http://hz.yongpay.top/gtmqxcrzqg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gotoacloud.top/gtlpddqsre.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gttwvpwxwp.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtbtnyfsyd.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtdgqctzmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtyibgknty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtkvrplerq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtipacbjqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtwarqozuu.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gttdepqlkb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj202588.top/gtouosmkhu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtelhtvofi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtrxkdzjqy.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtaibzxbbs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtfdlqpqfk.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtdflwwhtu.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtetxurdzd.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtviyiahxj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtrsducbcz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gtjcixcxbw.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtilovihvo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtuqgbjmja.html

================================================================================
来源：http://hz.havefunace.top/gtvehdftcc.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gtwkqegjud.html

================================================================================
来源：http://hz.tian-w.cn/gtwyypjfqi.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gttfcaeltt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtlcjycxef.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtcjkgcldx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtlwqnpxjr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtzrbclvse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtsujszaqn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ppjwa.cn/gtvkkdoybp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtsdtpyqkm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daxiang520.top/gthankbxyn.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtkqxamrwh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtsncbtthd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtjvfzxmjs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gttgdtoebx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtvsddnftc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtdjlxwyse.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shangyingyoupin.top/gtyceiawrg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zycfv.cn/gtccqqpgga.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shzxlz.cn/gttevxepia.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtusbbzvcm.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtrduewsca.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtaspvossl.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtsvxltpnu.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtyailwpto.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtaisalymf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gtglwhylbt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gthmldsqnq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtlhzyptlm.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtzyzjaugb.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtnzbbhrmf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtlzarcvlm.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtbgldrhrz.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtkzwyhkhb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtyzfhsfqw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtsxyufewz.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtasfzlxmn.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtfsenkddz.html

[H05] 捕获特定类型
来源：http://hz.pengpengdd.cyou/gtuzonlvbg.html

Py:   except ValueError as e:
来源：http://hz.zhongyouzk.top/gtniksgnoo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtydtrsvca.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gttyvxxufx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtvobnlqwc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtpminmokh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtjvpdlzwd.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gthvlifyqu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtnuyskezr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtdlbhoojx.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtezrfcljr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dianchejie.cn/gtvhnmvsrw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtyeiguphs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtbcfrmckw.html


<!-- 参考信息 -->