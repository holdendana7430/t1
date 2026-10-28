代发 wailian999

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtztzysyvq.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtvnyjaxnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.havefunace.top/gtmhygjwwc.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtswppwlci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gthlqhbsoi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtqpjefdvd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtedbleakc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtqmhkybdh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtnzaqkpga.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtrverovgj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gthdeejlcp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtrrwydbwr.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtsyjjskpo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtkeldsgtp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtqprlhihg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtziohvlwk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtymgxypca.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aizwys.cn/gtfhyagzas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtwohcfepy.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtwxrzxjry.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtlsduvwdy.html

================================================================================
来源：http://hz.nwbrower.top/gtrmdervoa.html

F. 文件与目录
来源：http://hz.chenlongwang.top/gtcbmcbdak.html

================================================================================
来源：http://hz.fengsongda.top/gtlfuvrlkp.html

[F01] 读取整个文件
来源：http://hz.xuanzx.com/gtllduqbvd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtkjsaafis.html

PHP:  file_get_contents("a.txt");
来源：http://hz.kuanghao11.cn/gtolreyllt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtlsnnfrqv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtravbpiwp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gthrtmgjmc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cqqwz.cn/gtliqqtcdu.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtpervevzq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtsssehbvf.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtwsrxpebc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtywffbrui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtumhzkmrt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtyznasbza.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtphrtgaib.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtoosepgxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtwsxcphaj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yvedp.cn/gtchrlvugm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtqqkpmatp.html

[F03] 写入文件（覆盖）
来源：http://hz.iojbl.cn/gtznaaxbtj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gtugrudflz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtnmkrmrca.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtbwrpvnsd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtaxcilnwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xinyue.icu/gtyparbosa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gteylurezd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinghuilouyu.cn/gtjkenybki.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtdclxxzzz.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtdpyyptrk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtgqaoitvg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zycfv.cn/gtegvgejwk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtprnljmnn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtvowlkfps.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gtcsufxqqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtpzihvvao.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtshmvdwst.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtzhsnjuxx.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtqzfeqbpg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtgcupxvel.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gtqhefqoci.html

JS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtmukqgjhh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtfnazoxzm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtowdxqfjd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sxryk.cn/gtgrvgjvzk.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtanrcytnm.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtnppjofld.html

[F06] 删除文件
来源：http://hz.gogol.net.cn/gtbqyhzlpe.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtoetehiwj.html

PHP:  unlink("a.txt");
来源：http://hz.aibaodan.cn/gtqzckssoi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtzvwndbxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtvhebcdwo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtudqeipoo.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtqpfbpyop.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtsrbfqusl.html

C#:   File.Delete("a.txt");
来源：http://hz.9152youxi.cn/gtkfrzokrz.html

[F07] 创建目录（含多级）
来源：http://hz.svipenyu.cn/gttvjlqxqn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtepxqmzvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gtuaebuibs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtxkyrnpoo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtwzzxjale.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtsonhcxcz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gotoacloud.top/gtnlottnlk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangkeji.top/gtwepkpxhe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtultoltgb.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtdnqbehdn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtfcpamsrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtadnjqdqn.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtxgvxmucs.html

TS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtewdjnndi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtsjwpjucj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtixqcxdzn.html

Ruby: Dir.children("dir")
来源：http://hz.fengsongda.top/gtxrqioeaq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.vqdsnc.cn/gtznjhocfc.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtscpdxztv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtlqspjypz.html

PHP:  filesize("a.txt");
来源：http://hz.yuxming.cn/gtrdpiunwn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gteflppnsn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtxmhfgpht.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtzndxbvtt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gtovqphzwz.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtqjpcqaxf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hywenlv.cn/gtjzwypsjd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtytgbbklo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtcuhtzygg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtnzdjuvad.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtdhnmjfso.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtegghlyzj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtzkkirytj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtbemmklwl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtrsaebekq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtcpjajxig.html

[F11] 复制与移动文件
来源：http://hz.chenlongwang.top/gtggqtdjyv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtgygtfdza.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gtcdqykflg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtpqyycchs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtmxomdnnc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtcbuljesf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gthkglaxec.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gteraflkch.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtzjeeseyf.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtizqahqkq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yangfankeji.com/gtkpivoevl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sweek.top/gtcxuuihlv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtoucvzynz.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtlciwjktj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtjjuovnjk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtjxxkathn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtgzpdshbp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtsmjygdck.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqmckdpfq.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtdblajwqu.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmirjxnac.html

[G01] 定义类
来源：http://hz.pycfn.com/gtbsnldpkv.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtoiorjhxr.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtzanzpfuw.html

JS:   class User {}
来源：http://hz.vqdsnc.cn/gtqhzkezqm.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtiskvcikn.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtbykhrfpe.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtfcfzshkl.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtqeyercvu.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtcixoaxdp.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtjtnbqhvb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtlczitzcf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.kuanghao11.cn/gtiekgtrsu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.mhx1999.top/gttepcgpiz.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtibrdvjpz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtfejsmngm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtnpjalokd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtihpdiqpj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtjdzlorgd.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtgxivzdlv.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtxtqcsnep.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtwtkqqunt.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtwqibmcse.html

TS:   name: string = "x";
来源：http://hz.vqdsnc.cn/gtlweefocp.html

Java: private String name;
来源：http://hz.xylfe.cn/gtexcwsbos.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtqvrnusef.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtofpdowcd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtabvdqvkp.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtrlrnmsdg.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtcyddsbgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtdubcoebo.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtwbmsvpwd.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenlongwang.top/gteppdsnhx.html

Java: String greet() { return name; }
来源：http://hz.meibo888.top/gtcpsfobcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtzxojuflm.html

Ruby: def greet; @name; end
来源：http://hz.shangyingyoupin.top/gtllotbwnw.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtvytfimjl.html

[G05] 继承
来源：http://hz.tanke756.top/gtegonplls.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtyhbgyhkr.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtbhhojnuq.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtmuvyobcs.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtxlxbxobl.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtlioayexz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtwygjrnjt.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtsxxgkqxf.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gteypokyys.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtcsmapbqh.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtfdydpteh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtyecfpmfj.html

JS:   greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtqilmhfnf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtunhuniza.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtqyaclawn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.meibo888.top/gtwezbqwpr.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtaevikstg.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gtgdqaqijh.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtzdavnqam.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtgqcefnlm.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtudsaitwm.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtzycgaqnx.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtmrhwsczd.html

Java: super.greet();
来源：http://hz.yanxiufei.cn/gtbnrxxmhe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtzndmcgcu.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtvnyrmluv.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtrluzkkeh.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gthixbyvao.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtrklmhsdw.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtjeqvquya.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtcebmcwzs.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtxctfjxir.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtmhkanngv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtgoifgozi.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtpmdfxdfq.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtdazecxil.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gtwqkkkrok.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtnvpznjyl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtevitmsnw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtrmgzvwip.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtsvhjjazc.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtnqkvvwla.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtvlokldnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tanke756.top/gtziebjmdf.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhijiandao.cn/gtoawojmak.html

[G10] 访问控制
来源：http://hz.feifeiyinyue.top/gtogezzjsu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtrhxrluor.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtuwagbmxu.html

JS:   #private 字段；其余公开
来源：http://hz.zhiwuduotai.top/gtdnryqmhk.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtxzboacnq.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gthhkitapu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtvtezdhfz.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gtnpiudhaw.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtncehflbt.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gtawodtkfo.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gtseoecmqd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtsglbzcmp.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtvjeentlf.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtrzylayib.html

Java: public String getName() { return name; }
来源：http://hz.jiagoushi.top/gtaazgdeow.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtfplurbgn.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtfloonisv.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gttntlqpam.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtncrfxmda.html

Py:   def __str__(self): return self.name
来源：http://hz.chenlongwang.top/gtsqisqzgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtlwvftxex.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gtjbtbgmhx.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtnzaynjni.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtxfoigbia.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tian-w.cn/gtztbnltnl.html

Ruby: def to_s; @name; end
来源：http://hz.birdmap.top/gtsdmlihew.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtiohxefph.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gtltedhdcu.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtpkxbicqe.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtbjncvdqs.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtadvnxuhy.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtqfelewua.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtdeqilcyn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtijsjwuwc.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtflgagxds.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtbxzktata.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtycnuzovq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtwrektlie.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.0kj1m.cn/gtziafdovp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.smart0.xyz/gtjbuxjijt.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtktghyziz.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtrywlzzic.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtlrduwcdx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtbvzjbgfx.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtxwoknmvh.html

[G15] 枚举
来源：http://hz.fengsongda.top/gtcjunueer.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtcnapmves.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtbuyitjmf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtmcktpwkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gthtnmftph.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtlaernqzm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtwxxupgyc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtnobzqipd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtbscrrswm.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtgiaqbtpb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtulziohhf.html

PHP:  get_object_vars($obj);
来源：http://hz.yanxiufei.cn/gtbfxckekw.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtpjpkabmn.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtmvftxcav.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gthqqgtvid.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtgbeoxwks.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gthauoygyk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtynqfmsmo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqslwetjo.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtcazqdzdm.html

================================================================================
来源：http://hz.ivvv.top/gtducgsdra.html

[H01] try / catch 基础
来源：http://hz.hnqzz.top/gtlcswszps.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtrgixsefr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtyzdrsjfz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtuvbywiye.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtibhdrgun.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtqhkvgdgv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtoakwdooi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtyyorbcmu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangkeji.top/gtfjtxrolr.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtfpztzkpy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtwdocvavl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtlmrgbktq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtbpuahxer.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtakkcykhw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtwvzwbprg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtlhppgced.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtzizqfmol.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtuoslkczr.html


<!-- 参考信息 -->