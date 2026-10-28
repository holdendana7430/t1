代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gthyzuqdtg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtcsvwmvml.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtbibavvke.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtbvyukvpi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtusiulych.html

================================================================================
来源：http://hz.andypj.xyz/gtfkmykzjn.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtzjkfyweq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkxhgnfpy.html

[F01] 读取整个文件
来源：http://hz.ivvv.top/gtaggdmcim.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhaomingkeji.xyz/gtkudldqer.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtttcuboua.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtthwikrcc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtcuuxnnmp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtdqcerqrk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtfxcierht.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtdlyefeto.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtajzromaa.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtacjmpbtm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtgjytbbpd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.smart0.xyz/gthnpxvndt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtwbntodzj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtubygzihp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtfujznsss.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtxnvjepcw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtzgdobkdm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtcdmapmfd.html

[F03] 写入文件（覆盖）
来源：http://hz.tian-w.cn/gttnrsldhx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtulwjojsa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtzphvtrgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtkjfqryai.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtrlzgmadv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtjrknddzz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtlzjdylfl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtsyqiryig.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sxryk.cn/gtgkesyayz.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtsfwttkci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtorcslrco.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtmhkvygit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtivdhhbim.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtbhfcvofq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtckufmqze.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtxefraxjx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gtebunrvzv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtxcmpvxyu.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtwmyfqbkh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtwizgyihj.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtsjagvgzy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtmjodbgte.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtbcexlepu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtcafhqfte.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtiymfwxwl.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtkyzaabkx.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtbfgpglnj.html

[F06] 删除文件
来源：http://hz.daxiang520.top/gtihgjbaeg.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gthzeemfuy.html

PHP:  unlink("a.txt");
来源：http://hz.316326.xyz/gtiqlnyiso.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtbmjyxdjp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtcrnicmkl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtnmfkfmxb.html

Go:   os.Remove("a.txt")
来源：http://hz.kuanghao11.cn/gtttjjnofj.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtshvrxiaj.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtwwrjlnfd.html

[F07] 创建目录（含多级）
来源：http://hz.jiagoushi.top/gtohlhjeqc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtwvcpqpni.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gttnlmmgel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtyimxuxjv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtninhidmn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtpkxzoggi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtiwprskjt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtpxkzfuto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gturtiqcox.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtzanzqthb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtrjtlqimb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtkfdawmdo.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtjshpysla.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtdlqnvvno.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtprxrmqcm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gteqalpcqs.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtnhcdmwse.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtvxwefbpf.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtmltiblgq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ybcxt.top/gtohabwetu.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtgtopmukf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtvukorevu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gttafbthit.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtjqukkjkp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtnbtepdks.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtirmgfhgr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtlppklwoz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtxptgvtmc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtzqtokjca.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gtmyskzeyx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtfxeoytgf.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtmmnufkuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtpgpwpjnb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtmtjserig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtkvjpqtip.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtjeuoxujr.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtzxecpttq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtktoiisrw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtszdqyskh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtanigetfj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gttfxagkan.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtvsrfpdtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtznxiubib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtvqozrjjh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gtsvnkzqsw.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gticimixzq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtairqfmua.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtcrvvnxaj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtldtpunwm.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtonqjslzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtgpesablc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtoyujntzz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtbuzyqwdd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtasfsyogv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkviolptp.html

G. 面向对象
来源：http://hz.sweek.top/gtaxyiqmka.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxpxmccli.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtmoxwylfr.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtwfndtrez.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gtrobhyjfa.html

JS:   class User {}
来源：http://hz.hammf.cn/gtmszvvprq.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtyswtbllo.html

Java: class User {}
来源：http://hz.svipenyu.cn/gthofzbhqa.html

Go:   type User struct { Name string }
来源：http://hz.shangyingyoupin.top/gtmeqzbdhj.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtjrrmelrn.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gtmpoqxrlp.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtpnqeodly.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtkzcdbfar.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtrlnfsrwo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtzzvywoqx.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtxuyemvup.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtamfubtnn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtximjmtae.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gtmqrifcob.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtydbfxoqt.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtjyzshjcd.html

Py:   self.name = "x"
来源：http://hz.xinyue.icu/gtdzihjyky.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtnyyjwfmn.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gttjzcvqaw.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtgavfeugk.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtnxqkdmhl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtkmbpditc.html

Ruby: @name = "x"
来源：http://hz.dianchejie.cn/gtakvkqhib.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtwfbpckow.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtcsshlwud.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtiwsethza.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtnhnoxmop.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtuavtswyy.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtejfamxrq.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtyoeugxfa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj202588.top/gtodallgma.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtsdxezead.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtnuhbxdgj.html

[G05] 继承
来源：http://hz.tianlin.xyz/gtqieqjzqv.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtmzzvspqo.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtdfmhvkoo.html

JS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtuxgvxeep.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtwojplmpw.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtmundwtti.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtwdjutmat.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtynkqoxni.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gtsytjisof.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gtvdmvpnae.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtkumlegrl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gthsncsowp.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtpymatdkt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtwsqfurmm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtibqyrfza.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtmsrydsur.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtabjthnat.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtdeawxdes.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtyqgfeepv.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtckjzzren.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtyzkxjiyv.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtvffhyxlj.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtdrrqzegj.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtzlmlpdzy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtndbbtclo.html

Ruby: super
来源：http://hz.fengsongda.top/gtjmlardvc.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtkxoaeorw.html

[G08] 静态方法与属性
来源：http://hz.cucudq.cn/gtgkkgobax.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtumalambe.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gthxpeqnzi.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtbyxdqwyh.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtwgyovheu.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtdmmohnuz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gthsekvibz.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtanddcamz.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gtigxzvvxe.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtsfjogfqb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtqbylfxpr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gtghynnjwc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtirokdjuz.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtyhoapqmt.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtulhxcsuc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtkizotgxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtilamuama.html

C#:   interface IShape { double Area(); }
来源：http://hz.gaohongyu789.top/gtdmfmjnfq.html

[G10] 访问控制
来源：http://hz.fengsongda.top/gtmypikgzh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gtjztevklb.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtawtdzfcn.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtntckyirx.html

TS:   public / protected / private
来源：http://hz.tianlin.xyz/gtuuikvcos.html

Java: public / protected / private / 默认包级
来源：http://hz.0kj1m.cn/gtykvkovvr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.bjfxy.top/gtvadaxifq.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtwfxxjosp.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtyilovzmq.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtacmhqbpr.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtbckvlwlh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtvjbboqdo.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gticmsuhyw.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gteaczsysn.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtwzrqmqmh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtjipvjcnj.html

Ruby: attr_accessor :name
来源：http://hz.aibaodan.cn/gtidhblcbi.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gtbzcyvmnn.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtygogxjyy.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gthgsjzfoo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gteddyewxe.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtqupylsbu.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtejxfaiqm.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangshuangyany.cn/gtjemndrrp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtvrhdgytm.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtelejkmxk.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtyicwbbxj.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtpqenajhy.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtrdfjetax.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtdlnkzzye.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtnqfyhuhj.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gttpaqogdq.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtcnyypkrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtbxkhsnqc.html

Ruby: u.is_a?(User)
来源：http://hz.cashguo.top/gtuanyvizv.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtjyryuyyn.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtawvygsgb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtdnupphci.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtfpahnlzo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gtxnjcmcbs.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtesqoazxz.html

Java: record User(String name, int age) {}
来源：http://hz.sufxvd.cn/gtuhqucsnk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtkgnzskte.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtfhgbaxbq.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtkujptrgo.html

[G15] 枚举
来源：http://hz.ydzc1.top/gtwwwyscin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtboeqjaok.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gtlegsujle.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtiqellasj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtcstbpxuv.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gtysyxvwkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtylekfdqq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gttdcscssd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtjnmtxbys.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtiuxeknxu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj202588.top/gttjcsbjag.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gthmnesoqo.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtjeheupwh.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtoprpumxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xinyue.icu/gtaqsbyfce.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtwmiapurv.html

Ruby: obj.instance_variables
来源：http://hz.ivvv.top/gtgikdcvxj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtwpvdccrk.html

================================================================================
来源：http://hz.zdqjudy.top/gtmsfeznym.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtwwbqmqnj.html

================================================================================
来源：http://hz.hywenlv.cn/gtrojhtlvb.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtqygpecsx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtcunbpyhb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtbcjywtex.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtutlpspwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtuynpvfcl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtogmjlzhs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tian-w.cn/gtwewmxaze.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtpbcrczbm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtwerquyer.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gthxlhonau.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtobeqqbao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtotoeqfqz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtpweekupi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtesnbtosw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtvzjoegtl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtbsyntxdn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gttyznscek.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gtrjedfdkz.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtsymjvxyt.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gtoawlczgx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtghmscbrt.html

JS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtkkuiiswx.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtplwrhckc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtairitpxo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtrjzcgflj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtstiptfpu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtmxvstlpq.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtvznvarkf.html

Py:   class MyError(Exception): pass
来源：http://hz.hywenlv.cn/gtwzbzsshm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtkupfeubl.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtmkdiaucr.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtlvvwffcn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtatwffian.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gtvsmlqotw.html


<!-- 参考信息 -->