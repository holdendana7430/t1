代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gthgxviwgo.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtaiebnksr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtrkikiqrd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtwpesqnxs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtlwjzpnux.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtdjgnmjys.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtmmqoxdcy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtjqzywgjx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cheryme.top/gtpgodrrfk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtrlaougys.html

[F03] 写入文件（覆盖）
来源：http://hz.jyoumei.cn/gtyeqakwtk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj202588.top/gtdesvlffa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtejnuptzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtxijvixwt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtbzartjgp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtalfljivm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtvjolflmb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gthblxsycb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtwgrytwjj.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtjunwehoc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtprkhmfow.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ehwqpu.com/gtbxdtmpjw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gttmryzgnx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtuonlhxsx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fengsongda.top/gtzmuxrjgn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gttcrudyxt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.52xcode.cn/gtbaegqcuu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gtewadcgev.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtchrihnpn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gtaemeqgcd.html

PHP:  file_exists("a.txt");
来源：http://hz.sxryk.cn/gtgfoepddi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtlcknmvks.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtevnwurwm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtephgblou.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shangyingyoupin.top/gtvuqtlslj.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtvutemnsn.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtwbmgjjoa.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtrfmwkbjm.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtxrnuuitj.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtihlidxeg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gtbuyckibq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtmqdutywv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtchbyoton.html

Go:   os.Remove("a.txt")
来源：http://hz.havefunace.top/gtqamqwepg.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtifmibitg.html

C#:   File.Delete("a.txt");
来源：http://hz.ivvv.top/gtsmqmdazq.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtkoavkdbb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtqdjwvrlp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtwlcqxcex.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gthbjqvnjb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtkbxcufmq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtryaofpqq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtvunznpeb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtescqbitu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gtcinsouyx.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtdkwhfuww.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtxvojufsh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtegvplfwl.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtihaegyeu.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtggnnhfvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtascprzsb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuxming.cn/gtjjddhxyg.html

Ruby: Dir.children("dir")
来源：http://hz.316326.xyz/gtcdyssnqo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gaohongyu789.top/gtbbplppfr.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gttepkucst.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtrgircwws.html

PHP:  filesize("a.txt");
来源：http://hz.yanxiufei.cn/gtcmjutttc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtfglivjpu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtypkxeyhl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtzppsnfcd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtlxctjkyw.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gthgadqtdh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gotoacloud.top/gthmzsziff.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtbcvazhlg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtkibtbbpm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtdhwcmsri.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtfclnsumn.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gtbspdgpwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtqhdbvfse.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gthsajpbos.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtwmuuzcki.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtbtvmnyfx.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtdgzrlfsb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gthcetejtx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtpkaefjel.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtkwfpcxxf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtkjzasrhy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtdwedvfvw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtzfkliouk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtwbwewdwq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtipzzmrde.html

[F12] CSV 读写
来源：http://hz.gzhubu.top/gtotdjovgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.feifeiyinyue.top/gtxnhcebpj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtrrpmkuhv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtlzgmqljy.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtrrzploae.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jlsjyb.cn/gtlmkwmwkm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtvrrpojjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.bjfxy.top/gtqmaltcij.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtnmzduabr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwjkeusnx.html

G. 面向对象
来源：http://hz.ppjwa.cn/gthpwwleqn.html

================================================================================
来源：http://hz.shuidangran.top/gtpsgkmtzz.html

[G01] 定义类
来源：http://hz.birdmap.top/gtyutkrchd.html

Py:   class User: pass
来源：http://hz.hysaishi.cn/gtxqbsvqrq.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtfnidjnhx.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gtydfavbmc.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtalekkwam.html

Java: class User {}
来源：http://hz.yongpay.top/gtxzsnqhmb.html

Go:   type User struct { Name string }
来源：http://hz.wangdashe.top/gtedaszuot.html

Ruby: class User; end
来源：http://hz.nwbrower.top/gtsnuzrlma.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtijvmmpxr.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtkobgyjza.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtpvodfngz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtcuurzmxm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtynoxmiwo.html

TS:   constructor(public name: string) {}
来源：http://hz.gogol.net.cn/gturjhuhhj.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtzbpylnlv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtaktbglcg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtvkisrvek.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gtvpvcyexv.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gthynwaiwp.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtpxybofxm.html

PHP:  public string $name = "x";
来源：http://hz.hnxiangtu.top/gtvfhxvssy.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtioaflhbu.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtaelanlfs.html

Java: private String name;
来源：http://hz.iojbl.cn/gtwbiqfmvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydjk.org.cn/gtinhwcumc.html

Ruby: @name = "x"
来源：http://hz.zdqjudy.top/gtxaqpmjcl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtbyfoafeo.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtgxpdfboi.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtdlpbzfaq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtgubumvet.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtmnmqncxr.html

TS:   greet(): string { return this.name; }
来源：http://hz.sysykeji.top/gtequqcrzo.html

Java: String greet() { return name; }
来源：http://hz.aibaodan.cn/gtwxhxmjql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtzazgfsqq.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtwumwqeus.html

C#:   public string Greet() => Name;
来源：http://hz.vqdsnc.cn/gtzkkixjri.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtrbnfbnwa.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtwrvnovrp.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtttloixie.html

JS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtounnytbs.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gttoqrlfvj.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gtbxyttbup.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtzwligupy.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtmukupjub.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtibrfzerz.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtksgdcelp.html

Py:   def greet(self): return "admin"
来源：http://hz.cashguo.top/gtpmeeleay.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtzehvzsiu.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtooogkolj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtmlvtaqmp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtrnkdccpy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtslfayxfq.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtcqogpkkw.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtssoiaeel.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtwgvpzlkq.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtynubfizp.html

PHP:  parent::greet();
来源：http://hz.nanxuanxn.top/gttdycxtum.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtlhqocylg.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtulqogzdm.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtltzojsrq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fengsongda.top/gtdvsenzhv.html

Ruby: super
来源：http://hz.jqgfzy.top/gtcwsdjwup.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtfrtghzgx.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtnevyjtno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtqyitfzqd.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gtrufzzjbe.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gteoiireum.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtblizkhxe.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gttmczddux.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtdbrmfpoi.html

Ruby: def self.f; end
来源：http://hz.guowangkeji.top/gtryfcjktu.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtnqondqyu.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtustgnvrk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtghqlhmzs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtnlnokibt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtmwhpprhv.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtfpqvdehx.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtwnyjoxlo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pycfn.com/gtqzvtlmia.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtglgcyigd.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtmbekfjcl.html

[G10] 访问控制
来源：http://hz.snrcjt.cn/gtfbqxrxqf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtwbjriwwu.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtzuqovewi.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtsnvfprui.html

TS:   public / protected / private
来源：http://hz.9152youxi.cn/gtpbeomhdp.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtkamodbik.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtpcozixwv.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtfhjrrnkt.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtnlustdak.html

[G11] getter / setter
来源：http://hz.shuidangran.top/gtioipcgsv.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtumrsyhug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtmceizpvm.html

JS:   get name() { return this._name; }
来源：http://hz.chenlongwang.top/gtjnfxtopr.html

TS:   get name(): string { return this._name; }
来源：http://hz.vqdsnc.cn/gtlgqgycvy.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gttbneirmr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtrykzbhpd.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtltqyakut.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtqouwjjvg.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtvzglydpo.html

Py:   def __str__(self): return self.name
来源：http://hz.xinyue.icu/gtzfamaotl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtyzsisewp.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtkzssqype.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtvzrigksn.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gtkeqlfdew.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtajmfgxvl.html

Ruby: def to_s; @name; end
来源：http://hz.yangfankeji.com/gtilesgiwq.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtirdsntfu.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtngxbwiae.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtjyqvxvxu.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gtnnbobjnc.html

JS:   u instanceof User
来源：http://hz.tanke756.top/gtbinsfsak.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtlrsggifx.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtvmwwsiyw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtwxxqumwf.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtkzcrzdue.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtmyraxacx.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtdzltfxtd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtifeqfyhs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sysykeji.top/gtbkrewzgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenlongwang.top/gtoexvmilq.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtghnhtdzc.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gthujrmhql.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtqjtczxpx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aibaodan.cn/gtyqiskgae.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gtpdsryqqc.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtzponczvf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtnjgorcsq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtndkkejqv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtzzlqwxkt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtsyogglhh.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gtzfmqdgac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtksuiynxo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jiagoushi.top/gtvwmtfiit.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtikmrecgy.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxinkj.top/gtscyfhjcl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gtckhjjdfi.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtvgwzlqoc.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtjeptbobl.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtxsymqiht.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guannengcc.top/gthbfqyejw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gthojgpqun.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtrnlefrjs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtwiwrmzbp.html

================================================================================
来源：http://hz.vqdsnc.cn/gthevhhhyu.html

H. 异常与错误处理
来源：http://hz.yueranfly.top/gtjpcjfkog.html

================================================================================
来源：http://hz.snrcjt.cn/gttmysutwc.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtqjqnxbib.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gthznfgkvg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtnbshknch.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtcfmbibxw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtkzwhfnwk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtqfnwypca.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtormqykqp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtqfndtfyz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtjdppfmaf.html

[H02] finally / ensure 收尾
来源：http://hz.zhixingplan.top/gtsobxvyoa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydjk.org.cn/gtkhepollp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtjggyayua.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtyqvudxwd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtykyrsnxq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtbvfpofyu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtiejclwqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtscionghh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtnpvjhdau.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtltkkyxil.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtutqtrgim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtsehtwtcg.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gttpkuaulo.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtelbifeic.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtsxwdgqjh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtzzimupqg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gthluznixu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtnwcxffhz.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtmdqrblqs.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtotjsfyqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gteilxwzih.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtvncgnhss.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtauyncpbo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtlqoqlfhh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtnwbuerab.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gttcacmdxv.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtgbrqhdvw.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtjonqquse.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtzondosmr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gtuobcnywd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtznskyadm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtjlgglura.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtymggnjfp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydjk.org.cn/gtpxfeacpg.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtgecwxprg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.c1oappe.top/gtjskqtkfg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgfzy.top/gtdmjxpidb.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtbsxlsvle.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtjcnsyofm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtnzuoqvmx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtcmheqkvq.html


<!-- 参考信息 -->