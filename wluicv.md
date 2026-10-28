代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtcqupsugs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.52xcode.cn/gtjgacyjaa.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtbhiwmnwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gthdwplapg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtqzaoagwb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtlioqitpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtcnuxdwgu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtltlkkqnd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guowangkeji.top/gtreuypdki.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtyinktaui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtnvmiiwul.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gthnlroodg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtyhqkhbmo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jianghu66.top/gtwjlpdhtu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtcvkccbnb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtcdtxdjxv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtmdylksvx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtmfzkaurh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtgzkvhqjg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxinkj.top/gtmymwberi.html

[F05] 判断文件或目录是否存在
来源：http://hz.daxiang520.top/gtbqxfexpw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtaftjjgef.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtlnvzdtyu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtzlkuxkeo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtjxieazwv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtuapphvqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtqjiaeuvd.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtooiubdkt.html

C#:   File.Exists("a.txt")
来源：http://hz.gotoacloud.top/gtdchhwkuv.html

[F06] 删除文件
来源：http://hz.cdnleiting.top/gtzcyxwifv.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtkgwqewbk.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtgpnamjxo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtdlfmwddu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtozkvkxku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gthfqybowa.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gtvpwsvien.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtkdltmsbh.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtusirulpg.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtdzomtaap.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtemgolmcc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtrdbvtdcs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtkssxqlev.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtxxetlbyz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtkzwlezmp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtqewaoghe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nwbrower.top/gtxojdspio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtiseasmrw.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtmndnegjb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gtkyltgick.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtcvzlrsqd.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtlwenxzzz.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtyfjsvndn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtprngdybi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangtech.top/gtlzqzjrmj.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtyznehtcf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtxrcqfoek.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtbwzncsva.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtlxbikcsc.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtiyfresur.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtijveosdm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtoevhismh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtrwjkpcor.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtmwgyjytl.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtdcdqhpqi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtgmxodhje.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtfchaszdd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtywybdbes.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtjhdeehig.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtbyjrsalw.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtxecexsdh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtoucyqjzy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtzqkwuevv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtizjztzus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gtjamxnyoe.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtaxvelvhp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtcdpmvaqa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtoqsatgqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtflpeauhq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtdnaiyihd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtelqdjesr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtbwonjbzc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gteksyvwiy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtctvgmsfh.html

[F12] CSV 读写
来源：http://hz.jinghuilouyu.cn/gtevtklweh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtfqzlijpi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtioqvnxov.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtnycnvkjh.html

TS:   // 同上
来源：http://hz.jinqigfzy.top/gtgsnmqwhe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtxyuoklpt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtymvdvert.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxinkj.top/gtkvvcjdvq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtormhyqxx.html

================================================================================
来源：http://hz.guannengcc.top/gtctnqpvaz.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtehmsbbkl.html

================================================================================
来源：http://hz.guannengcc.top/gtxlevduvp.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gttixmnopg.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtamhzvtlh.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtyanmziep.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtpijkcrfd.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangkeji.top/gtmbuhtzrs.html

Java: class User {}
来源：http://hz.fzhhl.top/gtdwjikbam.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtekwonvqp.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtpwhpjkej.html

C#:   class User {}
来源：http://hz.birdmap.top/gtodmotepe.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtbzprgvwe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtocabttdm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.redwolf501.top/gtlscuzggl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtchzocodg.html

TS:   constructor(public name: string) {}
来源：http://hz.yueranfly.top/gtfsfbknnh.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtuhqypgft.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gotoacloud.top/gtpuusiacs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.snrcjt.cn/gttbrgtfxt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtbridnbqf.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtqtbgnikx.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtrylgvxaa.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gtkjsqkhju.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtdhkqbagh.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gthmnmhzxv.html

Java: private String name;
来源：http://hz.yj202588.top/gtbpsyimni.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gtypvncpqq.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtabusmqcp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtplipmmwu.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gtyjgpxbcw.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtbzfrxvot.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtweyjfinj.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtvufbghjb.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtxyvphian.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gttldlpguy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtfxfbikse.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtdpxmauyb.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gtzzolqwte.html

[G05] 继承
来源：http://hz.xylfe.cn/gtlumlxaut.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtjbgvqcea.html

PHP:  class Admin extends User {}
来源：http://hz.52xcode.cn/gtaiylwuao.html

JS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtkqgxnzal.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtmqsykdvg.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtufvondln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtoitgbtms.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtmxobqkon.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtmiijwurg.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gthvkqqquj.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtzhhzbzmf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtovpnipxm.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtufejsxwt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtkqpytmet.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtkfqzvgrp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtgvygadlq.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtuvdzialt.html

C#:   public override string Greet() => "admin";
来源：http://hz.birdmap.top/gtzenfehnl.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtmhyevvvp.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtaheumlug.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gtqfazvklp.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtkvgouwut.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtkosoyqlf.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtstpnrdgg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtcerhfsyk.html

Ruby: super
来源：http://hz.ydzc1.top/gtmidodlar.html

C#:   base.Greet();
来源：http://hz.nanxuanxn.top/gtexxtlawz.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtdnxbkpwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gogol.net.cn/gtoeogqpbi.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtzsywtwjn.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtxuvmryfv.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtqhqscqit.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtiqpprtix.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtrnlszkea.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtldnrqsvf.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtccfjshta.html

[G09] 接口 / 抽象类
来源：http://hz.cdnleiting.top/gtqpsmqhol.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtmphodhcm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtlkygcrhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gtguqylbuc.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtervvzvmj.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258888.top/gtgktlouov.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtmdmgbmtd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtpgyjrxou.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtcjitxttx.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtnxnuzewo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtiubqdinx.html

PHP:  public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtbmnrovwu.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtrqlarzzd.html

TS:   public / protected / private
来源：http://hz.gaohongyu789.top/gtydytcvzl.html

Java: public / protected / private / 默认包级
来源：http://hz.ppjwa.cn/gtdcrlbozd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtpkkwuzmq.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtsjvgarbo.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtyctddjkm.html

[G11] getter / setter
来源：http://hz.tianlin.xyz/gtvjnaajex.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtlhndbzqz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hammf.cn/gtshxngxdx.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtxjchlrzg.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtssajcudr.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtpdxtfseg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtsbouugnn.html

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtrpozvfke.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtbnoltzjd.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtolyfloic.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtxfbvwvkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtvprncgit.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtmnlekekn.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtphgabixy.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtifxjqbiu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtifcouvgm.html

Ruby: def to_s; @name; end
来源：http://hz.yuxming.cn/gtjfloqjqd.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtzdzidggd.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtwgwwotrj.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gticwbkkzz.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtzctfkzxd.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtlthlndse.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtddqkcusw.html

Java: u instanceof User
来源：http://hz.sxryk.cn/gtkcdcthbr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtnpxionpr.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtuhuusmpj.html

C#:   u is User
来源：http://hz.yj20258.top/gtpfktmfkd.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtgmiyyooq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gthhmvwkqr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gthcctptgk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtzvdmwcxf.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtkonoyabk.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtqqpfyrdo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtzzntdira.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtoqkxlsyv.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtwvgxsoja.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtoijowkuv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gttbibpscx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtjscrjrki.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtceecbvsw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtareljnha.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtaepermzg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gotoacloud.top/gtefewgwlu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenzaomai.com/gtfuyxwcbl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtuctubdre.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtsnekvwyq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.vqdsnc.cn/gtfoszzymm.html

PHP:  get_object_vars($obj);
来源：http://hz.hnqzz.top/gtnvzwclgt.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtrxfafums.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtzimyelen.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtiketrioq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gtpaxhjhgn.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gthlohbbob.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtykwfgdqq.html

================================================================================
来源：http://hz.dashuyun.cn/gtysclqbwq.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtmgfkxwbj.html

================================================================================
来源：http://hz.snrcjt.cn/gtcagdtgky.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtnvpiasus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtxdijqvpt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtvkochwlq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtdmldjnxs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtehtxjbxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtgihznvxm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jlsjyb.cn/gtausgyjti.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtqihavbdo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtfzuavkbf.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gttdsgmsfj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtetnoksap.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtpwqhqunk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtdymytuze.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtefsjayuu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtbyimydqm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtvxkcgyvs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.quarkkingdee.top/gtlxlghdjk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtdqwwtyer.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtddnsvlpu.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtfnmkyjim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtkuemdxxp.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtvrzrzxpe.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtttniurbe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtgokvnuss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jiagoushi.top/gtskvuzajm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtfuopadqn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtenzflpva.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtcorokwzh.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtfopwxsnu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtjxsntzyb.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gteiyiunzx.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtftdpqqom.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtwewwyblx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtbxhibesn.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gtkesghmhm.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtoiqacidx.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtrhgtkwty.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtbcskaxfk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtogzebdju.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtdfxmxppg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtqelrstqy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtbzoxlglz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtutpaoujk.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuxming.cn/gtgwboxhni.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gttoszgtwc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtmqlxmfps.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtoipmdyfb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtroefaeek.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtugdvoyca.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtpphjagdw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtwpimxcaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtcyyvgvbh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtjgerhkow.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtrlysiuvt.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtiolllreo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtxuxifynf.html

PHP:  assert($x > 0);
来源：http://hz.zhongyouzk.top/gtymzglofc.html

JS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtnkpofqvl.html


<!-- 参考信息 -->