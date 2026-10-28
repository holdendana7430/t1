代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtyliqszgr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtqfzocyoo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gthzzwetxt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtaogjcflw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtuwynjisw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtywmppeyr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtdozikzds.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtanvawene.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtxdksekek.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtcemdhbri.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtwybwhtmx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtgefqdhfm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gttvxzxkpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtliqhwgdk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtxdaqinso.html

Ruby: s.bytesize;  s.length
来源：http://hz.aibaodan.cn/gtecjcrrxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtnfftkfhk.html

================================================================================
来源：http://hz.dashuyun.cn/gtnpkcteqd.html

F. 文件与目录
来源：http://hz.sysykeji.top/gteuvjahcq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwejqhcfl.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtyjhrvzcb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtewgvqupu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtuxdbzyrv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtwzfcykhn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtfczraasa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtxxvzhtzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtcfyrbtle.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtcexampqg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tanke756.top/gttwobrijb.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtyfmqjnov.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtlukmuhys.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gtaecuidsf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtjnzxhwyz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtjgvmhwvf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtsurtmcpq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.smart0.xyz/gtqtuyjcxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sweek.top/gtwjpbsbke.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtobksfaka.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtuljkaatf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gthuevipbw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtnaawnuld.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtykdnwfxi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtjjnlrjoo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtbtpglzqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtoixfenya.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtkkirutig.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtenwbejbh.html

[F04] 追加写入文件
来源：http://hz.shangyingyoupin.top/gtjimhxwif.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sufxvd.cn/gtplludeyo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtbalbwnus.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtqtjzghws.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtnqjsktma.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtrpcwefsj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydjk.org.cn/gtdifodngi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hywenlv.cn/gtqvjaideb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtqowvrscw.html

[F05] 判断文件或目录是否存在
来源：http://hz.ehwqpu.com/gteakwstji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtmtvghgnx.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtdgypqvyi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtnbykigii.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gthitzfnnv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtrxcamuen.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtvuzgbyec.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gtgeqwzzce.html

C#:   File.Exists("a.txt")
来源：http://hz.zycfv.cn/gtbcostbcr.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtkufrxyai.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtnnatykes.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtxfkqnwwr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtvynljmzw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtxpootssn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtwoavgikw.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtfecegjkg.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtwfgokvpy.html

C#:   File.Delete("a.txt");
来源：http://hz.redwolf501.top/gtkasurrep.html

[F07] 创建目录（含多级）
来源：http://hz.ybcxt.top/gtfxossalv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtlwfxnofm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtnpwtdjzw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtirvlsdvx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtebtdztya.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtelhpmosf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtavndpwpm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuanzx.com/gtbpmlpamu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtyxanoaah.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtindttdcj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.havefunace.top/gteuunvpvd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtmndcjegu.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtlvivbquj.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtrgvwcdub.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtkkkhqecr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtnijsnegy.html

Ruby: Dir.children("dir")
来源：http://hz.pengpengdd.cyou/gtrjcffksy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.iojbl.cn/gteylzuyny.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gthdbxcxia.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtdkfvjlik.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtpbcfigmo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtptkifmvc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtmtkmjhhp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtwzznxnzu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtxjxcfavj.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtsnhnfkpt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtxerfwfwr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtdprnkzef.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtrmtsoyfd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pycfn.com/gtxeohnjhe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtgpizound.html

TS:   path.extname("a.txt")
来源：http://hz.hysaishi.cn/gtltisqspa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ybcxt.top/gtjvtollch.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxomzzhen.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtrarptpyf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtvucnvdfs.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtitjurekp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtrfjiecgj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangtech.top/gtywepbznf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtyijinibv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtqamlrkyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtupzfrmve.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtkkxqnntz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtgmabjzvd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtumgmtcts.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtoaichbay.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gthwtknkfx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtmaixbejp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtmraxuvbr.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtabmzrxux.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtbkrrosdg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigfzy.top/gtpftmjtyj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtqthpdrfd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtscqehikb.html

================================================================================
来源：http://hz.xinyue.icu/gtdypskppu.html

G. 面向对象
来源：http://hz.zhengqikj.top/gtodargzcz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtiukdnouu.html

[G01] 定义类
来源：http://hz.tanke756.top/gthdckxfbu.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtoclepbiy.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gtyvyrrwiv.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtbeqnyakj.html

TS:   class User { name: string = ""; }
来源：http://hz.hongshengwenyu.top/gtatodtwqh.html

Java: class User {}
来源：http://hz.sysykeji.top/gtibeucgpj.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtzrnbilps.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtihrxwbav.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtavfnfwgf.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtylakjgls.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtdvrrozzz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.mhx1999.top/gtyescdblt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gthpqklejw.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtfkyjujxy.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtvbpzzfjj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtfeieyetm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtqxnlaimd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuanzhike.top/gtqsncvdbq.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtgelwvidv.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtaaomujka.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtuhzumxst.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtuqosmmnf.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtiaaiyfeq.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtlxtrxrrn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtthchgypx.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtqrjbxyck.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtzywgrvef.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtwkswkgvd.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtapgkbwbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtbmfmircf.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtuorvwmxs.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtmoohpptm.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtsypqxvqz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtlfybovxg.html

Ruby: def greet; @name; end
来源：http://hz.jinyuanbaomall.cn/gtdcyiuisa.html

C#:   public string Greet() => Name;
来源：http://hz.ehwqpu.com/gtkvtgtvxi.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtbhidggse.html

Py:   class Admin(User): pass
来源：http://hz.zhongyouzk.top/gtzbfrnpmm.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtrwfhwuxh.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtyelqyglx.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtfkghkhbo.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gttkklmdwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtjkoxixsl.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gttanqcaif.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtkvpyktqg.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtpcfbhorm.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtvuorjzcc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtspgjbiuf.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gthehzcubp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtnidpctdl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtpadrhbab.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtwnbfulsa.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtcaojloaq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gthevrmpsp.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtzddfbpza.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtidafdiej.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gtijvfhrvj.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtxoaikopa.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtnekefcgl.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gthnfdoeuh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gogol.net.cn/gtbeizqchv.html

Ruby: super
来源：http://hz.ppjwa.cn/gtjwhotfhe.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtuvggwweq.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gtfxfktovr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.mhx1999.top/gthdnqlhbs.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtfxclngwy.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtuyuxzeif.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtbsbnylhb.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtupaxnojm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtubfeqrwg.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtavzayuqf.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtgzsftast.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gthvmkagsm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtityhyebh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtbincesfw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtxdsmyihl.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtblmdxpld.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtdbsatbwc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtcqrndenp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtcygwamep.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtecluzygr.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gtdeupvueo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fengsongda.top/gtoxpmgyaj.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtfplcbrlg.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtuusmikbf.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtfkywtiui.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtqtwsljaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtmbkobnfg.html

Ruby: public / protected / private
来源：http://hz.fengsongda.top/gtbqexuyhc.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtlhtjzsuq.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtonhqfuza.html

Py:   @property 与 @x.setter
来源：http://hz.zhijiandao.cn/gtmeglwyup.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gthymjojjb.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtubcsrbhj.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtxxwdvpsk.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gtnqwaaxqr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtkovlaszh.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtrrfrpfjp.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gteehaedgd.html

[G12] 对象转字符串
来源：http://hz.redwolf501.top/gtofinkjou.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gttnxbceud.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtfutgrtzr.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gtamtpjrab.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtjmdzbcub.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtfqfckvba.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtgigpugdj.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtdgdqxvxx.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtgafqbvlu.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtfkhdftzr.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gtzmqhbrba.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtiuyzykst.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtnelrvkmn.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gtrfemecbt.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gtnenagpdp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydzc1.top/gtqlulopnr.html

Ruby: u.is_a?(User)
来源：http://hz.cashguo.top/gtyqgotwia.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtfoztngfl.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtczzvjhhw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtgjzkthpg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtbvoogxdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gteasbzckv.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtfqtaaelv.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtmbjfepik.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtpbggmmjz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gtapcnigce.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtghymzgfa.html

[G15] 枚举
来源：http://hz.zhixingplan.top/gtuatsgusu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtlosbnuyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtkxrfmeve.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtmrpmqrzn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtughhkxqe.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gteuqcmlwd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.andypj.xyz/gtrbtjadet.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtnzyjvqwi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtymjxmvbt.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtbjnmyfvi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gthtzsmjkv.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtxjhzditj.html

JS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtonlednuh.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtcxhvlpot.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtzjcngnpk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gttjkarymv.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gtiupjcqvp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtecbladxj.html

================================================================================
来源：http://hz.shuidangran.top/gtswyyssww.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gttpcvyaae.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpjfoidgo.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtdzfomszx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtdwbivgxj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtdtxgdeot.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtfybyaexf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtppudprho.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gtjfzldlne.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtclpkiaaa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtvcflyanx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtvnqyrrzf.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtrijmlnpl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtllufypvi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtanoonict.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtfsiyhwsd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtlzzvaekw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtifhtdgrn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtgtzrascg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtrogsslnj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtzhcmllrt.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gttssmdpcu.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtlttraswh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtuqplcrod.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtpiqrpqme.html


<!-- 参考信息 -->