代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtxblaufus.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtuosakfeh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gtqqghzzzb.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtxnyuyywj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtiwumeyld.html

================================================================================
来源：http://hz.wangdashe.top/gtkjcxizfn.html

F. 文件与目录
来源：http://hz.redwolf501.top/gtgmyvvkcz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlzepgace.html

[F01] 读取整个文件
来源：http://hz.sufxvd.cn/gtjzgerbxv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtxnajghjr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtdmjsshal.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtneluxswc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtmxlzkwvg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtqycbxurp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtcolvtcpz.html

Ruby: File.read("a.txt")
来源：http://hz.guannengcc.top/gtoagwyscj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtxgqiyope.html

[F02] 逐行读取文件
来源：http://hz.fengsongda.top/gtjlpcgrzs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fzhhl.top/gtxwedafpn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtyjyhmuxj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gttnxjilct.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtdtcwrboz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtlvivxrfj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtdvjniasd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtyiziismc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtpwzdofdh.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gthhxbzkxn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtbasvupyi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtsyxatndc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtxkvffurc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtvyuxegag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtfuufkgik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtstrwwlzv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtoooxwera.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtdughfgsw.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtuqzsolst.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtlggzujrr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtbkehbnju.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtxjrezhud.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtcpxdmyjk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtfwkpcdku.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gtzjzyrgto.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtyzszabxh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtwyzcevof.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtmqjddntf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtanmbtpsd.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtjdxojbtn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtgjuxlago.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtegemacal.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtnbqllukt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtxeltjijj.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtfadawggv.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtoxfydejm.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtqgjfeglm.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtxmmbiphw.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gthcqjifcv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtjhirqobo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtkdclusus.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtfmyrwpiv.html

Go:   os.Remove("a.txt")
来源：http://hz.wangdashe.top/gtozmogwbh.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtjoclolrb.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtturaphqx.html

[F07] 创建目录（含多级）
来源：http://hz.ybcxt.top/gtbtbneggg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtjtmfooso.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxinkj.top/gttbrpfqhv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gticlzulhy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtgzygjhjw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gtoxonwukq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtzihjktsq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yanxiufei.cn/gtdcndoyrn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtkdirzoyr.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtejfgdyvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtueuhzrqc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtdpxmwozz.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtfqlyxryr.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtxmwcgysp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtsuvdswux.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtvkutnrll.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtkdscdrpx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtptaigxwc.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gtnmkbsvrz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtlpraavym.html

PHP:  filesize("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtnunocryf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtfnoddhmq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtoxnhheqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtebxobyyd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtmkubfexk.html

Ruby: File.size("a.txt")
来源：http://hz.pengpengdd.cyou/gtetymieft.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gthhdsbdbk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.snrcjt.cn/gtlxsgohhu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtyftutjoq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtmeszksjb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtjhvtgyyp.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtnfdamksi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtagxbywoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gttoalllib.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gttjzsspsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtcubixunq.html

[F11] 复制与移动文件
来源：http://hz.9152youxi.cn/gtggmxldcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtbvjwwsic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jianghu66.top/gtsyxdjtsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtykfjsvyp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtmvipjuml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtheromzpl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.mhx1999.top/gtpzwhbvhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtkthshhjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtqnngfdpy.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtiedaoary.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtvhrsyuxx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtnzxldrpi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigfzy.top/gtyakjwejq.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtolylloko.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.snrcjt.cn/gtesxloadz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shzxlz.cn/gtvinnvlpu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tanke756.top/gthjrtxjoz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtipxnobtd.html

================================================================================
来源：http://hz.tianlin.xyz/gtyafwunnv.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtwdtwpjse.html

================================================================================
来源：http://hz.dashuyun.cn/gtymdnolco.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtiuwxmjnx.html

Py:   class User: pass
来源：http://hz.hnqzz.top/gtfxyjorbe.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtsguvkkrq.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtzoyziwoe.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtewcylgtj.html

Java: class User {}
来源：http://hz.wangdashe.top/gtsxfhmjoi.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtdpijgznt.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtjcyjbamn.html

C#:   class User {}
来源：http://hz.hammf.cn/gteglmqlfy.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtuijyawgr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtemoixbwc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ywan-chungtsiang.top/gtwzkaoxbu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtuettoikc.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtgyacbbdj.html

Java: User(String name) { this.name = name; }
来源：http://hz.sxryk.cn/gtvhevrmos.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ivvv.top/gtpjwtnjyt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtwrmihbfi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtnlqnmafn.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtjenpvmwy.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtjjeptbrr.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gthdrlzswu.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtgyqxbrws.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangkeji.top/gtufscqtmi.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtzyodehnu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtaolpzfqi.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtervmzwdc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtkiehafda.html

[G04] 定义方法
来源：http://hz.chenlongwang.top/gtcicelwae.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtlsvuuyah.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtxkkfuvzi.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtyafbftse.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtefndmryx.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtfazdbqzv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtocphmbda.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtssewmtzs.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtfqhywxxb.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtfyhzoqfi.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtyukcnwif.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtcibehxrl.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtvuojzqqy.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtpfkkthfk.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtechgcnte.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gtmzkcqqgr.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gtamxperba.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtavnrimgt.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtprehyiij.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtmjjxkdnc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtbnyschns.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtodrjlwih.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtscgfsqtn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtjrvpncsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gtmcmzjkij.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtesolhhzu.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtctsgwbji.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtmjhnuguv.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtduvffjva.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gttvyutjbk.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gtmdrplesh.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtkubmvdbs.html

Java: super.greet();
来源：http://hz.shuidangran.top/gthyijxqpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtnjzldtmh.html

Ruby: super
来源：http://hz.cdnleiting.top/gtgnmznoer.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtepfnzjmd.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtobavvkcy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtdwbyttqp.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtpcoddhsp.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtbnsvhkld.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtqechddrl.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtxydwyxaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtyvuhgdhz.html

Ruby: def self.f; end
来源：http://hz.c1oappe.top/gttahhsbnl.html

C#:   public static void F() {}
来源：http://hz.hywenlv.cn/gttfvykbtu.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gttegfhknh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtzgbfeqqj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtjifbqnji.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtzpxmuyrt.html

TS:   interface Shape { area(): number; }
来源：http://hz.jlsjyb.cn/gtblrfxyeo.html

Java: interface Shape { double area(); }
来源：http://hz.hammf.cn/gtdcopqmex.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtoqhbrcof.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtdnoymlak.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gttirlfatj.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtjfqpjkdr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jyoumei.cn/gtyifxovmv.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtzflkzxol.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtalkazcrq.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtjtukcvci.html

Java: public / protected / private / 默认包级
来源：http://hz.hywenlv.cn/gtdbmmocgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhixingplan.top/gtitcegwcq.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtpvittxqw.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtzqfgxxmb.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtjwendvnq.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtkyonqjtl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtecauxvjh.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtdlmggwmh.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gthhfxpmmj.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtgvvlllgn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtqrjhymba.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtgqemnnhn.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtfvgrskes.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtvjdvdsdt.html

Py:   def __str__(self): return self.name
来源：http://hz.daxiang520.top/gttpfpfssj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtwmabbqgd.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gtanbmrlew.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtaqnlclvn.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtgtjeqcnv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtryvahnoi.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtdtalcfha.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtmrdxqftj.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gtwcbdzhjt.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gtqnmtxhle.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtdjsidqpg.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtesygwgok.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtovrkrrkf.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtiplrfnky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtnsukgvyg.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtmqugujao.html

C#:   u is User
来源：http://hz.yvedp.cn/gtnnbvqdhh.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtqdeclxmz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuanzx.com/gtxwrjqjqd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtoswzvirf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtabdrmuro.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gticyyzroc.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gttmfltrqa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtsdarwvug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.iojbl.cn/gtfsfwanrp.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtvpvlcaxv.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtyvwhmvov.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtiachkynt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gtnrlegigm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtdwsfseaq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtqwuuzoyu.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhiwuduotai.top/gtfjnrmsbk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gtziucvlzx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtzkelgbat.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtnbvgrwwa.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gtwjvcwgcc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtzamnasuu.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtduaouakc.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtjmnkgktt.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtiuvnczjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtvpeybpcd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtcixqvdsw.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtmyebnivb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtkoopjfwr.html

================================================================================
来源：http://hz.yongpay.top/gtdtsoiejb.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtjeytquxn.html

================================================================================
来源：http://hz.hnxiangtu.top/gthurnzatf.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gtruzdqizg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtykxhwbog.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtptfeclpg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtpyybcqiy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtuvmurxiw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtxvchonoq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtxsmssjou.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gtmvblyftv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtujhpquhm.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gteqpfpmzo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtzxeimxva.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtzjlufhab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtzhqwuvpt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtpusjhpeo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtxbyuehxk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtixklnflk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhixingplan.top/gtljawyxbr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cdnleiting.top/gtbqizpthk.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gtczbkkivl.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtrspmxfqv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtmiwgjyeb.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtggcjlhny.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtuajtfsbx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtiecdanro.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtvgdtdxxh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtfnhwojvx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtmksoljiw.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtlmuxzwas.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gtbjooyjky.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtkxaihikn.html

JS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gttellqpjo.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtvseguvnc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtqvnliuxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtrrydghew.html


<!-- 参考信息 -->