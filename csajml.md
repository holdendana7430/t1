代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtpldlcoot.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtsnckykoy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sysykeji.top/gtldxkcvpz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.andypj.xyz/gtidmwppvj.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtxyckeaws.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jiagoushi.top/gtaceexvvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtxlrkwnoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtajtoxcnc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gotoacloud.top/gtvdmsyfel.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtlpetdbsf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258.top/gtnbgdyjeq.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gthbrvygyu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtjzpprgpm.html

================================================================================
来源：http://hz.yvedp.cn/gtescpezbs.html

F. 文件与目录
来源：http://hz.vqdsnc.cn/gtmwjiudxl.html

================================================================================
来源：http://hz.cheryme.top/gtfgwiozxo.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtxnljsglt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtidfbtoty.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtsuvcenko.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtrczwieha.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtoswiphzm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtobwtlwrz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sysykeji.top/gtvfmsebkf.html

Ruby: File.read("a.txt")
来源：http://hz.ehwqpu.com/gtwellrbcz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtcvrtznft.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtxmslcgpb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtdktlqpfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhoulong.xyz/gtndejpmxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtahvwgtxb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtjlayfalo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtakqbqqkt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtsahzlcpx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gtrwxiltbj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtjuykdlfg.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtmyhufbwy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtrostaeyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtnwdzadgy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtnslnmmpr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtvklhemxa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daria6918.cn/gtdfijfqkz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtjyghrfto.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gtuqizfwon.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtabygotcs.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtkluykhrk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtuqjmazxu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gtlyqyeeay.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtyggobehs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtdcscvfay.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtjgjmkkat.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ywan-chungtsiang.top/gtbjalefqj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtbzsnnqmz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtpjlgcpyg.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gtfbxfrxft.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gtnicdajqw.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtneksjdlj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtcvoyviop.html

TS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gterjdbuep.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtmrqloikd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtihfnjqkl.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtjnugamfm.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gtgfgufwca.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtbhwagdvm.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtdrdikebf.html

PHP:  unlink("a.txt");
来源：http://hz.9152youxi.cn/gtscxyfksp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtqodninym.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqhyahlei.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtvhxhnirk.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtlaipxumc.html

Ruby: File.delete("a.txt")
来源：http://hz.jyoumei.cn/gtblgdvyjw.html

C#:   File.Delete("a.txt");
来源：http://hz.hammf.cn/gtkgfarkty.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtcwvcojbx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtgqowgocr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtxkkceiro.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtknzmwczp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtviwehyhj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtrvjtquvu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gtmgclvjaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtqvnrmrhb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gttzbenuzw.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtxzsdgxve.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gtywxyjtxl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.316326.xyz/gtfgdjuaat.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtqztgxmko.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtattgyopg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtpvtrfszu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ivvv.top/gtbwxwuzjn.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtywweiyub.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gthhyamtmv.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtcgespglh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtjyfwpmxk.html

PHP:  filesize("a.txt");
来源：http://hz.kuanghao11.cn/gtyegokwny.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtxjbcvcry.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtlpsfskos.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtcrrrribs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtytcqvwsf.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtnmkryguj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gttrtcrrtr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gthducugwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtkfmbvewj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtxzgayzkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtdvnoghxi.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtnlpupybc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cqqwz.cn/gtboclxwcb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtorymauxp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdwixbdfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtixgnzzdy.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtmkkplcjz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gttdpojavl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtbrjfoyjr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtjrtwzkiy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtbpbabgzs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtymdjcfkx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtwtrcdxbg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtvjebtjfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtcanejpvp.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtotumkbzr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gttmciywcd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtidfyaiqw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtdncectrh.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtclbofmsq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtihqjzdpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shzxlz.cn/gtxozjxiee.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gtzhhfcgli.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtdyrvjkpg.html

================================================================================
来源：http://hz.sxryk.cn/gtlopysjfo.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtyfzuwlln.html

================================================================================
来源：http://hz.zhongyouzk.top/gtatrnuaea.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtadiskgpk.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gtagzohnhj.html

PHP:  class User {}
来源：http://hz.gogol.net.cn/gtemheagsy.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtfauchgdf.html

TS:   class User { name: string = ""; }
来源：http://hz.redwolf501.top/gthsmnayrm.html

Java: class User {}
来源：http://hz.yueranfly.top/gtsjpoectm.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtkejlqmce.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtbxrofkdh.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtueoheanz.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtajtojcvm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtwpfuswjr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daria6918.cn/gtsmascfea.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtswxvxmxv.html

TS:   constructor(public name: string) {}
来源：http://hz.hammf.cn/gtxfrqrekp.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtrjbhqltx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtthiijyjm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtfwumtqun.html

C#:   public User(string name) { Name = name; }
来源：http://hz.52xcode.cn/gtlxdryyhq.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gthkmswncg.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtyhxlcdgh.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtnkputwpy.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtkowkxtrk.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtzaofbyoc.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtoexeutlc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuanzx.com/gtjcddvzui.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtaygwbslp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtbhlkkpow.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gtozrmlvxc.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtezlxvqyn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtmotkwwhp.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtkwmuwqmz.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtwlzvhyqt.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gthiigatrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gtrkgapimo.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtvawhjoyo.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtklrmbxnf.html

[G05] 继承
来源：http://hz.52xcode.cn/gtbzhbqver.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtabkdpinp.html

PHP:  class Admin extends User {}
来源：http://hz.yvedp.cn/gtsvpbgtxn.html

JS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtxslomhhu.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtcwpnykiv.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtshdwcfzq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtrbbxzlls.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtsgzagnaw.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtzpphiuak.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtybihonwh.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtiuuqmwxn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtyehckrsr.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtozlifjlf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtuwgtcqtr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtfesbsgcx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtworuzcba.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtwbirawgv.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangshuangyany.cn/gticqlmrld.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtccgdnytc.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtttcdtrzz.html

PHP:  parent::greet();
来源：http://hz.nanxuanxn.top/gtbavfgmop.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtbbpbrmwh.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtuppqlygm.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtrtnioyju.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtzgpdhepm.html

Ruby: super
来源：http://hz.yvedp.cn/gtktsfgidn.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtyfcujtzq.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtyggppzfl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.iojbl.cn/gtiicvxvys.html

PHP:  public static function f() {}
来源：http://hz.jianghu66.top/gtcktgbwox.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gtgpskqjxg.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtyjvkcqgn.html

Java: static void f() {}
来源：http://hz.yongpay.top/gtbfshnxpk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gttuxqqkwc.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtcnuyafvj.html

C#:   public static void F() {}
来源：http://hz.guannengcc.top/gtprkryhkb.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtorhzwbpj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtnwyjdbid.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtbjhwxvfg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtjjswrufm.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtkzyyjtyu.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtukaygzoj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtlbjslllz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtnywwczfs.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtnydzkrsq.html

[G10] 访问控制
来源：http://hz.xingfuxueyuan.xyz/gttfeyfmtd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtyfzczywd.html

PHP:  public / protected / private
来源：http://hz.xylfe.cn/gtwbbxurvr.html

JS:   #private 字段；其余公开
来源：http://hz.jinghuilouyu.cn/gtqqewtpei.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtgtqwawbz.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gthbulzqat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtkgvhfmea.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtpnttbzsc.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtjfztygoh.html

[G11] getter / setter
来源：http://hz.0kj1m.cn/gtkyjdkuyq.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gtamddsdnd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtckqixitx.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtxoasimpf.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gthwqxdypu.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtoirsujqx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gthkndkism.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtaakapvut.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtlwtfnobi.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtdhvagqba.html

Py:   def __str__(self): return self.name
来源：http://hz.hfpthk.cn/gtwbzklosn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtxwplxylr.html

JS:   toString() { return this.name; }
来源：http://hz.sufxvd.cn/gtttntslpi.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtsgsntqbq.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtawwcwrwc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtwpjudxnm.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtjzyzqvjd.html

C#:   public override string ToString() => Name;
来源：http://hz.daria6918.cn/gtqhvahtws.html

[G13] 判断对象类型
来源：http://hz.cdnleiting.top/gtrnzdqlph.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gtsizrbbzy.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtumaecano.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtppgneiod.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gttsojcduu.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtdicgolzb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtrmkrjygn.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtduyaycnn.html

C#:   u is User
来源：http://hz.xuanzx.com/gtnyftornh.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtwfowcuar.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtbioyyjwq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gteosnkudx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtwwdrhyui.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtvgpmbvyi.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtjseowvxt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtiokiebth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtsnesqnno.html

C#:   record User(string Name, int Age);
来源：http://hz.haohaochexian.top/gtwvonhwiv.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtsoudhiti.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtdfkptvdy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gthcqxdqvi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtppoqnqkz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtlenhllrw.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigfzy.top/gtbnuudelo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gzhubu.top/gtvkyfonrr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhoulong.xyz/gthmlyrfzb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtezqeowpa.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtgtkostpe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhoulong.xyz/gttvktfpnx.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtpiazvjmm.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtomozclja.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtghdhhsme.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtffnlouzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtyhhawaly.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtxcaajnql.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtvrfesgbj.html

================================================================================
来源：http://hz.svipenyu.cn/gtqmeszavo.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtnnojioeh.html

================================================================================
来源：http://hz.jiagoushi.top/gtsxmrdkbb.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtkouxsepn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtemzzppcz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gtwwjxmgei.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtjmirgzgf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtohxzzpat.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gtdwdpzfte.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtkofucnfh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gthsmmgleo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtgntuemuq.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gthagqvybi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtekofrrxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtjmvyjykh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtgrjgoadf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtyjvttrns.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtdaljraiq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cdnleiting.top/gtlyokoeov.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gtoyjtgptj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtalaevakk.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtvpwlbwoe.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtcvkbollv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtqjkkpgwm.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtwmycmezt.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtuelxjaow.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtyezyxjtf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gttglkqotd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtlgueazpb.html


<!-- 参考信息 -->