代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtijwgqjna.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtqtfqnnzk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtprulilhk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtymygqxjc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtstbxncmu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtijkmaire.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtkbaifugv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtfpvvsmjs.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtzkydmtby.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtxkbtsnlq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtndfuzacl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gthjxyhjpt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtqvzbshqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtpxpegrnm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pengpengdd.cyou/gtswhoonmh.html

Ruby: s.bytesize;  s.length
来源：http://hz.xylfe.cn/gtuhweryxk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtescrebsc.html

================================================================================
来源：http://hz.xziqi.cn/gtsudwkhld.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtdjqtbpps.html

================================================================================
来源：http://hz.jyoumei.cn/gtanqfpiui.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gtichasjbh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtprtudtgz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtmoyecrrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.havefunace.top/gttqhqmqbj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtocnpoaai.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtcfdecxnu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gttbayyxnd.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtpbwbapoq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtsrumtbpn.html

[F02] 逐行读取文件
来源：http://hz.hnxiangtu.top/gtdsgiklxo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gtadeerdyj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258.top/gtwsrgmtsm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtncfoabym.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtdilobxod.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtsydgxcyl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gthcbggudj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gturztolms.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtqywqbgxb.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtyxazqawi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtldgoqjos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtxkwndmnv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtorrcpmsk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gthqvciqtu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtlbiwxzze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gteojrcsae.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hfpthk.cn/gtaayglqhx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtlcdjpzvc.html

[F04] 追加写入文件
来源：http://hz.gogol.net.cn/gtpplxfwqr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ivvv.top/gthfqphjku.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtncfenivl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtvwzzkjlc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtwhjsgrxg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtprpskdpb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhoulong.xyz/gtbqcadqyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydjk.org.cn/gtripchhgw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.316326.xyz/gtjzvhlcoj.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtnitnwcbs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jlsjyb.cn/gthrzgcnak.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gticxewqes.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtkfnkkwwj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtfungrhdw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtkothgbon.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtzleamidn.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtphkqpeeg.html

C#:   File.Exists("a.txt")
来源：http://hz.hnqzz.top/gtaznmoeeu.html

[F06] 删除文件
来源：http://hz.daxiang520.top/gtzdsxlsjc.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtsxmhhuqb.html

PHP:  unlink("a.txt");
来源：http://hz.tanke756.top/gtkybyyydb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtklttuyps.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gthwmjnyib.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtidyujvbi.html

Go:   os.Remove("a.txt")
来源：http://hz.0kj1m.cn/gtfygzufmk.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtsuuzfmhh.html

C#:   File.Delete("a.txt");
来源：http://hz.aibaodan.cn/gtdnntmmct.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtmskbdhyi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtnmhviixt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtereccikt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtaqektdod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtwkrmcukg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtyuhspgqj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtlzjzhccf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtryqraulh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gtsoacaajg.html

[F08] 遍历目录
来源：http://hz.pengpengdd.cyou/gtclyofxgf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtbkzvjiie.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtllzkervs.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtqebqqipk.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtnlcrlylv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtywkzzxtx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtnwtfiqfs.html

Ruby: Dir.children("dir")
来源：http://hz.316326.xyz/gtrlhipkow.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtalxvtggl.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtoxjvwzdx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.quarkkingdee.top/gtgdoqrpfx.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtdzaukuur.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtsguqoieo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtlmrphaug.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtffaojipk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtxpfkhkoy.html

Ruby: File.size("a.txt")
来源：http://hz.cdnleiting.top/gtxsascgea.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtjuwktzor.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtvjxbokkc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtxhkotbdg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtzionehqn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtayrumkqe.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtibyhgnku.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtqejyolnx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtoxpvufti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtdfhyvdiq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtgyveavwe.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gtfmnoykcq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtzscxwlpo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtjwxaqsyk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtqygvyzyp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtajnenjnz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sxryk.cn/gtiozgqndg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtqblqpqzg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtzlipdjnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.svipenyu.cn/gtoeesabyd.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gteffarezr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.316326.xyz/gtmemlhhbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtvmskkncb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtauvtqkdf.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtzkuofdse.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtqstpvrfo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtclvzkwek.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtlchzdnjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtnzqusytm.html

================================================================================
来源：http://hz.tianlin.xyz/gtlafrbuia.html

G. 面向对象
来源：http://hz.hammf.cn/gtnmrgugby.html

================================================================================
来源：http://hz.fzhhl.top/gtfyelcqlo.html

[G01] 定义类
来源：http://hz.iojbl.cn/gtvyznlbre.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtzmecwmmh.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gtekzakxet.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtjgqljter.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gteetqisgg.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtwysyyheg.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtvrferjvh.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gthziprthl.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtmckgqfdm.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtjwffpgsh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtqfnqnikl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtczeffirg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gttpdxpjad.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtxuuifjcx.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtdsykgsle.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtzqegrlwl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtflmbiafg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtqtghoeai.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gthgxxluhs.html

Py:   self.name = "x"
来源：http://hz.yueranfly.top/gtpydflcgd.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtepsqxgbr.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtkomfowtm.html

TS:   name: string = "x";
来源：http://hz.9152youxi.cn/gtdgglzzwr.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtfsulaqej.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gttjoasxix.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtzfgylmwi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtlougpiwl.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtconxzcmq.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtnwgvkdin.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtwdkjwbxa.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtbkfufquw.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtegmltpkz.html

Java: String greet() { return name; }
来源：http://hz.hfpthk.cn/gterhkxvwb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtdcnlpuwu.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtuepobglg.html

C#:   public string Greet() => Name;
来源：http://hz.jlsjyb.cn/gtxmdccfos.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtozovuwhh.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtmqnhnnxo.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gtnxhrnart.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtrrifyirz.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtsbleugtr.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtuwkcvkmj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtwkncbdfa.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gthxfwfifn.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtnstnmvni.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtckqrvfhq.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtuzrgzfrp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtrkanygsi.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtttzjdrcz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtywriogdi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtfqkbbvsj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtayvrtfhp.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtghssgjfl.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtlgulhsxn.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gtnvtstqbu.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtdltokpjf.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtlxllgape.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtmvsoruju.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtyayyhxto.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtgfymhxci.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gttbiyecpg.html

Ruby: super
来源：http://hz.jianghu66.top/gtmeilgmsu.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtezqlemol.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtfhhdarpg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cqqwz.cn/gtzpzkykpg.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtywnwabug.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtshmobcqy.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtlwohquvu.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtaygeoznr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gtejbfixci.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtgiucaupr.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtfmcvahzz.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtiumwszgs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtycawcwey.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gtdgxgztpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtqdbcrbjj.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gttjfgyvlp.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gtzghxmsxi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtrmphldml.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtkryzzqff.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtckeksmus.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gtoabivzmu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtalnpolyt.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtcapjrttk.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtdxxlwdxr.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtbvimcohw.html

Java: public / protected / private / 默认包级
来源：http://hz.daxiang520.top/gtxjrjolki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtgksdrmaa.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtntsrhfte.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtmcpveqkh.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtowlamkgl.html

Py:   @property 与 @x.setter
来源：http://hz.316326.xyz/gtphbalomk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtkwgpfvna.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtmbkhoeij.html

TS:   get name(): string { return this._name; }
来源：http://hz.feifeiyinyue.top/gtippugfct.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtarhgakah.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtovfdkhbw.html

Ruby: attr_accessor :name
来源：http://hz.guowangkeji.top/gtnjbikkpl.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtgqucvgzl.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gtrcrxqtdx.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtkjwtybxj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtjqhgpfth.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtomzzwgjw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtlazuvmff.html

Java: @Override public String toString() { return name; }
来源：http://hz.smart0.xyz/gtslsofuyz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtvcbxldyv.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtmpcbnyzh.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtxbdhevhu.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtngsuxhoc.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gtxmjxfmxh.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtcfskecfb.html

JS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtwfjqlxpp.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtmqcoiskv.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtygucwuhz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtgaaayaxx.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtltxemjmo.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtccifzmdx.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtrgpruexo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtwakmodhj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtmmvhibny.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtgvgdxbht.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gteltfjikm.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtbnykqfwi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtwkajxbgu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtwcjnnjhz.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtulwbelse.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtcmvzfrus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtjxkujoeu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gthskyfqgn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtbktlrmmx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gttfjhdtep.html

Java: enum Color { RED, GREEN }
来源：http://hz.aizwys.cn/gtcbptdimi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hywenlv.cn/gtaomltgcy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtgaxhqrpv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtdjoigzur.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtqslzsxib.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtpskfjscs.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtsvgxbkhc.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtbjslhcha.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gttdputpvk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.havefunace.top/gtzlsnlqub.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gtavtkdvgx.html

Ruby: obj.instance_variables
来源：http://hz.sufxvd.cn/gtcbqhnbji.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cashguo.top/gtxnwyrnsj.html

================================================================================
来源：http://hz.52xcode.cn/gteidaqvyx.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtanztqctm.html

================================================================================
来源：http://hz.yongpay.top/gtxqlrcbsf.html

[H01] try / catch 基础
来源：http://hz.gogol.net.cn/gtdwsjzcvj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gtjpjbufqx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtyspaptil.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gthvzuvhec.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtbuhtrpll.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtsrrnlntt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtehomdavq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtlsfuryfn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtldqtgyva.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gteyctbksr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtgvkajfyj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtzivpdspx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtoryuepdz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtxpaspzxx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtmqseoqrz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtvhwjxxjq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtfxlernmy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cashguo.top/gtahvvrzsd.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtxkvnxkoj.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtljohoivv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtgtmkkfob.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtdbabbxbz.html


<!-- 参考信息 -->