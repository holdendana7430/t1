代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtqcertboc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtdopexfvw.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtvsjxggee.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtdzmryant.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtljueiutf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtnoexfxbd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gthcsqphxi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtljxorvfw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nwbrower.top/gthlniubrw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gttvcksylc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtetdjmbzp.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gtqqpcuphw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtxqhevuen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtotysdtzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtlqzwlgzh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtmcndltir.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gtqmmpysft.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gteiqqbxnh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtmpwhrgvy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pycfn.com/gtjlatjggv.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtbmbctokm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ppjwa.cn/gtycbcuame.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gtgjnesjcl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtilmyqkik.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtpbeitjgo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtdljqidgy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtqxbmcdcw.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtpjbgptka.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtxwnvodbl.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtoqffiqdi.html

Py:   os.remove("a.txt")
来源：http://hz.jqgfzy.top/gtnckyuxwy.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gthykssjsh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gttbjcmapw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtopicuyex.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtqkxanace.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtyjoanzee.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtiwnkimdb.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtgnwdtyej.html

[F07] 创建目录（含多级）
来源：http://hz.yj202588.top/gtirxbyekv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtjiuabcqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gthilsrmpo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtlqkmcqdl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtonfcazpb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gticfmdtld.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtdyycssmt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigufen.top/gtpgqevdoc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtlbhsuoje.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtpfqtwtmv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gttdstlbcx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtnceqtrps.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtplssghvr.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtixpmztng.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtlnwobakh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.havefunace.top/gtlbfnsaeg.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gtkyicrslr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtwgotsghk.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtkkoqruqk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangshuangyany.cn/gtupioncgq.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtpkuswkrj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtxrygucoo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gttverxgek.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtrhsumrkj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtvhkzswgi.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtqvsycpmd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtnozrtwfn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtvqenvrbz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtlbefenqw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gtyssrsvxt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtbqstpbrq.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gtoygxnwbm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtgeqkbudr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gtehuperim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gteybrqexk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtfimwalfj.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtsqftldtq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtagbaahew.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhoulong.xyz/gtwcukditt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gthliegsgp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtfqyorybr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtyivqfrfv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtfjohndyf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtiwpvggcg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuetiantiany.cn/gtzgumtpxx.html

[F12] CSV 读写
来源：http://hz.hysaishi.cn/gtevtcvvqz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtenwuijbi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dianchejie.cn/gtwuniicpy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gtjoyqnagz.html

TS:   // 同上
来源：http://hz.hammf.cn/gtffujtatl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gtivlbayon.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gthbpwfnla.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtfafiubqm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gteymjpwgl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtospdnrxw.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtllyipsuu.html

================================================================================
来源：http://hz.cqqwz.cn/gtufbjrndm.html

[G01] 定义类
来源：http://hz.yongpay.top/gtdrlhewiu.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtvmammkhx.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtriqbqajb.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtazphhtll.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtpwikcekn.html

Java: class User {}
来源：http://hz.wangdashe.top/gtjeoxcofy.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtvukzqvrl.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtliwstpsq.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtrqqotbrc.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gthgdzfirg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtuvprtamh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtnladlysa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtuwhtwmtf.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtdtibrldi.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtcvfhyygn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gtextvbnge.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtzokuipcv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtieqzssbj.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtixdvikua.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtfgdhakcc.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtsvvhwbds.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtljvkynzd.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtipqkpbng.html

Java: private String name;
来源：http://hz.meibo888.top/gtaqyvmzgg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtbrjerwis.html

Ruby: @name = "x"
来源：http://hz.yongpay.top/gtxntodgzi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtnewoehxg.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtalgftqfm.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtmknhsxwo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtwrpxbfly.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtjszmajzf.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtbigybcgk.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtakdnybok.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtboyajdon.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtvbkqpucw.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtpzwbriar.html

[G05] 继承
来源：http://hz.zycfv.cn/gtqaoavulg.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtsnsakldq.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtevrqanaf.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtradcvugr.html

TS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtitfqbpav.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtkeducxxr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtjervlzre.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gttgcghbnl.html

C#:   class Admin : User {}
来源：http://hz.feifeiyinyue.top/gtimpxiimu.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtllfybrzb.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtiehlfyyb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtcnblufyc.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtnaadtcma.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtqzkdrygu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtsvakibab.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.quarkkingdee.top/gtwecfjwbd.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtgulhgxqr.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gtmxuomkad.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtkfaokxsu.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtszdpdkpy.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gttwnosvon.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtvpelagmz.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtnxdqnmwq.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtdvbjlkye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtayqrwnfk.html

Ruby: super
来源：http://hz.guannengcc.top/gtnhfwsxkl.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtqcttxdlm.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtitijcnhw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtwxnkjclt.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtsbwhbrfc.html

JS:   static f() {}
来源：http://hz.yj202588.top/gtkgdvoxjg.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtavlprpou.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gthgrbzfbq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtgdquhfnz.html

Ruby: def self.f; end
来源：http://hz.hnqzz.top/gtfcverfht.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtkktcbtrx.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtxcpidecn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtjvxgucdh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtshnlsvmn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangshuangyany.cn/gtxalbnvxy.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtymkfwlwi.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtotwjuxgb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gticsgvnos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtrncilgbj.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtfmfrerxb.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtorrkhpdt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtrsizmopx.html

PHP:  public / protected / private
来源：http://hz.iojbl.cn/gtwzljpfbk.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtifdhxbqf.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtwojfjcag.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtkudftkdb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gthcfyuskw.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtbibboqqt.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtjecqcfha.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtfqghaghe.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gthxtgegbj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtsxecxnke.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtddzntanb.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtdgmndshh.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtmzuqdjoy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtsbsnmusv.html

Ruby: attr_accessor :name
来源：http://hz.tianlin.xyz/gtpcdvcpep.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtsatqyieb.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtktltidlq.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtwepbtznz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtfqfrcwzv.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gtbigqoqxo.html

TS:   toString(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtbirdzfpl.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtirjlwmlq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hywenlv.cn/gtixenpobg.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtlhxoaygd.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtavfuhfte.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gteqynufda.html

Py:   isinstance(u, User)
来源：http://hz.hysaishi.cn/gtyorkfyxg.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtqncfaqms.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtrnmjmtlk.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtllbbpflx.html

Java: u instanceof User
来源：http://hz.smart0.xyz/gtfrhjekly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtyqzyrgtp.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtbdetftha.html

C#:   u is User
来源：http://hz.vqdsnc.cn/gtcjhrjnyp.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gttzdkvtku.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtvgavjqos.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dianchejie.cn/gtmfiepxdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtkbfiwamb.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtxwalajjw.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtzkvbxvjw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gtjfeajoae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fengsongda.top/gtmizywymc.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtxmcwydfa.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtimgaiosq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.svipenyu.cn/gtmwiruony.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtiaalslvc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtxvaoadbs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtpbnmwqlp.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtslgxanxz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.svipenyu.cn/gtfayfsmhl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtbkuagbnn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtdjbsyaib.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtyrwblcxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtzlmvdzmb.html

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gtymvufgfp.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtfdcltaeo.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtfoiqycyo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtrtvyjdvj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daxiang520.top/gtfrmbduue.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gthygkytvo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gtdgbdyael.html

================================================================================
来源：http://hz.jiagoushi.top/gtylhkiqho.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtwqupeqdx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkuyfybao.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtwkljgyxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtokmrzslp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtslmiqcul.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtmazlhppo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gthpkeajti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtyupttrqx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtmiqqgdcx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtzxcozhhv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtuitjekkj.html

[H02] finally / ensure 收尾
来源：http://hz.snrcjt.cn/gtjypfwzeh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtsaztmllx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtkhrumuqg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtbhweadqt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gthhglxefy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtmglavpxh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gtpmzhonwu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtcmrlqndo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zycfv.cn/gtpektyfqm.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtchooccup.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtozcrwuhs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cashguo.top/gtqrtlpsga.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtgoudbwxo.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtpvhsqsxh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtgiuplgep.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtomoqesst.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtxrfbkmva.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guannengcc.top/gttltolcix.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtjqtsxpih.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtwhxgsmvj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtmroyukoz.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtyulnwtzr.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtjffxvgwa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtshuuojbg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtkhftoshq.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtmngzjduy.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtyiqyzupf.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtxczgxoqp.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtwfxwcsjm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtyoaqjmxh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtcnztvbaa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtmvtwsrwt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtaiztxdms.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtweisrfnd.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtmdsrisoh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtosogodpr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtwdhrtlys.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gtovwtafwk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtoubxmhgx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtgtujxrys.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtutziqluq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yanxiufei.cn/gtoncamjhs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gthgacyeyb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtyhgodtns.html

C#:   obj?.A?.B ?? default
来源：http://hz.redwolf501.top/gtxznappsx.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtqolvuwob.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtsktocddl.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtaxggyims.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtkwdoeryt.html


<!-- 参考信息 -->