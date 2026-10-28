代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtriazfzhx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtaimktshh.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtcslbpzwp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqnbinqrq.html

[F01] 读取整个文件
来源：http://hz.yj20258.top/gtuoukhgmu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtovhwqupz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtcxhkuwnt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gtfsffeotx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtfvirwlpw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gteqgizqgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtjfdtbqqv.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtferwgfdz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtgsualhqg.html

[F02] 逐行读取文件
来源：http://hz.havefunace.top/gtktadzstv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtcoqwzbmm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258888.top/gtxhmxzgto.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtarzxdbtb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtftuxtukg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtgrbrjvqd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xziqi.cn/gtuvjicaev.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtoosvocdk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhengqikj.top/gtoqmfmggm.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtitacnzvf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtorwvedsu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtfrdypnbp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtjwdujvvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtzdmqzxzo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtokhlgdbb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtjxjdcyib.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhaomingkeji.xyz/gtfifjijyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtwereklwc.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtyyoqvmmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gogol.net.cn/gtvbxulkxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtvvfpkiaw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dianchejie.cn/gttxrhydfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtewkohgel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtrdgztxff.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtcdgemdfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtncdhelgt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shuidangran.top/gtylwnrule.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtituszrxt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jianghu66.top/gttcmhzagx.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gtbbxzwvex.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtahujxwtc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtqiglrtls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtnvikotke.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guowangkeji.top/gtkzvxbraz.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtxkbfamcn.html

C#:   File.Exists("a.txt")
来源：http://hz.nwbrower.top/gtbpnbkcvp.html

[F06] 删除文件
来源：http://hz.shangyingyoupin.top/gtuuehfqwp.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtdfjejged.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtlabvfmyo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtoizrrbch.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtikhbipxb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtqkypvufz.html

Go:   os.Remove("a.txt")
来源：http://hz.gotoacloud.top/gtuvpnpowo.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtkknmznsq.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtgxfadjsa.html

[F07] 创建目录（含多级）
来源：http://hz.yj202588.top/gtrzgbwcys.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtfsrgcmcj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gttjkrxgxg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gterokxyqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtgigjdunx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtujuhmotr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtarimvmyu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtfkvodfft.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtouhohxtj.html

[F08] 遍历目录
来源：http://hz.guannengcc.top/gtxxyolpbw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtminpcyxq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtekovmhip.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtsrofjwop.html

TS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtudffstux.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtwxrynarq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hammf.cn/gthhtneqfx.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtupnscykv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtlevuffyf.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtblpgykpf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtbvdhsyqd.html

PHP:  filesize("a.txt");
来源：http://hz.kuanghao11.cn/gtelmdvwnj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtnbezromu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtirzyalya.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtbknmycxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtdxnwhwfa.html

Ruby: File.size("a.txt")
来源：http://hz.zhixingplan.top/gtybggiapb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtjnhsthll.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtacxqnltq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtnpewccyq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtmqqxdlkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtgknyuttu.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtaqgyhfeg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtttkweqph.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtsagccalh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtqpdpmdhx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtoohzwbrx.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtsroluxpx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtzfuytbuf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gtecfqdmks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtcmcsqnwm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gttjjxmldi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.havefunace.top/gtfcpsjoxx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtknhhrumv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtbjunmpxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtjheeaznk.html

[F12] CSV 读写
来源：http://hz.xinyue.icu/gtoquappco.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtcnxmsmck.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtfwkwffls.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtscyxbpsi.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtefcrcvhr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gthvqmzwrs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cashguo.top/gtzfrolilq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pycfn.com/gtzmrxvhab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtnzpywcev.html

================================================================================
来源：http://hz.0kj1m.cn/gtaktojjbb.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtmyhduhes.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdcihmqxp.html

[G01] 定义类
来源：http://hz.shanyushiyangtech.top/gtzfeqdiwe.html

Py:   class User: pass
来源：http://hz.vqdsnc.cn/gtmsqugmdz.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtvkhcguns.html

JS:   class User {}
来源：http://hz.yonumen.top/gtqwthhstz.html

TS:   class User { name: string = ""; }
来源：http://hz.ehwqpu.com/gtacnhbsaa.html

Java: class User {}
来源：http://hz.ybcxt.top/gttakwkqxg.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtxrchgssb.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtzhrvkuen.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtgzzhwjmh.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtshavqyjs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtnsvoaftx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtccxmxzom.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtaxfytbns.html

TS:   constructor(public name: string) {}
来源：http://hz.xinyue.icu/gtliefblrb.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtprqvihxx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtqrwwcfzs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cheryme.top/gttmbjjyiw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.vqdsnc.cn/gtceeyxvol.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtdbenweeo.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtqpcwzbtm.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gttwbndmnt.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtljtebpmo.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtivuhbhav.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtbiwfdnqo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtihkgqfjk.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtgecjnboy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tian-w.cn/gtydoypfkm.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtsmatpsnx.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtyogfkhsi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtyioqsfjd.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtzbzbjzly.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtnfzfrstc.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtjoowtyry.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gtywdkahcq.html

Ruby: def greet; @name; end
来源：http://hz.ybcxt.top/gtiviijepf.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtyilnfcra.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtrwmheujh.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gttwzagnar.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtqgnzsxab.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtvguagzft.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtaomavvok.html

Java: class Admin extends User {}
来源：http://hz.yongpay.top/gtsbhjxrsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtooviansr.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtqdgpajzn.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtgckohoth.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtfwuijpam.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gthvptbzbv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtgnastdmx.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtptefitqq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtuphghsae.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtnqdbksjv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtunrxudop.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gttmvubnvu.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtlqhdicns.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtgoekpozc.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtlyuvqpms.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtxticlqji.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtqzdxktgs.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtrcwyphfv.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtijprtzxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtkzufpjvo.html

Ruby: super
来源：http://hz.shzxlz.cn/gtxggzjobn.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtnpdfevbj.html

[G08] 静态方法与属性
来源：http://hz.svipenyu.cn/gtlkbtjksh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtockgqath.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtukkjnvoc.html

JS:   static f() {}
来源：http://hz.gogol.net.cn/gtqjtbzvkb.html

TS:   static f(): void {}
来源：http://hz.ppjwa.cn/gthypdhhof.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gtscuydzjo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtuyqfhogi.html

Ruby: def self.f; end
来源：http://hz.jinqigfzy.top/gteltiuwod.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtgjorrrha.html

[G09] 接口 / 抽象类
来源：http://hz.tanke756.top/gtxdentpox.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtneiaxwot.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtdvapktqd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtfnxmchjf.html

TS:   interface Shape { area(): number; }
来源：http://hz.daria6918.cn/gtxndcnyjh.html

Java: interface Shape { double area(); }
来源：http://hz.havefunace.top/gtaqcvyjwz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtmgkbhctj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dianchejie.cn/gttipjnbpm.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtbyiwckng.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtmzlhfwmt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuanzhike.top/gtuudvxuny.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtprxrgvaf.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gthhejwchc.html

TS:   public / protected / private
来源：http://hz.sysykeji.top/gtrpxnbfwh.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtygklclpv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtoazbpkzm.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtgvzaoydi.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtvejpypuc.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtywgadhvw.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtjkfkdmhk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtnctyvuaj.html

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtlhdpqqgc.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigufen.top/gteaterqxu.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtoiznqann.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtmhchgdxt.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtxvvqzgxy.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtmfjtwsaa.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtaklhvgte.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtrqpiizsz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtwlocfspk.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtoftvcegg.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtgpqccrer.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtopbivoqe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtobeaprle.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtlcjykxpa.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtvegjopap.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtkgyarbhg.html

Py:   isinstance(u, User)
来源：http://hz.0kj1m.cn/gtvchgypdj.html

PHP:  $u instanceof User
来源：http://hz.pycfn.com/gtlsyjzyqd.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtlfftumss.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtaidnqzwi.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtpbzgjzzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtoplizida.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtgalbvyhj.html

C#:   u is User
来源：http://hz.nanxinkj.top/gtigszisab.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtyyjyqjpr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtvugwfhye.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtcidfsrap.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtyiegonrq.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtctceiqqc.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gthwzidtca.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sufxvd.cn/gtaqgidcco.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtnxdnkcgw.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtqzxchpsd.html

[G15] 枚举
来源：http://hz.cheryme.top/gtszodqxop.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtsegbdvuz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtwzxzaqij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtmjdezoei.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtfgczkuwq.html

Java: enum Color { RED, GREEN }
来源：http://hz.316326.xyz/gtrleeistt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gtkggipzgh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtdlnfionr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gttvukeeac.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gtqezzefve.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtvwszwekl.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtgegqffmp.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtnhdrhxnn.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtqartlfdl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtjyacfdpk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtfxcgwefb.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtpiynjjvy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtiwhmflus.html

================================================================================
来源：http://hz.yuxming.cn/gtbhtwufom.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtxtgbgvvi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtiibqxmlk.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtlxmgwibq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fengsongda.top/gtmwplvqyf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gthjldomie.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtixczvbyc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtuilvukck.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gteqidxtfs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtmlwzvtwt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gtkhrleead.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtvvmtkugl.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtzusunzhj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cdnleiting.top/gtjtxpeiae.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtcqygarhi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gthlleinbz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtbhjpyksn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gthicizubk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtfywyvabt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dashuyun.cn/gtgednltxs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yonumen.top/gtwaumndva.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtcjaexvfm.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtpclxbift.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtpwailwcl.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtrdosyifr.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtzmhnefry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xziqi.cn/gthnodrwfy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtuzlipjgd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtczbujykc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtwgubpyax.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gtcytwkuzd.html

Py:   class MyError(Exception): pass
来源：http://hz.hongshengwenyu.top/gtaubekhca.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtecnrojmw.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtubdcovmy.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtfcjhuvlp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtapbwsbpq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtekruatwe.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtqmizdysp.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtrkozojyq.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtmsqziyqr.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtyulolyhg.html


<!-- 参考信息 -->