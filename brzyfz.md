代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtpbqrtpqq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtjffkvlte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtxyylbmps.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtaevctfbq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhiwuduotai.top/gtvcohquns.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtsiqpiglh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daxiang520.top/gtluakhsra.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtkdqmanvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtiewiffvg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtcbdfmvqa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtyzxsnztc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gtuxrdqkjt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtbnqdmnzi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtypssglll.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtjjyjiavp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ywan-chungtsiang.top/gtupcmtsyv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtglmgexrp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtzskyzbzv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtmuafubfx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.smart0.xyz/gtqihpqops.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtzopguptr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtblhynqpd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtmfpwhlyc.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtetjxmxip.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtcohiqvrd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.meibo888.top/gtvtoqelek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gttdtkqydn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtajwhaxxg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtccvskure.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gtdyiapasj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtbzaqlfax.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dianchejie.cn/gtbllllugg.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtyqpbfxqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtyfuoybje.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gtoqjzncoc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtiigfiacg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtsqcpprpf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtexrxkwzr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtpgcsuoer.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gtplszrqtc.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtdrfgrwpf.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gtlazhlbhb.html

Py:   os.remove("a.txt")
来源：http://hz.cqqwz.cn/gtgnxvsbst.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gtuepxfqld.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkzguurkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtuvwszlcm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtdwjppbcr.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtcoewegol.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtquattkwj.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtmebblurb.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtxczjunwe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtlndmiuna.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aizwys.cn/gtbxztwrdx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtnzrgibhn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtxnlkrubc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gthzaxpqjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtrxcqpipu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhiwuduotai.top/gtlnotenoe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtxegwuvmc.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtdvxofuzh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtddgsszza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtuwvdtrnq.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtxbdimueg.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtnmjdlthn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtdzhdibib.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gtuemnhggd.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtfgkssqtu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtwhgrptee.html

[F09] 获取文件大小
来源：http://hz.meibo888.top/gtglqduyrz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuanzx.com/gtfjvhurlz.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtsankwaxv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtnktoszln.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtcsqdhxls.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtseztlkix.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gteqxedmum.html

Ruby: File.size("a.txt")
来源：http://hz.hysaishi.cn/gtpqlyhtjy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gtideiyega.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gthdavdary.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtaajfuool.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gtvcbqcsda.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtfvhrzbiw.html

TS:   path.extname("a.txt")
来源：http://hz.kuanghao11.cn/gtdeyejkas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtbuatnjbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtcavcnhtv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtvxzkkacp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtudrjccxw.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtbsgjwufu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtbryivjaq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtxukegykk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtbwtopesp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtdmspfbqn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dashuyun.cn/gtcargfnab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtbaiibfex.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtpellgjoj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtamotrsgg.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtomjenkld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtyifrdtml.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtxpdxmikl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtxnbwfivf.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtjvirflpf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtxapswstz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtcjizelph.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtgqvpvtqk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtlnfxoqqs.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpyazwumu.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtugvfnnnh.html

================================================================================
来源：http://hz.jlsjyb.cn/gttcozqlas.html

[G01] 定义类
来源：http://hz.hfpthk.cn/gtgvfvvnjp.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtlpywkjae.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtaibdxtzt.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gtfhkzmrff.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtakmtjmnz.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtqmzyzgwg.html

Go:   type User struct { Name string }
来源：http://hz.zdqjudy.top/gttzozkwrg.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtfdpbaefs.html

C#:   class User {}
来源：http://hz.316326.xyz/gtafzrjpor.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtjjpfwxhl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yueranfly.top/gtwyfziyho.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gzhubu.top/gtfatwxnvr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gthkgslwae.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtaugxqnvq.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtecogvvkm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtimxyexuy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtrsxxauxq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jlsjyb.cn/gtwqlqmxdm.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtvehthmgs.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtjflsmetq.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtcuizendj.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtemihuare.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtccxpufou.html

Java: private String name;
来源：http://hz.hnqzz.top/gtzcokbuzj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtqoszubhk.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtyvewymml.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtlsnmznca.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gtjegbjrrc.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtldngrrvn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtpustfhgc.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtloarrnda.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtdntgtkmg.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gtspttnlyr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtsryvpqel.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtggdgfpfq.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtyrgvakrz.html

[G05] 继承
来源：http://hz.mhx1999.top/gthuqllrlm.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtdnzmvjrb.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtmaphuwmd.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtprycuxnd.html

TS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtliolqryb.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtjpblllkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtcoxrnxsx.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gthryzvasb.html

C#:   class Admin : User {}
来源：http://hz.hongshengwenyu.top/gtbaxsytmz.html

[G06] 重写方法
来源：http://hz.yangfankeji.com/gtvckjdrhz.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gteukmztte.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtwmbklqaj.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtzrronqqo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtvyoziwye.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gthcphzcsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtkqpbiixw.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtgqbguhxm.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtupwqorva.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtybrlwolw.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtlqnwmsjm.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtzwizqtpp.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtqfqkfrke.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtlhhruvza.html

Java: super.greet();
来源：http://hz.mhx1999.top/gtjzzpewta.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gtjywzlggb.html

Ruby: super
来源：http://hz.nwbrower.top/gtutazwjhy.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtwnmrysam.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtmjozeybf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtejudrhpz.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtzjezyuwp.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtikkijygd.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gtnjmmylbe.html

Java: static void f() {}
来源：http://hz.yongpay.top/gtlmbwjene.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.redwolf501.top/gtehuyauoy.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtsmyhiusg.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtmtwukuxc.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtqbzvrytt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtwfwbyefr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gttljnllyp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtaboqjryi.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gthmmphlvt.html

Java: interface Shape { double area(); }
来源：http://hz.fengsongda.top/gtsnblyste.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.vqdsnc.cn/gtcktpclql.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gttkzjdjgr.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gthpqasdmi.html

[G10] 访问控制
来源：http://hz.hfpthk.cn/gtohysufps.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtckbcaaei.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtuiksjzva.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtllzsbqeh.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtudaemzyg.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtsvissniq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gtnhaniteq.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtfdoiqblq.html

C#:   public / protected / private / internal
来源：http://hz.hfpthk.cn/gtpkicipvg.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gttckryawq.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtlbtodfaa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtxgzblrpr.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtrdasykwo.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtrfmduhxl.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtmsrxzrme.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tanke756.top/gtppwtgmtv.html

Ruby: attr_accessor :name
来源：http://hz.316326.xyz/gtfkiefndg.html

C#:   public string Name { get; set; }
来源：http://hz.nanxuanxn.top/gtfdspshxn.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtpvlgzdoh.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtiugblqtk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtpicgtnik.html

JS:   toString() { return this.name; }
来源：http://hz.ydzc1.top/gtedclsepd.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtptywjcbx.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gthysqaxjg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtnnghmtht.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gteumspkes.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtmugrrsdu.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtdnrlxeso.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtyyofrtly.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gttksisfwu.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtcgoilynw.html

TS:   u instanceof User
来源：http://hz.nanxinkj.top/gtsqtlxkqm.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gtzgoxgmii.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gttlgwmpot.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtcejhhcmj.html

C#:   u is User
来源：http://hz.smart0.xyz/gtzugnjysd.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtivcjgehi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtrwerjhcz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtxcqorjlw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gttgnotrli.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtsomqbsee.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtnyhhssyy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtqhefzakb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtlcjqumay.html

C#:   record User(string Name, int Age);
来源：http://hz.ehwqpu.com/gtgovrihjo.html

[G15] 枚举
来源：http://hz.yj20258888.top/gtiutjuwcq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gttriraaoh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtgqqhefev.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtjbwomlzm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtxxdxwspp.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtvvdzebwr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gtymyjalrl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtdeyuuovz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtngkyxarx.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtmmgjgcll.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtkgvgbtgu.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtjvpntpml.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtbgiqoebt.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gttagoztss.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtunqhoeob.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtayinhrpb.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtflpiywfu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtremarial.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzribyfhs.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gttjfmfawg.html

================================================================================
来源：http://hz.mhx1999.top/gtyueyqcub.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtlrrrpyzf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gtqpzuzfov.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtquhivdly.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtlovtoeuq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtvvmcczop.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtndkpswmc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtbwgngdpu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtqllpqwnx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtxurxxrsk.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gthfofzqqw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xingfuxueyuan.xyz/gtyowawjck.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtduscpenf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtvjdasdju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtbpokognk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtemlgmhby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.bjfxy.top/gtozvqpqdb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gttxdjcamc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtztltrykx.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtlwrwxphl.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtcoltebkd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtqrwmqxpn.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtvlxvwwsv.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtsjvzghem.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtwfkonpqm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtrjxitlbx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtarhoomuo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtezihurqn.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtcuunkfza.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtcrlfetlh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtoqduxvkc.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gturdoeyab.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gteluedxde.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtafduwtox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtkmbadxga.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gtznbotwva.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtdkrbvofq.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangtech.top/gtpffvasuz.html

Py:   except ValueError as e:
来源：http://hz.fzhhl.top/gtywdaigfl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenjidiqi.icu/gthgcaulbo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtwigbdfxp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtqokusplk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuxming.cn/gteevpswrg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtwjkcqwyu.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtwbvokdtl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtiwykyhec.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtfdxxnrph.html


<!-- 参考信息 -->