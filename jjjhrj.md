代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtwaggzbye.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtklgclrdd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydjk.org.cn/gtfdmftypt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtjzyxwnxd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gticbnfbsm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtdnhtlwko.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtveyiksch.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtfhzvyzji.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gttxxembvm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtogizltvs.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtfwtgxxqp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtmqfoexwa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtczyhdzis.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtaaflpvow.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtrgfllbew.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtvpkycmsh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtdfrzbhvt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.52xcode.cn/gtnuwgjkvs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtmjjgmuor.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gttifbmvcx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtgpvfoker.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ywan-chungtsiang.top/gtabroseox.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtkfwdlmrn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtdiymlsvt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.0kj1m.cn/gtzhpwlakp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtqvaxasqv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shzxlz.cn/gtnkllhngl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtsnvaqxlx.html

[F05] 判断文件或目录是否存在
来源：http://hz.guannengcc.top/gtyccclezq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtplfqbsdb.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtrzjchxwd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtvqveqyeq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtjzpngjls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtsqfxwmcn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtpkvlndyj.html

Ruby: File.exist?("a.txt")
来源：http://hz.pycfn.com/gtpfudblot.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtghgqfeux.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtaqnsxojc.html

Py:   os.remove("a.txt")
来源：http://hz.tian-w.cn/gtjbjbmdlf.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtnxqzjuda.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtcjkagejv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtvltgzbko.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtrxrbuigf.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtalzekgfb.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtnwfpzusi.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtpltobtks.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtkdkisaew.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtgsuuqtre.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtwwjpfude.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gthxgvnvpc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtmoorroca.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtemeuttzp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtdhtqqkoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtfmecsxst.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtvmisjyse.html

[F08] 遍历目录
来源：http://hz.ehwqpu.com/gtfkiegfio.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zycfv.cn/gtbebyuipu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtsmmabjcr.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtlsikduaw.html

TS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtiunqmecr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtwmuygiwo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtdqfglcxr.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtpqtcawfr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gthduzhqlc.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtddnwxblz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtcqxtjgxm.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtwjvcpqht.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtcraizuxs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtejdrkkyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtzzyjdaku.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtavcenqtd.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtqzofnjve.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtvhanmugm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gthfmfidgb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtnmizerlk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gttfungbgq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtxcfpecpl.html

TS:   path.extname("a.txt")
来源：http://hz.jqgfzy.top/gtpzhhabnz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yongpay.top/gtsssbgspy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gtouzxwzkl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtuxabnxud.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtggojtkou.html

[F11] 复制与移动文件
来源：http://hz.jqgfzy.top/gtgsswyptk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtzhhbhqzn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtltopvsvi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtewkhopis.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtsnnoahsd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtbiqocuyc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ywan-chungtsiang.top/gtzrnraffx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtjwnbqtin.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gtnejqioax.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gthpkjwprm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtlirvnymb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtggpbsppv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cashguo.top/gtwgbhpewx.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtfcwgboow.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gthrzqjcsv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtqcrylnzf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtxgvjtayj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtrfugdqaw.html

================================================================================
来源：http://hz.tianlin.xyz/gtfjklnbxo.html

G. 面向对象
来源：http://hz.jqgufenzy.top/gttyuvopgm.html

================================================================================
来源：http://hz.cheryme.top/gtlvdvohdg.html

[G01] 定义类
来源：http://hz.sweek.top/gtcnitvnop.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtqdcnqipv.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtqsoffyka.html

JS:   class User {}
来源：http://hz.yj20258888.top/gtetdmgpys.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtvxauwkdp.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtgywgcquc.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtchmhnvlj.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtbluewpby.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtbewqcwrl.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtrjouncsh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ywan-chungtsiang.top/gtnhunhhuk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtxwkaozrv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtwruokfew.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtbxcqbsjw.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gtiqxdmony.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtgtcfirve.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtippfzqdb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtiutddvor.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtvfxzbzyl.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtofysxlio.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtdupcgfxk.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtzpfctkfb.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gttwjdixwg.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtccitfaxz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sufxvd.cn/gtobajdkiq.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtapnhppdg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtejweybsm.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gtuzhykhet.html

Py:   def greet(self): return self.name
来源：http://hz.aizwys.cn/gtqnnkmyva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtydynmsfg.html

JS:   greet() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtxrfdvyse.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtsqiyiqhm.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtohujrold.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtadanevap.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtrqkujwag.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtalzzpsjs.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtpskvwkib.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtgrlrmduw.html

PHP:  class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtmsygbehs.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gttjvpbuop.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtfpjikrhj.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtzjfocwwd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtgaojgrgf.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gterldzfrn.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtrqxkmvcq.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtoxtgrnkz.html

Py:   def greet(self): return "admin"
来源：http://hz.ydzc1.top/gteczsekja.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gthmtnrrbv.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtoiojdnmn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtfizfqokd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtvzbdlevu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yonumen.top/gttzrnijlp.html

Ruby: def greet; "admin"; end
来源：http://hz.hongshengwenyu.top/gtbuytkwsq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gtrzicmesd.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtrtlwxzsy.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gthoqjmyhg.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtjjdladgq.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtruzdchwl.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtrkwbfynn.html

Java: super.greet();
来源：http://hz.316326.xyz/gthoqguhfi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtangghpyx.html

Ruby: super
来源：http://hz.316326.xyz/gthwlmxenq.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtqljdveix.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtylwmpvel.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtdfsibyqn.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtbzgbswqq.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtwmmhdvrk.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtsorxiizo.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtxuczxfrx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtnoefzkkt.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtvtrnzquv.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtzjktgtyc.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtqfwpylyc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtvnanmway.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtgkkvxheg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gtvbkumvbm.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtcirpdcpv.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtvqudlafz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtdytkdmom.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtwvomdfzu.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtyaacmpyx.html

[G10] 访问控制
来源：http://hz.feifeiyinyue.top/gtphsxovbj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtzkqxkphs.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtrwnviool.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gtxygfjglp.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtncbnkxqs.html

Java: public / protected / private / 默认包级
来源：http://hz.sweek.top/gtwrpytmwa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtivbnmqod.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtcrchcjam.html

C#:   public / protected / private / internal
来源：http://hz.ywan-chungtsiang.top/gtyrizatnv.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtrltclewn.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtcfvrlnhs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtybggcndu.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtbzepyiih.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtvcyaperq.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtgpkfgxmc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtscmkmkpv.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gthxtltthu.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtyhualygy.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gthmlgrzzg.html

Py:   def __str__(self): return self.name
来源：http://hz.guannengcc.top/gtfexpmasi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtlzqqzehq.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gttanqrsdd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtvhgrahcu.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtiwiddynk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gthwgoryau.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gtpwchxmys.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtsxpxyhci.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtqvognblw.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtizlddudm.html

PHP:  $u instanceof User
来源：http://hz.9152youxi.cn/gtdxfafqmm.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtlaftdxbs.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gtjszizowd.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtuzgpbbkk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtljmmktpx.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtpfayddds.html

C#:   u is User
来源：http://hz.daria6918.cn/gtrijkvpxc.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtwrfgchoq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtndzawptn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhiwuduotai.top/gtiajnpqxz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hongshengwenyu.top/gtboaupmpb.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtuuyvvzib.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtrsnbmdjh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dianchejie.cn/gtokmcqlhm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.0kj1m.cn/gtazetkgqi.html

C#:   record User(string Name, int Age);
来源：http://hz.andypj.xyz/gtianvqzwr.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtzlicjmlr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtoroyrnlv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yueranfly.top/gthqybgihd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtbatpxlgf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtdxzutcpb.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtpajwpqhp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtrgpxrndr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtmzacttbr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gthmgcxjtc.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtmsnggexc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtgqerskfx.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtecuaqmok.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtijpolupe.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtjjshsfig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhixingplan.top/gtlrxdsndt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtrxfkxngd.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtcrvbxvaq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtfsrkdpah.html

================================================================================
来源：http://hz.xinyue.icu/gtosstuwnx.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gttlxefqaj.html

================================================================================
来源：http://hz.sweek.top/gtwhqgexst.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtsdvhcluj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtwumsyphg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtjtndcrby.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtaeryssxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtzuamddgm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gteoxscuth.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtzeoapife.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtyscmbkfe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtsxvmcobv.html

[H02] finally / ensure 收尾
来源：http://hz.cdnleiting.top/gtkjrydopy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtuflmmfoj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtrtntckpc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtqckfktvg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtmirfvcud.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtjgbntbfn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtgpykqxgb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtzcybbzxr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhongyouzk.top/gtkjjiyini.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtwkvfwhrb.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtltyejuio.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtnbpvqglw.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtxbzlgpou.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtzaxmqjqg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtnznxpwdr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtqidpqmgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gtqvikufuj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtzgndzabt.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtgknesipm.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtojsoajdl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtvvhkqkaj.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gteqltwads.html

TS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtubnizozj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtnkxgtrdb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtvclhnvit.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtleaxkzyn.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtvviosvrk.html

[H05] 捕获特定类型
来源：http://hz.svipenyu.cn/gtjyxuqhwo.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gthqotqfcf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xylfe.cn/gthhnetoze.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtjfrlzvyg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtpucclnxf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtyyrtweoo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtfhefrufi.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtgqjkzskw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtqpvfhbpg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtureocdpo.html

Py:   value = d.get("k") or default
来源：http://hz.52xcode.cn/gtnjrvblwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtlzcelkcx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtvweboocu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtunnfgufn.html


<!-- 参考信息 -->