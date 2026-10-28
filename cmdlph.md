代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gthvgvslzb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtshwiwwji.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtotnrzqgq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtctvdzjls.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtdilfjesi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.quarkkingdee.top/gtlznbclzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtuhodtznh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sysykeji.top/gtvcrlrwxc.html

[E22] 字节长度与字符长度
来源：http://hz.dashuyun.cn/gtmekyupsc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gthnstxqsq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtyitfpncu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.9152youxi.cn/gtidjkqqts.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtmgkwmces.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtqxheqgnq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtbualecnj.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtdhgmuerx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fzhhl.top/gtneizrvxh.html

================================================================================
来源：http://hz.bjfxy.top/gtempnxtjw.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtolfjcgdy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgkacenox.html

[F01] 读取整个文件
来源：http://hz.ybcxt.top/gtupgyrtib.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ivvv.top/gtplyueugf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtbttgxehu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.svipenyu.cn/gtzdfikuoh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtcrghbczt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtvyeumwpy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtftuomnfw.html

Ruby: File.read("a.txt")
来源：http://hz.xylfe.cn/gttdcpbsyy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtcczdoknm.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtgusfwiem.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtkqabrsgx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtxeenaxvv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtowrtudff.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtiloewlcb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtgtxwembt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtdhirrfgw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.kuanghao11.cn/gtjgpykuhz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtydmgejrm.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtwodtmwjy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gthxltatwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtvznbeuxv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtmljejuyv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtrlkcjhsm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinghuilouyu.cn/gtuogkrjrb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtcaqcjibz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.0kj1m.cn/gtarabcunq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtqedwbqnb.html

[F04] 追加写入文件
来源：http://hz.mhx1999.top/gtzbqjhqwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gthiiynnza.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtpybiryqc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gttmlkltzl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtwwiutmyz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuanzx.com/gtzqpypukv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gthrigjvei.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.birdmap.top/gtlkgyxsiq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gttfnhaoxo.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtmqlsdyrv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtzjsmtldy.html

PHP:  file_exists("a.txt");
来源：http://hz.hnqzz.top/gtqsqvvrbu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtmeaqtnsq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtldnvgono.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtefqzetif.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtfplwmlab.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtmobmxhxt.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtvrhnjpxl.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtzwoauwrn.html

Py:   os.remove("a.txt")
来源：http://hz.ybcxt.top/gtxofhyhbf.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtgnwvjffh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtcdndgvvf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtnubozpet.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtysdxjwyr.html

Go:   os.Remove("a.txt")
来源：http://hz.fzhhl.top/gtvzadfycx.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtvmolphfs.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtzpzxojus.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtlcsglwwr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtaollifin.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydjk.org.cn/gtrwdslhgh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtmtamelcy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtptebgmuq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtfbrzpznw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtycfmbemd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangkeji.top/gtvntobqwu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtvuxhkiec.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gtvyjaxlte.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.havefunace.top/gtzpawplma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtparnaugg.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtyxagidrs.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gthejonnxp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtvwqgnxph.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtgbibrykk.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtkdblwgia.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gticxbsrig.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtkaoefpux.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yonumen.top/gtovuzhnbp.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigfzy.top/gtpidxejmt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtoynlgixb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtlcjdubxa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gthzlnjdll.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtnapdided.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtjqgtvrwy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtvyzteqrc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cdnleiting.top/gtnzaazyna.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gteojgkvni.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtmqewwqiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtomdoloqa.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gthnrklvtu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gogol.net.cn/gtfifuvmxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtbbkzhzul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtbcjcxcpq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gtwzgrjdne.html

[F11] 复制与移动文件
来源：http://hz.wangdashe.top/gthmiojswj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gteonzlewj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtrzdsibbh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtetreegil.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtcsplpfnk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtnsfukpmp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shangyingyoupin.top/gtiezpiown.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtckbgqlmn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhoulong.xyz/gtzykzuubz.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gtzrxftjee.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtnzharmzp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtjjwhhktc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gthofrgwlx.html

TS:   // 同上
来源：http://hz.zycfv.cn/gthjnocawi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtnohcudkx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtbpspkslz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtvyaatxns.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gturkayxfv.html

================================================================================
来源：http://hz.nanxinkj.top/gtnrthajsg.html

G. 面向对象
来源：http://hz.svipenyu.cn/gttqoluesq.html

================================================================================
来源：http://hz.zycfv.cn/gtsredxqvs.html

[G01] 定义类
来源：http://hz.sxryk.cn/gtsxosvraz.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtcibqebjt.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtkdfevvid.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtisgflarw.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtywbfxllp.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtvtwtlkag.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtnszlleaw.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtpbhaejli.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtsgfvzpya.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtvxzhsevk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtvzeiyyxm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtxdwqsyhn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtzmjwjewp.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtpzovjnak.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtcmlflzof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtslcifgby.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtxbjnzdvr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtrdusrcjs.html

[G03] 实例属性
来源：http://hz.svipenyu.cn/gtpichgimq.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtejwssljo.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtjddibcqp.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gtppcfwgjh.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtclsbyhuk.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtmhtahqso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtrwjidyxn.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtbhmdlwcn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtgygtyual.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtjsohmsam.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gtcnsihamf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtnzfylbhx.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtibplywez.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtvhiyykyq.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtmldhalfl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtdgbpkkhn.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtojkiasga.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gtoupqjzce.html

[G05] 继承
来源：http://hz.redwolf501.top/gtehmjjard.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtydsnlbhf.html

PHP:  class Admin extends User {}
来源：http://hz.yuxming.cn/gtkujssirz.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtcxfxqajs.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtwetyeshh.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtoghnkftw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtvaohbzat.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtxnjippct.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtnuhshfrk.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtrfxqgtoc.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtzhzvkzvd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtfkiexkno.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtjktjvzcb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtzwfisgqf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtwibxqqdl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtfpojnsqw.html

Ruby: def greet; "admin"; end
来源：http://hz.ywan-chungtsiang.top/gtchawitoi.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gtmknjgcdu.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtswuhykxq.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtlhwbudsn.html

PHP:  parent::greet();
来源：http://hz.mhx1999.top/gtkylzdimi.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtwezkdudm.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtbjmzpwfo.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtsixvpqlr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtyfiuxdag.html

Ruby: super
来源：http://hz.xylfe.cn/gtmeiafcch.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtrdqgwxdv.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtyylggidr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtmektparx.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtyvgfjaij.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtbiyfzuii.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtgjcvgsgj.html

Java: static void f() {}
来源：http://hz.jyoumei.cn/gtvbucftxx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtkeyfpgpi.html

Ruby: def self.f; end
来源：http://hz.zhijiandao.cn/gtwojfspic.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtgaooviak.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtldmyhggj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sweek.top/gtlziqwtyj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtufmvdtld.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtluspgzki.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gthnnyltki.html

Java: interface Shape { double area(); }
来源：http://hz.hammf.cn/gtkwjhuidx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtcarzkioa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtdpjvtfcu.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtqdcizocs.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gtvllajjvs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtfkknpksy.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtigneffnt.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtlanuxsnm.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gtbgbkswlq.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gteyzlqcjz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtsfxjkglp.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtxhytaijh.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtnwieqarv.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtkoqsourl.html

Py:   @property 与 @x.setter
来源：http://hz.xylfe.cn/gtehwhvgwh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtzmwnbygt.html

JS:   get name() { return this._name; }
来源：http://hz.guannengcc.top/gtmfelfoyw.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigfzy.top/gtffojlcym.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtbshxwecc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtgytbnqyi.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gtrjidyrdz.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtongewxke.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtvtclhelr.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtldhaauxc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtjthgnbjf.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtuxyudsrp.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gthryojexk.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gthmkrheor.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.316326.xyz/gticediurb.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtbhkxtgxs.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtlzisozzq.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gthqjibsrl.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtxszinzrs.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtjlcrnzku.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gtzyqhwmgz.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gtoxkrwlyh.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gtoxmrspaa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gttcdxoqfc.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtujkigcds.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gtrreimfmk.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtsqivmngs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtxiyydovg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtjffiyzux.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtktagvqjd.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtksnuibpu.html

Java: record User(String name, int age) {}
来源：http://hz.zhoulong.xyz/gtjbovuwud.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtecuaxzuz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenlongwang.top/gtkgcbgehx.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtsftoomkb.html

[G15] 枚举
来源：http://hz.zhoulong.xyz/gtirwgzjcq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.haohaochexian.top/gtogybtzrl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtnidwoejy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.iojbl.cn/gtrlzphodz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtqxmfpiof.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtwbjllmry.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtaqywzguq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtrcnrwpzw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gttrlxksbh.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gtzzlibwao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtomggiqaq.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtrxewoqai.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtynunchrp.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtgdfucjnu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtsedlccdh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtxgaxcqhn.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtcrxnlouw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtfbqajeut.html

================================================================================
来源：http://hz.haohaochexian.top/gtyppwmjiw.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtqeiavdif.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdocroxkk.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtqueognqy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtrcvatyvw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhijiandao.cn/gtepatkgrl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtralhnycd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtyquzjyuy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gttiidfhhn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtpyjypzwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenjidiqi.icu/gtshlfxrgk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigfzy.top/gtmxsshbkj.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gttuxfvzdq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtyebdfgyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtdkeivemu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtibooafrx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtrrsllulx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtqnmsacsi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtxdsxgvkt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pycfn.com/gtmeactrsn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxinkj.top/gtzkqvbrxp.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtrjnwnavm.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtenbzjuui.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtvbjxmqam.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtamxquqsd.html


<!-- 参考信息 -->