代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtwbuvdrsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtgmdsaodj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtngsjcqjp.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtjztvyffo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtmrmbvogg.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtpacbxdwu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtjhkkupqk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtrxuaylej.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtmvvplqig.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtunsrxewt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtzfzirzhf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gthwhciiyl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtmwpxetpq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gtaphueogw.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtydkaqxau.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtonljbdul.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtonwutetg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtjzxjcphx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtywurgzrq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtgbbytmqu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtvvrqfiii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.iojbl.cn/gtjjdpnxrr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gthjkrnmjv.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtvkomoecg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cucudq.cn/gtfbloqkqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtdickcjud.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtqnngtbdx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtyvbfeabq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtkjpowqph.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.meibo888.top/gtmltisiah.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenlongwang.top/gtqprgdeml.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtbnutkygy.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtacosvzuu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gthfvypujo.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtzxirudnf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtbycooaxg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtdqymfjcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtltxeaqia.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pycfn.com/gtwxijgaqu.html

Ruby: File.exist?("a.txt")
来源：http://hz.kuanghao11.cn/gtczzpefdr.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtzkrqucad.html

[F06] 删除文件
来源：http://hz.zhoulong.xyz/gtpaauiozk.html

Py:   os.remove("a.txt")
来源：http://hz.fengsongda.top/gtzwiiehrw.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtjbtcbeuz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gternkejts.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtlbriebvh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtnipflzsg.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtnsrngkmz.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258888.top/gtsixcjpuj.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtwbsnqudh.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtfblsnazt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtkyrisyvi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gtmgjbclfw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtdrgwlpwx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtjtmumszy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtbccnspbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtxemoljfz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtoinklvka.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gtjwbykfdy.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtongickjt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gtejyvhbnc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtbvxtuzel.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtecmgvoht.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtozgggbys.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtihmhaulm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtxbnvskoa.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtvgdinwqn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtgppkjern.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtmnrnafql.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhengqikj.top/gtjdhfpymp.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gtmwjlcaci.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtpkbxjeep.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gttfjggyww.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtiwjkulny.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtarbaatss.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtpbuzeofh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhoulong.xyz/gtjehlbhka.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gttmktmums.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtmmomobov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hysaishi.cn/gtfvdxxkyk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtyefdeksk.html

TS:   path.extname("a.txt")
来源：http://hz.jinghuilouyu.cn/gtyxxsyhzy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yvedp.cn/gtjpogtrge.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtsndsopst.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtzmoeyzcz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtltcaocar.html

[F11] 复制与移动文件
来源：http://hz.vqdsnc.cn/gtinilysyb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtkahhragd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhengqikj.top/gtscqkumng.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtvevqerep.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtefgpzmbp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhixingplan.top/gtgznemnlb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtnoqmumxv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtmbatfcga.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.redwolf501.top/gtqqcjrfxz.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtssnxdhmu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gotoacloud.top/gtwmowjrhe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtbgbxoqqs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtzzeeqdol.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtxcglwbxx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtyymhhlra.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtewmzstcf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtkofpxnpg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtvmutoyvr.html

================================================================================
来源：http://hz.vqdsnc.cn/gtktvdxuqr.html

G. 面向对象
来源：http://hz.wangdashe.top/gtdsalchbn.html

================================================================================
来源：http://hz.cheryme.top/gtapofnqqc.html

[G01] 定义类
来源：http://hz.cdnleiting.top/gtqbansqye.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gtmbqxvrka.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gtnucletck.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtddinejtx.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtonwmupdp.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtskbfucfi.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtknzlymou.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtgjpmbbap.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtltnjfizh.html

[G02] 构造函数
来源：http://hz.yj20258.top/gtsakmpcaq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtaplfhjis.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gttkdetdei.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtrlzujuny.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtrjsgndee.html

Java: User(String name) { this.name = name; }
来源：http://hz.tanke756.top/gtpiprgdcx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.quarkkingdee.top/gtggdotskn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtkyogirgp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtsrxgyyoj.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtqlsfdrna.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtjijbmaix.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtahtbpuos.html

JS:   this.name = "x";
来源：http://hz.dianchejie.cn/gtbauswegi.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtbhdleopp.html

Java: private String name;
来源：http://hz.52xcode.cn/gtglypozft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gttsddaqbi.html

Ruby: @name = "x"
来源：http://hz.9152youxi.cn/gtvkngbsxt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhixingplan.top/gttiyrivbl.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtvclolcsn.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtvcbupvfl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtoznphmfp.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtqanehlyn.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtzvvkdujq.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtjzxspsli.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj202588.top/gtzmynigdw.html

Ruby: def greet; @name; end
来源：http://hz.kuanghao11.cn/gtftmgjfde.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtbopjbtac.html

[G05] 继承
来源：http://hz.jqgufenzy.top/gtihwqyxtp.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtrbmkiriz.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtmopengsc.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtudcqbivr.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtsrjidlyk.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtaogeeadw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtiedldmbr.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtzirhtqme.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtmdmnexpz.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtcjttacjv.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtgtjvyvgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtzcvgbmrd.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtmjdnrfgm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtbuytxbeh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtvprzassf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtlbwbydie.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gttpyqxoge.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtnhwmsbur.html

[G07] 调用父类方法
来源：http://hz.aizwys.cn/gtguvjwetn.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtguroynqy.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtxvgxbrkn.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtuwnpguli.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtpmsnkrik.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtvepnfbpv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gtntozukrs.html

Ruby: super
来源：http://hz.guowangkeji.top/gthskdrsog.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtzewapgdu.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gthvwwxomi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinyuanbaomall.cn/gtpvookkpa.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtzafryycy.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtuwrdivsn.html

TS:   static f(): void {}
来源：http://hz.guannengcc.top/gtroxlrquw.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtpmypawkt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtsttoeqhm.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtysergxea.html

C#:   public static void F() {}
来源：http://hz.jinghuilouyu.cn/gtplvmruwc.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtsjrlrgjv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hysaishi.cn/gtolhdjkwc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gthkmcbxts.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtfsctqtro.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gteidbdtug.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtubjddcla.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtulzrblmr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtyxttjufp.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtnhdxfdcc.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtlxwwyvui.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtmsytwiwe.html

PHP:  public / protected / private
来源：http://hz.zhixingplan.top/gtylcbxbnb.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtklxaefpn.html

TS:   public / protected / private
来源：http://hz.xziqi.cn/gtqjxsnblz.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtuggonnhs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtkjesbauy.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gteilwapxu.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtxlmnfdyp.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtnzayhdre.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gteviypbcx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtkfszdihg.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtpgqjvpah.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxuanxn.top/gttgyseggf.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtpqgyftqu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhixingplan.top/gtkazojvhb.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gthvprrwkx.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtfofumykv.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtckovfjeo.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtcinruqzt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtsmrwgsui.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtsvkjgbly.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtgihdaysw.html

Java: @Override public String toString() { return name; }
来源：http://hz.tanke756.top/gtbhsehqsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtrangaleu.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtldxsemqf.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtpelqmvba.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtprllrueb.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtvxnovael.html

PHP:  $u instanceof User
来源：http://hz.nanxinkj.top/gtjpfjeamj.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtwureltmz.html

TS:   u instanceof User
来源：http://hz.nanxinkj.top/gttzenaics.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtfgcmkrro.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gttjknbqno.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtkvqzhalz.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtjdkmnwot.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtdyaniplz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtdqgxnekz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtbmuzbdix.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gtmegyhlra.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gthalyendl.html

Java: record User(String name, int age) {}
来源：http://hz.xuanzx.com/gthjpiwrxp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtfctbeewt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtsntsvqut.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangkeji.top/gtotpzzvlk.html

[G15] 枚举
来源：http://hz.yongpay.top/gtlhkxbkbq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xingfuxueyuan.xyz/gtupccrhjv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtixrrvzri.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cheryme.top/gtvnsbwaff.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtmvqkbeoy.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtgkvnfjsd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtzoeurqcw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jiagoushi.top/gtnyvfiqsj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtvkuvgovr.html

[G16] 对象转数组 / 字典
来源：http://hz.aibaodan.cn/gtlombvtyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtesmkwkkn.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtogarycmp.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtlxvolrab.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtkfgdhybg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtivfwdkuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gttpbudbnm.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtqgesjjgc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtruuowhbt.html

================================================================================
来源：http://hz.hfpthk.cn/gtqagkoyem.html

H. 异常与错误处理
来源：http://hz.yj20258888.top/gtgyosenvs.html

================================================================================
来源：http://hz.jqgfzy.top/gtauxmffye.html

[H01] try / catch 基础
来源：http://hz.chenjidiqi.icu/gtahvkxmzi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtzeijcdzc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtvwohaslo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtifvewdbi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtngkuzoyi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtsgsggqls.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnxiangtu.top/gtvphtbtle.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtbprjhunc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtwxpdorpj.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtzeslvixy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtnepbmvpu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtppyuuysf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtmhtgktmx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtwypfoghi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtjmsltrzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shangyingyoupin.top/gtiehmfugp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtwjhexnpm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtaocuwrym.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtyggqxgle.html

Py:   raise ValueError("错误信息")
来源：http://hz.yanxiufei.cn/gtfaoobzkp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtumkmerkh.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtvijjbrju.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtbenogrwb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtlmfihwyu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhijiandao.cn/gttyqffzic.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtlmwnhows.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtgbczkxvy.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtqpwzxnvq.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtuqheznyw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtgncloumi.html

JS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtabefqclk.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtidokdkmj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtnvlmsjgt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtmiwlxiih.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gtcswbwohl.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtogjzpeez.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtenaugxve.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gthqdjqbql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtlwotqmyg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtufmsngxc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtjhlxwgym.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtqkhrkkng.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtknkwkytt.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gtsvotengz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtskqbjier.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtdumbcbag.html


<!-- 参考信息 -->