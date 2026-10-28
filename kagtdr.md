代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fengsongda.top/gtmzrkypea.html

================================================================================
来源：http://hz.yueranfly.top/gtouzezgvo.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtzzvulpse.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtetswqlap.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtchzqwyxj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtugxgjmec.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgfzy.top/gtjolctlda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.quarkkingdee.top/gtswepuedd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gtrfetdtce.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtniahxryq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gttnxxfqwq.html

Ruby: File.read("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtvojjhqqf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gthcixhxcn.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtedmaxvfu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daxiang520.top/gtgkbduvjk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtowzcklqa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gttzkgmuhb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtvuqceaxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtcnhcmuzp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtipoaaoec.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guowangkeji.top/gtmlsbzqxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtedytnksk.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtzenkgpdo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtwgmouwro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtslfbmfxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtkjepvtvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtzjhmxmjx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtmcoupkxd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gterfccjaz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gthsplwdxo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtzxdpjjzr.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtirvzlhcd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtyhpcdqfy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtfruazaau.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtvyraqlmy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gttjflvnzz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtzljawdyb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtooftmwen.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtaodxdajf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtnrnhmzef.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtjoipzdfb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtmjljambc.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlmjlzcgf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtijvfjofc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtpyjwhzjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtzbkaqemk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtoxjyxewd.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtfxxptyrz.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtajhcnmhu.html

[F06] 删除文件
来源：http://hz.jyoumei.cn/gtrusvysaf.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtrxofhrua.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gttcmyuewl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtehxlgoby.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtzdwkeqod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtiggibwrd.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gttxyrzmew.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtlawoigtq.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtbzpeyjao.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtgwfkrjnc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gtketszdhk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gtvfnycjup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtrabloggz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtfpnvaoli.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gteefpfwip.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtsywfktad.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtjdqqwisy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aizwys.cn/gtdskksxdg.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtzxirepfq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtumevmzzk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtjydfafaz.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtzjekeaoc.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtpvqphaev.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtsxxaerzp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtwjbmonit.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtrubjtusd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtwqeoxljj.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gtvseqicjh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.kuanghao11.cn/gtrwixsqlq.html

PHP:  filesize("a.txt");
来源：http://hz.chenlongwang.top/gtmmzkkesz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtugstfnqe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtgtifefls.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtlfxbpqbi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gttnfomjza.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtdsegepox.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtkopmepux.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtehezobws.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtbcjopfkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.iojbl.cn/gtfihymfkc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtaxvrjnka.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtbejtdpeo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtqumtujdi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtbcbngbnd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtubhcttem.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gtfexxrpzr.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtthxzgznz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtvryoyuut.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtnwjkmgxj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtrdtwomqm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtywafzazz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtbpionvnf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cdnleiting.top/gteamfgozk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtyticislx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnxiangtu.top/gtpgufhezn.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtorezhdvr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtuttqykgn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sweek.top/gtjtoikwzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yongpay.top/gtzlwtgkcj.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtyihvznqw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gzhubu.top/gtxqyqmcwh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtaetitvdt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtmynmfwrt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtgpwnxhxp.html

================================================================================
来源：http://hz.sysykeji.top/gtptzoxfnb.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gtyahfljes.html

================================================================================
来源：http://hz.yj20258888.top/gtovhclchw.html

[G01] 定义类
来源：http://hz.xingfuxueyuan.xyz/gtpwwkpvyo.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtcoyunbsj.html

PHP:  class User {}
来源：http://hz.hnqzz.top/gtzwlwiydy.html

JS:   class User {}
来源：http://hz.xziqi.cn/gtzvnccvpn.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtfbodcutb.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtymcpmgjz.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gthrkkoone.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtatvjenha.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtcpzqdsek.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtvmyylsfm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gthrqnufbi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtqwdwriaj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtmctadnjl.html

TS:   constructor(public name: string) {}
来源：http://hz.xuanzx.com/gtryxnaeec.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtkkkhwbzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gteaclfjar.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtqubuncvg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtszhkotrt.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtbqbwpcme.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtdvjrltch.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtmyivbams.html

JS:   this.name = "x";
来源：http://hz.zhixingplan.top/gttdqlgotm.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtqkdahcji.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gtllzngtbr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtxudtdzkd.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtfavbkmgw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtgzcjwcdg.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtevmqlbfk.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtrppfdfqt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtgdsvaptd.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtwaveqmio.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gttwlrmbnb.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtmxbykxjq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtadnlqhch.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtenblfhls.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtpvujkcil.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtqcjbvakr.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtdngfkffg.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gteqgfwqke.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtbfgaxmin.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtuapwecdb.html

Java: class Admin extends User {}
来源：http://hz.ppjwa.cn/gtvsfgwwny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.svipenyu.cn/gtxacnvtio.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtenukgqlq.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtysqsaljk.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtardyfjbr.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtawqfyxcy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtdvzldbqf.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtreegtubw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtegspmhfg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cashguo.top/gtgxqezysj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gotoacloud.top/gtoanwmhla.html

Ruby: def greet; "admin"; end
来源：http://hz.zhengqikj.top/gtqrzoyqjo.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtrkcqwcxm.html

[G07] 调用父类方法
来源：http://hz.shangyingyoupin.top/gtwpyavdij.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtgbgwluqe.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtmiwrnmgn.html

JS:   super.greet();
来源：http://hz.dashuyun.cn/gtaigmbuac.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtobddlaic.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gtlgmwltyc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtiusufehw.html

Ruby: super
来源：http://hz.xinyue.icu/gtdlpgqsxi.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtuklrgzas.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gthwhjtqji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtasmpqeej.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gthcmfgxyg.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtnwbpazoq.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtvzmigxnt.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtpwdrkziv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtpnrgnjwh.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtcsmkbfco.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtulgiborq.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtyibybxsx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtcfyxwslx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtjuckxeon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtpexusgth.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gtpxjbafpm.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtehufjxis.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gtusvlwihm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtbnpjomuh.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gtapkrlfnk.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtitkmvhkf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gttjebjpqe.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtpyhreyqy.html

JS:   #private 字段；其余公开
来源：http://hz.nwbrower.top/gtnjxlwbmn.html

TS:   public / protected / private
来源：http://hz.sufxvd.cn/gthbsnplyz.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtwlpejwmt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gternafust.html

Ruby: public / protected / private
来源：http://hz.gaohongyu789.top/gtgpmwsxqw.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gttbftzlqq.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtdfjkomxb.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtcyxxegno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtanjyvvnp.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtefycpefh.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gtjnhdawiv.html

Java: public String getName() { return name; }
来源：http://hz.ydjk.org.cn/gtrfmefrqs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtffvbyhtt.html

Ruby: attr_accessor :name
来源：http://hz.hywenlv.cn/gtojxqxjsw.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gthqcijdrr.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtqjnyjshs.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gthxfafuak.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtfndnnfue.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtmpqnjeih.html

TS:   toString(): string { return this.name; }
来源：http://hz.nwbrower.top/gtwpihwirs.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gtzkavspfu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtuvincmwg.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtmlsivtms.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtbmymlnml.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtydwtsfle.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtflkyckbb.html

PHP:  $u instanceof User
来源：http://hz.yuanzhike.top/gtzihvzizy.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtgfwjojmf.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtgtzxxrbf.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtcusnvqnm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtvqywitut.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtjtgpssgo.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtxkgtstcr.html

[G14] 数据类 / record
来源：http://hz.hongshengwenyu.top/gtmlwfkpyy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtdmlpqydo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtdgcvlavz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtxmfrwwlm.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gtnovkjkuy.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtqhgkpxvc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtorpjfrjw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtpmxsxxxn.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtmuriztvi.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtnlqvlime.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtyjjxdoju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtjsphppch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtnuetgmul.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtjsfcmqvo.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gthoxbznzw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gttfjrfmrg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtiqjntgvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtmqoiuwrh.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtyhelpskc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtenwoccaa.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtckhhxogb.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtixnyiiip.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtnhizhmdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.havefunace.top/gtvhhqlpal.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtxanmclxq.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtqcazjvpx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtfpnykwbx.html

================================================================================
来源：http://hz.c1oappe.top/gtoohkbiaj.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtvurxklhk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlqgifmye.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtkyjqsvye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtpnayldku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtqrtzycow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gthkdawiys.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtylwexfhl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gteeavcfen.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtkwrmkaic.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtghwlfcoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtdmglebpv.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtxiirbkqm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtkstastab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtcizbgugu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gteyqyfxkl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtiwhobrjr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtihumsauh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtlafbsrvd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtssvtfjkn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtttferwer.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gtwdthxoor.html

Py:   raise ValueError("错误信息")
来源：http://hz.andypj.xyz/gtinflajld.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtkdexatsc.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtzwqvxexm.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtbnkyhkwn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtbxhrlawz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zdqjudy.top/gtbadnexzf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtqonpavyw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtbieviuov.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gthabbkqlu.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtqzxkbfrb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gttdlqbxdk.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtzlihbllk.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gthkkteonv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtlhncvjnp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtuolrxgbs.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtaucsyebb.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtimjfonyh.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gthpkzblxi.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtxrhodjlh.html


<!-- 参考信息 -->