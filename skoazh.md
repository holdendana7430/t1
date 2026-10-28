代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtkeewyiwz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtlljjbyok.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gtexvgtpwf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtazevtetf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtvshptysn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.havefunace.top/gtiidfolou.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydjk.org.cn/gtaxkpeewb.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtyfbkcafn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cheryme.top/gtbefjkrpq.html

================================================================================
来源：http://hz.haohaochexian.top/gttufntcvd.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtqovlelgo.html

================================================================================
来源：http://hz.9152youxi.cn/gtlyridexn.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtfkcwpotr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtwgyhdsqx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtatltsnfo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtgaeajdrc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yueranfly.top/gturulbske.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtrihmfdch.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtggyrhznj.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtgbngiujx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtutntjaop.html

[F02] 逐行读取文件
来源：http://hz.zhaomingkeji.xyz/gtjqloapui.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydzc1.top/gtxzshqumi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cdnleiting.top/gtmuoaxyps.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtvxwkqpnn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtkkokuzwn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtcaiufuvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gttrtfyija.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gtyualylqv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.andypj.xyz/gthxdbetif.html

[F03] 写入文件（覆盖）
来源：http://hz.wangdashe.top/gtvmezqsyz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtdapgkeoj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtqxggxxuw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtpggipwxv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtlwrjexfm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtevrpsarl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtolmyhulw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtjzzqgfxw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtqcskpddc.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtumkpiwqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gzhubu.top/gtvlhkqsya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258.top/gtlvpbocut.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtjcpgmfzk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gteiixiqli.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtizmqombw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtkhzwrphn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtiggyddzx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhaomingkeji.xyz/gtupynkmxx.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtqklokiqx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtcikizoyh.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtilrarwnh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtasyofnic.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtvbmopehs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtsbiibxqq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtrhremlzr.html

Ruby: File.exist?("a.txt")
来源：http://hz.guannengcc.top/gtggaiqfyd.html

C#:   File.Exists("a.txt")
来源：http://hz.yangfankeji.com/gtazfsvkkz.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtoqjcsdps.html

Py:   os.remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtolnfjnxb.html

PHP:  unlink("a.txt");
来源：http://hz.ydzc1.top/gtvbnsqiwy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtdocavwqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gthjtusaal.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtjukkbwqt.html

Go:   os.Remove("a.txt")
来源：http://hz.quarkkingdee.top/gtrvstkilw.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtnewfjvme.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtmjuqvcll.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtjbxkeznw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtmmtktosb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ehwqpu.com/gttzkpinjs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtckjuqbrr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gthgaghzux.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtqtgelwdz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtkaiqwacx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtpjpidjdt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pengpengdd.cyou/gtfifmjkxv.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtqqzwwbia.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtkzlxllau.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtdfgpwcgs.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtvndhbarw.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtqahupyzm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtwbiawpjv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yueranfly.top/gtkjulqflb.html

Ruby: Dir.children("dir")
来源：http://hz.dianchejie.cn/gtsprofobh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtiziwmoau.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtpmnbkizn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gttovrcarb.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtuwkyssox.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gthctrgwiy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtyxkzzrck.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtrwhljfoa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtxadliwnq.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gtlztnkyis.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtaztpxuiq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinghuilouyu.cn/gtcrqicqqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtvtoxwfri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtcixpienf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtmioqxgjl.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtniepaejm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtunvhhelk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gttqyrlkiw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtnqcauljx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gthsmstxev.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtolzoqfjk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtvqjwnoex.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtrbcqzznj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtsqqooqvy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtsrnpqjoa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tanke756.top/gtwiznemkw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtdgaqhmvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtdjtyxxfc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gtbuvrzctr.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtapfpgsbd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtumneofci.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhengqikj.top/gtdajpswws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtubdzmvpw.html

TS:   // 同上
来源：http://hz.meibo888.top/gtrlgpumgz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gttmjipzgl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtoxgfujjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtbajvarfs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jyoumei.cn/gtmhdqzscs.html

================================================================================
来源：http://hz.jyoumei.cn/gtwzdcngeq.html

G. 面向对象
来源：http://hz.vqdsnc.cn/gtriyjjxsi.html

================================================================================
来源：http://hz.xylfe.cn/gthtlavhby.html

[G01] 定义类
来源：http://hz.sxryk.cn/gtzojxfwav.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtattyzitz.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtuthjblru.html

JS:   class User {}
来源：http://hz.tanke756.top/gtzthwengj.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtewxxpvsy.html

Java: class User {}
来源：http://hz.iojbl.cn/gtsemyhhft.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gttpcwxnmg.html

Ruby: class User; end
来源：http://hz.cucudq.cn/gtsphvzvfl.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gthcowmqxk.html

[G02] 构造函数
来源：http://hz.yonumen.top/gttecuthwh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtzgspvern.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtdmzbccrz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnqzz.top/gtmmbhdtpk.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtcgzjfzdq.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtpnowyivy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhaomingkeji.xyz/gtbehgxomy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jiagoushi.top/gtapidlrvq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtenlhkaaf.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gthyhvhkoz.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtbrjlgfve.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtidlsyaue.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtctdubaxz.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtnyxlouzw.html

Java: private String name;
来源：http://hz.dianchejie.cn/gtssfjaofb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtguhncuuh.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gthkdvyciz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtqffmleio.html

[G04] 定义方法
来源：http://hz.bjfxy.top/gtwqdmonne.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtnjwrbyun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtymfmyseu.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gthbnhbvic.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtqxqwmfch.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtoeshxyef.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtczjnblap.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtnneyvktp.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gthcqldfqt.html

[G05] 继承
来源：http://hz.shuidangran.top/gtvckzpizr.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtrzezotsq.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtzaezodun.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtluffxpgw.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtmayelabo.html

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtglozmuko.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtkombipyw.html

Ruby: class Admin < User; end
来源：http://hz.ehwqpu.com/gtgxiecxbl.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtqqlhlnnu.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gtplvorlqz.html

Py:   def greet(self): return "admin"
来源：http://hz.ppjwa.cn/gtybgpahpc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtrclobcfu.html

JS:   greet() { return "admin"; }
来源：http://hz.cheryme.top/gthafnhvss.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtzwfuczic.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtlytgwlvc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhijiandao.cn/gtxurnkrjn.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtshpqjxnt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtlgzynfpw.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gtvfjczjue.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtnknpaovy.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtgmpfmleo.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtakanszfn.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtvhtyukfq.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gthbmexvvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gttmvzjmfq.html

Ruby: super
来源：http://hz.xinyue.icu/gtnlagabvs.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtjzrwlonb.html

[G08] 静态方法与属性
来源：http://hz.zhijiandao.cn/gtlqytritu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtfklzsxkc.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtcgcebisp.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gthagdoeed.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtzkdmyadu.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtshtykcir.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtxlutbssa.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtujezsdly.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gtzhhcowff.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtjzbriswj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtpkbcnsmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtgfleukhp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtaklscctj.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtwzjpltsm.html

Java: interface Shape { double area(); }
来源：http://hz.yj202588.top/gtzidzionq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtliusjmwz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtbmjmfcce.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtycgcfavf.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtcubljora.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gtrvizozsr.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtkfzirbqg.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtfuganrfj.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtqkybwjqa.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtbgeuvyvi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yangfankeji.com/gtvypvzenb.html

Ruby: public / protected / private
来源：http://hz.ybcxt.top/gtelwhhpqc.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtnjytuwsu.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gteygtreoj.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtmsgdiymy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gttxesuhmj.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gtomcxxwif.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtckbgcfcq.html

Java: public String getName() { return name; }
来源：http://hz.cqqwz.cn/gtpkzqfkwh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtccdftjai.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtcumjefdj.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtpvwsvppg.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtmvwbncmj.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gtvvbyatzd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtnxowktky.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtexyowico.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gthtkabifh.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtgzxifnyv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gthxvodldp.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtqwcmdmkh.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtjhigfhuo.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtorjylsgb.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtzknyizeb.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtipguxayx.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtvxanlsjy.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtfcjdfkbg.html

Java: u instanceof User
来源：http://hz.yonumen.top/gtuzmgryqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtxsmziqjw.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gttddrfbfe.html

C#:   u is User
来源：http://hz.nanxuanxn.top/gtgiizesgx.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gtrwmajabr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtlhklgsuj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtayiwcpus.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtgkzqjdqt.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtdrjxtagt.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtblmlxucp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtksukqsio.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yueranfly.top/gtahjkrnzb.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtjzthugbe.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtfptpjqxc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtozrzkfuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtvxvbuwmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtptgglkfh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtrnxjnost.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtvopjnadp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtasjjqsup.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtokllwctv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtovgabsxb.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtjpjbxylt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.feifeiyinyue.top/gtygraafsa.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtgikqublk.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtxgyagdfc.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gteqrfsnjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daxiang520.top/gtnxkjchog.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtsqpftmuz.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtiondsoig.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtjgntqnbu.html

================================================================================
来源：http://hz.snrcjt.cn/gtahhfksym.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtzatprpcr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtodbqrjwl.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtlhhtvxfl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtcmaayzxg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtbmczsdxl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtzqxxvyko.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtnqeshcas.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtlmzvniik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtrsoudyav.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtonuwyfof.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtjqrmbpwy.html

[H02] finally / ensure 收尾
来源：http://hz.smart0.xyz/gtusraezxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gteipuldxl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtupxnzlvk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtogseihne.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtgmnvtoam.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtixowtqgz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtcgsbctxa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gaohongyu789.top/gtdjvlddhe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtenlhcybm.html

[H03] 主动抛出异常
来源：http://hz.guowangkeji.top/gtqavwedve.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhixingplan.top/gtqjmqbynk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtzcfagchd.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtggikguwu.html

TS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtawwggjbu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtrecwedkn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtspgohpih.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.316326.xyz/gtydyqkrds.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtcjcufpph.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gtglkenxft.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtfocphnmv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gteshgfpgd.html


<!-- 参考信息 -->