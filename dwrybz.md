代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gthywerkvl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.9152youxi.cn/gtbeirwgsv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtjujfgmxt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtmutvlcqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtfxahiwon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gtqjhoekae.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gttkhblaym.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgfzy.top/gtdtgsmcqg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtloewrjix.html

================================================================================
来源：http://hz.snrcjt.cn/gtwofiiswg.html

F. 文件与目录
来源：http://hz.yueranfly.top/gtcixhajhf.html

================================================================================
来源：http://hz.smart0.xyz/gtgsqjgxeh.html

[F01] 读取整个文件
来源：http://hz.aizwys.cn/gtqlezfnmp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gtgwrhqgei.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtobvoudur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtkildclky.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtyerhmgju.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtccrpwaiz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtwthnswga.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtbofatyos.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guannengcc.top/gtmoxvfkth.html

[F02] 逐行读取文件
来源：http://hz.yj202588.top/gtljwezden.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtgpimtqes.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtsmwzpdga.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtmnzolkim.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtfkordsha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtktizefvp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nwbrower.top/gtlyiyxhws.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtwtqafsfy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gtmxixcvul.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtgnckinun.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtzsfemcts.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gttguxgnkv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtwbzowlxx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtylesywog.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtodhhcpeg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtjzmgflol.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtmnfkzzhy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtuygriswq.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtjtrawoqa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daria6918.cn/gtgyfycdft.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gtfkvzvgrn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtwqhzgysv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtqifqjgms.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtcmjfybuc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtwppkpqgg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ppjwa.cn/gtxrjqzivi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtoubfogem.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtkmfdrelu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtpkdbhqpv.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtmybrtltt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtugplyqzr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtqjrvnvey.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtjhxvzknv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.0kj1m.cn/gtonafrlct.html

Ruby: File.exist?("a.txt")
来源：http://hz.andypj.xyz/gtgqdhcuzt.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtpnlcvvgw.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtvdeoiajj.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtsdcmpili.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtvuaeoyuq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtxcgddutz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtnqocuozc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtgwdkeodk.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtyuuwqnmp.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtfjkojgpj.html

C#:   File.Delete("a.txt");
来源：http://hz.zhengqikj.top/gtriacfnxa.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtelfkyopy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gteqcpnjgb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtpoljynje.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hywenlv.cn/gtkpknyosx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtqmuyljea.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtioiwxhoc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtqhuclkeu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.9152youxi.cn/gtlnbygyyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtenphfqvz.html

[F08] 遍历目录
来源：http://hz.sweek.top/gttcpqedac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gttfbanzzy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtetpkymwh.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtvsahxtdy.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtljnhgfhk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtbgoyltla.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtlydmilss.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtbbnwzcws.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtulirpixl.html

[F09] 获取文件大小
来源：http://hz.fzhhl.top/gtpdzfynks.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxinkj.top/gtrrmoamoo.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtdeeblssu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtihxohdmk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gttmqzdfub.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtvrweazsc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtaaqmjtpn.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtodeszpcf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtcbkvygfe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinyuanbaomall.cn/gtcvnvgsry.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtknncgcbr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gthkwygbpw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtwcndciqc.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gthrnzdwrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtbzmdtwrz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtdppdjldj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtfhpxitcn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtupmjxggz.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtgwtgqkpp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtkjecvzgn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtrsercora.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtckyuaarh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtkibjaorm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fzhhl.top/gtfwhwcnpe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhiwuduotai.top/gtnetciiyr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtyweagdnd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtntljnpbl.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtnzsnlbsj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhongyouzk.top/gtwvmwxjyz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtdagyhwqi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.redwolf501.top/gtyoiyjoht.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtzhgchgdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtobpbifrg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtjkhyulam.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtnjyquygz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtyebceftf.html

================================================================================
来源：http://hz.nanxinkj.top/gthsurmcdv.html

G. 面向对象
来源：http://hz.yuxming.cn/gtotucfnsy.html

================================================================================
来源：http://hz.snrcjt.cn/gtwssusqxj.html

[G01] 定义类
来源：http://hz.havefunace.top/gtpdmjvjaf.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtqzvhgnnp.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtodpmzura.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtuzaftsox.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtlyruffus.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtaaojegnc.html

Go:   type User struct { Name string }
来源：http://hz.sufxvd.cn/gtevkkaqbh.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtlgfgjypx.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gttglpmuab.html

[G02] 构造函数
来源：http://hz.zycfv.cn/gthdvsuexy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtsaegqefb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtuxlrubct.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtovbajbxy.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtiybfgahc.html

Java: User(String name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtewblitkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtfxottuzv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtposdfrnf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtygzyenev.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtsqhltiju.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gthqkrfmny.html

PHP:  public string $name = "x";
来源：http://hz.yj20258.top/gtwocwfmdw.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtmtfyzghy.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtzpewezmd.html

Java: private String name;
来源：http://hz.svipenyu.cn/gthxjxozbn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yueranfly.top/gtsmouvssa.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtxkfhhjfr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zdqjudy.top/gtbmxeibxq.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtkslifcfq.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtzsbjgaut.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtfphktzrt.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtfpjexetl.html

TS:   greet(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtezgpstsj.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtsgqjsmhx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtopjttiik.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtbxyljagl.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtmcrhhpfv.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtrcwhsjdy.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtziuctdys.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtjjqkvikw.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtvhpammga.html

TS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtfhuywmvf.html

Java: class Admin extends User {}
来源：http://hz.gzhubu.top/gtkreynvur.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xingfuxueyuan.xyz/gtpjtjrhkc.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtkeqmyjqv.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtxoukoizb.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtpnxixdlu.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtzrypzvsb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtivypiccl.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtdgwlplat.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gttwolxubx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gttdetlabd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtuvvwjtlb.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtijjxrkax.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtqbcgoulj.html

[G07] 调用父类方法
来源：http://hz.jianghu66.top/gtlhbzqxrn.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtwgsypxfe.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtgieqxgik.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtghkqbker.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtpvubyjqp.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtqiseqytr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtkmkorhnr.html

Ruby: super
来源：http://hz.yuxming.cn/gtxfupxlhr.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtuhythhtq.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtbigjasqf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhoulong.xyz/gtdopitzif.html

PHP:  public static function f() {}
来源：http://hz.jinqigufen.top/gtawyeowqb.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtqpthmlhm.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtaorxqayh.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtugjnpdet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtztyxhljt.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtvdmrztec.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtwgbtlfoa.html

[G09] 接口 / 抽象类
来源：http://hz.316326.xyz/gthlclutxu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtqxuzgtza.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtkxldmjtr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gtfahuchvs.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtksapiqxj.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gttivheokf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gttcjkzzhl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtkrwkzhkm.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtgprfwrot.html

[G10] 访问控制
来源：http://hz.havefunace.top/gtpqwtfvpr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtmzwneurs.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtpdwkomwa.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtzpoxlhrf.html

TS:   public / protected / private
来源：http://hz.jinqigufen.top/gtnqpsidyq.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtepawapoy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtxyqtktla.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtrztoptqj.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtcubfeygx.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtksarfghu.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtwaikzdxo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtbqgempjv.html

JS:   get name() { return this._name; }
来源：http://hz.meibo888.top/gtmbrwgpph.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtfwfkiccw.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtmrxvlowt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtomchyild.html

Ruby: attr_accessor :name
来源：http://hz.yangfankeji.com/gtkuxjmcgx.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtscmcnwmn.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gtmtqzjuqc.html

Py:   def __str__(self): return self.name
来源：http://hz.hfpthk.cn/gtglcbmuoo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtqjtpeyfw.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtwlckrjhh.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtyfkmwapt.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gteahzjixo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gttjjngxva.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gtbveakufw.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gtmzkmdlfm.html

[G13] 判断对象类型
来源：http://hz.pengpengdd.cyou/gtmxaxibnt.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtbxlqetof.html

PHP:  $u instanceof User
来源：http://hz.0kj1m.cn/gteqzihlup.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtnplfnjtl.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtpmzmwtqi.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtakggylij.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gtpcvrjaip.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtifjwfhtt.html

C#:   u is User
来源：http://hz.quarkkingdee.top/gttvqwsomu.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtjsyvgeku.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtnmsqofdf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gthjwbhlja.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtpopkmxzz.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtyyukqmep.html

Java: record User(String name, int age) {}
来源：http://hz.jianghu66.top/gtynxzfvwf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtrmrjrhkc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtwvaumhsh.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtpvxhcwbx.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtevvfluls.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtdeuutepu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtjeofnzpx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtarzdcens.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtkclfskdm.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtzzkyrknh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtwfoxwdwn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtwfpiywkk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtdtuwsvzh.html

[G16] 对象转数组 / 字典
来源：http://hz.zycfv.cn/gtcwscycze.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtwgztfpmu.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtfajatjhm.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtdenrosmm.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gttnxpedyh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gthktbtbxr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gttiplrjed.html

Ruby: obj.instance_variables
来源：http://hz.xuanzx.com/gtrjflusyy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtreddznfa.html

================================================================================
来源：http://hz.meibo888.top/gtlvxngyrl.html

H. 异常与错误处理
来源：http://hz.ppjwa.cn/gtinozzsvz.html

================================================================================
来源：http://hz.xinyue.icu/gtatckpdfi.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtbcpjtwqj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtgjozdvev.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtntypadxm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtsqgodqit.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guannengcc.top/gtyzhcwmsr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtupsrkojh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gttzrppjyp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangshuangyany.cn/gtyrrqturb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtbcehzska.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtthlusmom.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tian-w.cn/gtzwmyidqh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtiuwqpqpc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gteifrguhb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtfgjkmyjk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtlmuqsarg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtfqhiphqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtjopnbfql.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fengsongda.top/gtajpkshwp.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtnwdxpjvy.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtlspuefgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtngfooahs.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtvmpusthd.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtijeoixwv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gteltfhiyz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtkjnooyej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtmixhtumd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtzazolecf.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gtschxpppw.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtkwzjuztt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtjkybdpme.html


<!-- 参考信息 -->