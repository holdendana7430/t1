代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gtouekjyaa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtibfzzagz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtrtfmezxu.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gttzvzncgr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtrixvxjsu.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtwdkkokjd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtivoezpoz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtrihmbdhi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtrjokscgk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtjqwwzgjk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtallufvhb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gthpilayzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtkwiybsbz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtqkqgxwbo.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtscwcfghq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtqnnlihwe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtmlrjrbwo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtgicxxuil.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtksawibdu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtkzrdquep.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtcirvkiny.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtyowdszmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.meibo888.top/gtnhudpjwv.html

[F04] 追加写入文件
来源：http://hz.jinqigfzy.top/gtoshvhxia.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtfcwzroqb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtshzhmrwt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtdegijrrb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gteayyurrd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtahxwhzgu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtnemqzeua.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtsytdwynu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtagbpznhy.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtfwfxscvv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtxsewualb.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gttjifgepk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtwxfbchjt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtzfpruyis.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gttycjhczc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gaohongyu789.top/gtitnvxnuf.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtwslpxyxn.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtfmseqfqj.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtjouybkag.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gtxbqdegdy.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtgdsjszrz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtygfaskmx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtmxfrpcnd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtngimruhl.html

Go:   os.Remove("a.txt")
来源：http://hz.sxryk.cn/gtuulwvwjo.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtmieyhpjj.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtgqpnrlqg.html

[F07] 创建目录（含多级）
来源：http://hz.sweek.top/gtempokyyj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtbvdfiorl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gttfnrhrpm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtplggzmmv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtbpddhyvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.redwolf501.top/gtaxsbscys.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtlvtkgtlj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtsgyhtfxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtruipsajy.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtqbhitezb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtpbwwqgdm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtgojmgvui.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtebxufwpg.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtxhvdmyur.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gthiqkezpt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtssvwwtcz.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigufen.top/gtjuibecyu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtxyyzybiu.html

[F09] 获取文件大小
来源：http://hz.svipenyu.cn/gtvyfujfzi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtmemjjybd.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gtjudvijxi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gthqnsvgkx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gthkughxng.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtmuovordb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtpurisrap.html

Ruby: File.size("a.txt")
来源：http://hz.hywenlv.cn/gtkgdjkkcq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gttaacdncw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtxqaewjcd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtluwqjcgz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtgkujxjjy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gthxupyvnf.html

TS:   path.extname("a.txt")
来源：http://hz.meibo888.top/gtxhjslywr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtkijpnupk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtzczjfacp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttzzltxob.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtkfilojbp.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtggdiutxq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gttpwhxayf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtncbptlro.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtklbzohqd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtihqdrylq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hammf.cn/gtnnoilozq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtzciqxpew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtuzfsmncx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gtnsbtqwgl.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtaoxosjeu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtoemdzyxq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gttrryqawl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtflfykmfb.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtzpqtgblr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtolycbrqz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtfqmtvpze.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtyfgpxsoo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtdxaevkwu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrdgjbwdf.html

G. 面向对象
来源：http://hz.xylfe.cn/gtnejhcczt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnqkebiqi.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gtvlwlewaq.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtkjqmfuuq.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtwffqrjiq.html

JS:   class User {}
来源：http://hz.nanxuanxn.top/gtopcomnfm.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtvsitxxkh.html

Java: class User {}
来源：http://hz.nwbrower.top/gtqvhfaykn.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtyqtrjqbz.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtulievdfx.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtwbpslxfl.html

[G02] 构造函数
来源：http://hz.meibo888.top/gtgoerpvll.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtwelysruf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gtwhzpbeks.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtawbwmdcj.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtiyesitdw.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtmrpzwiqj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gthwrwhoda.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtmpywlruk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtkelijggq.html

[G03] 实例属性
来源：http://hz.sweek.top/gtillelmrb.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtgshijent.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtqzewlpfi.html

JS:   this.name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtwsbgczgu.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gtvuiwddkc.html

Java: private String name;
来源：http://hz.fzhhl.top/gtdzmvpdoj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ehwqpu.com/gtttaqbbex.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtejgmfubh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gthwkzssvt.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtckjhxqom.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtitpvymff.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtjcczfpqi.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtigtxbtyo.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtoherjcnb.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtzugezilw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtiartqlav.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gteuyqjjrp.html

C#:   public string Greet() => Name;
来源：http://hz.xylfe.cn/gtzxsifrey.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gtovvmxxwe.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtlzetilpj.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtbwsuuktu.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtsfgrqigt.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtmeaubxzv.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtgmtcumog.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtjfhyqmkt.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtyzlncmva.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtitsrhslu.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtucnjshzc.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtcjctznmb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtucvxmjpn.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtaxlffhxl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtnvxsyikd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtmbxapriw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gttfmwxrwc.html

Ruby: def greet; "admin"; end
来源：http://hz.svipenyu.cn/gtwmthugnh.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtggmxhrzd.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gtstxrcibq.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtqmpxylot.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtmppfzkdq.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gthuwlddbd.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtxbpqwwgq.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gtzjbpbctw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtymabgqgm.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtpfsxvtdm.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtbzswesqu.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtcarztoqq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtixsmipxz.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtotxcildt.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtpqliujae.html

TS:   static f(): void {}
来源：http://hz.ywan-chungtsiang.top/gtljjqkotr.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtowunrvvo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtfzbaysti.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtzmvccfjf.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtdrbqkxiq.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtzsqbamxz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtgvxjusut.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtgmpbppqx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtsuhqceah.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtfbjdwuru.html

Java: interface Shape { double area(); }
来源：http://hz.yongpay.top/gtogcxnods.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guowangkeji.top/gtpqtlbvpf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.birdmap.top/gtyivylang.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtwymlpggy.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtsznmahjd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtldcqhgvw.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtbukyxhso.html

JS:   #private 字段；其余公开
来源：http://hz.bjfxy.top/gtmblizvfz.html

TS:   public / protected / private
来源：http://hz.vqdsnc.cn/gtvduoxfce.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtllxwdrml.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtvtfabaan.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtnyolcexp.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtsymqyjkd.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtbvcdyvvg.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtzivbrxwf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtwfopvhzx.html

JS:   get name() { return this._name; }
来源：http://hz.52xcode.cn/gttmurpugi.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtojwhgolk.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtpylhlbsi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtghwjsfhl.html

Ruby: attr_accessor :name
来源：http://hz.cashguo.top/gtnpiibryb.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtcmverjdn.html

[G12] 对象转字符串
来源：http://hz.fengsongda.top/gtxwoprmdk.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtzaxntsfw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtjslgoeva.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gteauhpwnx.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtcdybaiug.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gttusqrvvd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtmuzczznj.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gtnxirpxep.html

C#:   public override string ToString() => Name;
来源：http://hz.yvedp.cn/gtdccbennk.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtwkvrwykq.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gtonscdsfi.html

PHP:  $u instanceof User
来源：http://hz.pycfn.com/gtppzhuqqe.html

JS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtzviigsip.html

TS:   u instanceof User
来源：http://hz.shuidangran.top/gtvupdvrzu.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gtdxbdvbvc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gtvvvnodgy.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtzekxxyfg.html

C#:   u is User
来源：http://hz.yonumen.top/gtzqbqaxqe.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtvzhqnlbw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtnzfcpbvs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gtjaqdsslb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtmyklbgvj.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtgrsjkjfq.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtfcyticpm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtlhlxvvxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtcfmzwjpw.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtnmfeaiup.html

[G15] 枚举
来源：http://hz.cashguo.top/gtmblbbwwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtgxsrhsfj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtlprsquor.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtxhdnhcnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtswntajzu.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtokmhmzgu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtahbuhrcy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gthmtyysoy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtjbdrplth.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtwnnfmjwt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtnumesdtb.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtdlimszug.html

JS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtisrptcht.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtzvqjacry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtrvofkqns.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtcxfywznn.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtsvtrluhg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtcrueqcsh.html

================================================================================
来源：http://hz.pycfn.com/gtafgmsrhb.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtwqkqxmic.html

================================================================================
来源：http://hz.gzhubu.top/gthcezrrbl.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtvnepjfet.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtvuqabpnx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gthlgthoye.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtnmvrigst.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtezaxeyxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtengawpns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gtwagyxpuk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtcssmmfjk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtnbqyrioe.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtlebpbdqj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtckodaqbj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtuamzxvln.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtghcuozcg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtfsrtloeg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtrathvqnn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sysykeji.top/gtcbfjyreb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtelobvtcy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtdfssewfb.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gtxxgvqgyy.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtklzzasxu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtwwoztwvg.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gthcsohurb.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtvfjacmkf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtogalgfrr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenjidiqi.icu/gtxjkcagmo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtjyvbtyul.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtwzwdievp.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtumfdnezc.html

Py:   class MyError(Exception): pass
来源：http://hz.iojbl.cn/gtrpwqujqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtsjgmcyir.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gttkyuljhd.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtwvefaali.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtmfggrcsu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gtfmsasliu.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtajvxcrgc.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtxvjdxezk.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtcytouotz.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gtetdhoqru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxinkj.top/gtpcqgaifp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtqeedwlga.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gttnyscibb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtnzeoopbu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtjmqedcsz.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gtyvrqcmvd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtjfaabotd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtkutdxfqq.html


<!-- 参考信息 -->