代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtquwlcycf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtrougyoxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gteoqmcejq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gttrqqdjtc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtahtcmmjv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtzrkvhilt.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtelwggywh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtdeuivgol.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gttfadzyoc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gthzdgnhoz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtopmrcxnl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtyywwmeaj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtzaxkhowx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigufen.top/gtwaoffsvh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtkemrqusg.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtfvoahmkm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zycfv.cn/gtxgpkiygx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtqfskmuww.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtovabjshi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtwjmosmyh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtcyyowqtn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jianghu66.top/gtrovarfro.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtjdscfjfp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dianchejie.cn/gtuzgbvmda.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinyuanbaomall.cn/gtrfsiacxw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gtjygtqgcf.html

PHP:  file_exists("a.txt");
来源：http://hz.sxryk.cn/gtbsmxzepm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtcxgxshox.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtdzadbyzb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gttkkenuqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtbieraota.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gtyimwdqji.html

C#:   File.Exists("a.txt")
来源：http://hz.ydjk.org.cn/gthjrbmfwh.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtcfynayuw.html

Py:   os.remove("a.txt")
来源：http://hz.jinghuilouyu.cn/gtofazsxzf.html

PHP:  unlink("a.txt");
来源：http://hz.tian-w.cn/gtiibdulra.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtpwjfrzif.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtzpxsffdq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtibamvbdn.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gtwczkjdno.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtdhogiszm.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtqygbraie.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtjgyesgub.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgfzy.top/gtjtzotnpd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxuanxn.top/gtxfborxls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtfmrzxdnv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtantlrjwi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtinycqhmj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gttrfpyzbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuetiantiany.cn/gtnyylixbi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtsbhtsgwt.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtsdobqvnq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuxming.cn/gtewqiqvax.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.andypj.xyz/gtxixrnunm.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gthylljxbr.html

TS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtxzdbckck.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gttsgqvves.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtekktuelc.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtpxnkbsem.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtgztbtjda.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtxtlvskbd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtnvvdfkgu.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtdhiidyez.html

JS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtowtblzyp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtdyfpcthd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtpgmblbfw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtbttrdpjf.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtwlnsmxts.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtpjbqmrnc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinyuanbaomall.cn/gtgfasclyv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtbrwwmxjc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gthzyeokdh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtgiiwsbzc.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gttkuxvquh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hammf.cn/gtfffzmrcy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtadhesxle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtfdjfrzyf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtujwtqopz.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtmeyewhmf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtlqtkxgqn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtzkdgqpcm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtrmxouxok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtwixdxdcx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.vqdsnc.cn/gtjwictkkq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtfitzixxp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gttszdklze.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtwnlchgey.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtxhstsljg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtbiyokprc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtrwwrdfxk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtcphczkdi.html

TS:   // 同上
来源：http://hz.zhoulong.xyz/gtsgyqzzgn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtbnbmbwgi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtgussjqtk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtitlrehov.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.redwolf501.top/gtqngrwyev.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxhykemkp.html

G. 面向对象
来源：http://hz.hammf.cn/gtyovjhosc.html

================================================================================
来源：http://hz.tanke756.top/gtmxuzutbf.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gtyfbpbufz.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtxvagwoop.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtnrprypdq.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtvnxalsyf.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtwmeybnmr.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtexssfkez.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtprsaxrfo.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtdopvwmuk.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gteominfsu.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtkhxhaisn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fengsongda.top/gtdlfpchiv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtnbrazlyl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtpqoxfkqd.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gtvkergsud.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtgkuasxed.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtoyqeuvoc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shangyingyoupin.top/gtnloctmdm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtviclwwcw.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtbpepxiab.html

Py:   self.name = "x"
来源：http://hz.vqdsnc.cn/gtdbtpepew.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtvblvtmuk.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtkjmvxafr.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtredtoxqu.html

Java: private String name;
来源：http://hz.yvedp.cn/gtisffszfs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gtpmumygvz.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtftfyvugl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258888.top/gthqzjqnpd.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gtqtwkutzi.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtzkpqbvez.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gttupcpipj.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gttxnojewn.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtczbgsqmq.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtaiktahko.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtojhxcsrq.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtjixbvowl.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtstyzkklk.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtptbmqywa.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtdcclmooo.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtmtyhtkon.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtoslddsii.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gthutrlzsg.html

Java: class Admin extends User {}
来源：http://hz.chenlongwang.top/gtcspblufv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtfwpvqdlv.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtfdohzocw.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtyvnncnoa.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gthdmuoakh.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtcdolqzko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtydjpmonl.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtlilfvvgz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtacmgnesl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtlnjuimdi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fzhhl.top/gtlbatlllw.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gthrybeqeg.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtrbmoulok.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtxqwhoyyu.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtboubhlub.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtsnigotgt.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtfmeqqtaa.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtaahhxagu.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtzieckaha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtvjwkifve.html

Ruby: super
来源：http://hz.0kj1m.cn/gtfprjdken.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtcecsehva.html

[G08] 静态方法与属性
来源：http://hz.yuanzhike.top/gtpuvldtzu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jiagoushi.top/gtxwqtytts.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtyjrpclmg.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtmzejimmu.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtmoqucuti.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtjbqqvdzv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtshelgvxd.html

Ruby: def self.f; end
来源：http://hz.zhijiandao.cn/gtmlqydpjc.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gtifciurnm.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtqubzubpf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.snrcjt.cn/gtqybbmxms.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtgrqllcuc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtruttefaz.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtsnfvoalb.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtpxjucnrh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnxiangtu.top/gtbzbrhovq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtdxintpzr.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gtlphtthtm.html

[G10] 访问控制
来源：http://hz.yueranfly.top/gtvvmdtrye.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtgwurzshk.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtyzmtrgmt.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtqrabcpzr.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtcffqlfkl.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtiunfqwps.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtebtkefrx.html

Ruby: public / protected / private
来源：http://hz.ydzc1.top/gtslcrfozq.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtjrvhhepa.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtszwhsepj.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gtbhhiiijt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtmvrzfvpc.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtntbmczpk.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtrpvomkkm.html

Java: public String getName() { return name; }
来源：http://hz.aizwys.cn/gttofpcyls.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtyicuyxmw.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtkydwqjcm.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtgfkqilzs.html

[G12] 对象转字符串
来源：http://hz.gaohongyu789.top/gtqibubwuv.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtekitcifd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtxatlxpfk.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtycptlczp.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtvheenonr.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtjvttkqhx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtuoqxvpvt.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtcrvoomub.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtdncvkcdf.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtiwhvhoqu.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gtvbyxmbeq.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtdmwdekyw.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtntjszfzf.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtikfhtrtu.html

Java: u instanceof User
来源：http://hz.sysykeji.top/gtwtijfhow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtakkdqvko.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtqgnyhpoj.html

C#:   u is User
来源：http://hz.smart0.xyz/gtfjrwmoit.html

[G14] 数据类 / record
来源：http://hz.smart0.xyz/gtaofslwfe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtktykidpe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhengqikj.top/gtcwrgfpnp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cashguo.top/gtsdkeolwr.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtmmfcdatg.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtxdxzznpl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtplwpitiu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtllocmdco.html

C#:   record User(string Name, int Age);
来源：http://hz.hammf.cn/gtnsqzgrvr.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtjthcnxix.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtcyluplgq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gttbtipypd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtdkyxaqqk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtaxrhkaqd.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gthumzgxec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gtjcoghtya.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtafgjjuuh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtwdasqbpp.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtwqrmlcdg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtilrpkmqa.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gthaleykob.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtopeqkttp.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtkqiqxcmz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtxgzkysls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtmrjhcmkb.html

Ruby: obj.instance_variables
来源：http://hz.cheryme.top/gtwwozjwvy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gttfebnvui.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthzxawwnl.html

H. 异常与错误处理
来源：http://hz.jinqigfzy.top/gtmlcqhdds.html

================================================================================
来源：http://hz.zhoulong.xyz/gtvluonnwl.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtmmileyjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtaasleort.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtsvyhuelj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtthdlztxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtmkvtdjmh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtifpjebbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhiwuduotai.top/gtoyfczjvm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtinogrzmx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtwlsgphke.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtvfevkfel.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtwolztqij.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtyoxydxes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtfegyybsy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gttykyvull.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtoetyvuex.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtqdajzfep.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.kuanghao11.cn/gtbnckkvjr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtskilknzu.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtjgcyqdxy.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtdrkzsrhu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtbqptjizx.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtvwixwcxv.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gttszgutxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtryiolqfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtdfoofwzo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtpxmxgxro.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtphmwkexm.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtbhsxzmfz.html

Py:   class MyError(Exception): pass
来源：http://hz.tanke756.top/gtuhnxibbg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtdtfdnzge.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtlonqxhfo.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtmcpeujii.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gtrcuphrqy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtzryouudh.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtnzlrikvq.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gthavkepke.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtqwhiujrb.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gtsrmnnudn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtqnaferlj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtnswslagh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtusgftlmm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtqxgprugg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtkdqnyden.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtlxtckrwx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtaelirnub.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtrfyxhlyh.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtelkqezpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtksrlvisx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtotnyhgdk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtsxvqybks.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtvlwcfihg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtvsfeabji.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gtehucjces.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtodcgvyxj.html


<!-- 参考信息 -->