代发 wailian999

Go:   if s == "" {}
来源：http://hz.jinqigfzy.top/gtpobkyhtn.html

Ruby: if s.empty?
来源：http://hz.ywan-chungtsiang.top/gtsjvktlmo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pycfn.com/gtkqyympqf.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtwikebptl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtodblfwjs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtdnwvvxzv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtqtxgwjpj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtiqxmphkh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtmaicpzre.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinghuilouyu.cn/gtiydtrxkd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtubqohozb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtvdawjika.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtnoxcshgp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigufen.top/gtbuxhdbuv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtqwhwwdrq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtnvlgnnjp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtatchiatz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtuvwalngg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtvieiexsk.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigfzy.top/gtvppyxfoc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.52xcode.cn/gtuevgsxxw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvnqhpcny.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtakvebpgb.html

================================================================================
来源：http://hz.bjfxy.top/gtttqpvkox.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtopztnwtf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gtdcokgklj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtfhshcoql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinghuilouyu.cn/gtharbjnno.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aibaodan.cn/gtbcmfxlln.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtpnpmknxw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gttnzywzxc.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtppfarmub.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtvohfmalo.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gthkudbbwx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gthzithnpi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtpycxibft.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtrdhrcbbu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtfqhtwbxy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtyhkltnqq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhaomingkeji.xyz/gtdeamzdal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtmffxjcev.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtegapymkc.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgfzy.top/gtsdkitlek.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtcftumhfe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtdtcjrstg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtyskqdrxn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtogzkjtly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtxyvutunr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuanzhike.top/gteszfgpvw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtclelxubm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gtqgszpmps.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtazzewbmv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sweek.top/gtvfqursoz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtjlqphzck.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtbtzrzcox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtkeyyzney.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gtqgrnlovg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jianghu66.top/gtmspycdbk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtybiaofqg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtqhmzhluq.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gtvsvoxqih.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtzephrhcl.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtuoktowph.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtgjvqbwfr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmzwakuog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtrrkucxwn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtuvtzstli.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtutdpwtus.html

C#:   File.Exists("a.txt")
来源：http://hz.yuxming.cn/gtzfbzbmaj.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtcnnxalbr.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gtlkiahiwc.html

PHP:  unlink("a.txt");
来源：http://hz.fengsongda.top/gtnhwqiwfa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtfemlpfrg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtyigncfso.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtedybfdgp.html

Go:   os.Remove("a.txt")
来源：http://hz.jinghuilouyu.cn/gtptpqufrm.html

Ruby: File.delete("a.txt")
来源：http://hz.dianchejie.cn/gtiddmrsms.html

C#:   File.Delete("a.txt");
来源：http://hz.havefunace.top/gtcvkxxlor.html

[F07] 创建目录（含多级）
来源：http://hz.cucudq.cn/gtkkpjjndz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtiqqccyce.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtxhatdayn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtmdbeksjw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtctlirkma.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hysaishi.cn/gtbtjbgtrg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gtfbjifmdl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtgbgxwoxh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.birdmap.top/gtuydmrkup.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtzgzbxpwf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtjhuwmfbi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuxming.cn/gtjdsebdfm.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtdmmdyqch.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtmuoutmrq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtzyacrlfj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtbkdqnxqw.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtonrofvld.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtgxjzlpxe.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtfesvtoos.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtqylwvtny.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtiowxmihx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtfgvzptjt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtilhxcdun.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtrmleqkak.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gteydmgcii.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtpzbrofnc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.havefunace.top/gtqlchgyro.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gthjlfntlb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtskmzskxd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtensllmch.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtnvjsmdah.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gtdfyivqjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ybcxt.top/gtymbxmzoi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtxmefmlza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtnbttthpe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtiqtgvtmb.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtlwxvrgcf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtqnmgslti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangdashe.top/gtrpavcyrj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtfdlotcfk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtlzrtcuue.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtbsqpwieu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtqwkssiwb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtxmqbsdpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtlrtjxlpx.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtrsvbdslk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gthvqlmuuq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtqrrqssaf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtibhnaudz.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtffjyhvbf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cdnleiting.top/gtzntyfpjw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtbkkvwaex.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtflovuesi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtnogrfxec.html

================================================================================
来源：http://hz.jqgufenzy.top/gttlsuxywg.html

G. 面向对象
来源：http://hz.xziqi.cn/gtbrqezllq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtltzujjkh.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gtdhruortt.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtkijxftyp.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtgnmpskod.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtiiaqbxsn.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtuwytjuev.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtosxiibnk.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtgkykxqha.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtizalaeqs.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtjololsgh.html

[G02] 构造函数
来源：http://hz.cheryme.top/gtvuymytmy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtiobaptxx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gtaklwzprd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gttrdywtiy.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtobhrssoz.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gthlsdqxau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pycfn.com/gtpwcukthk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtaxqebbhr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gtmzrbsggf.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtwqnyttik.html

Py:   self.name = "x"
来源：http://hz.hnqzz.top/gttckpopms.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gthmylzbhf.html

JS:   this.name = "x";
来源：http://hz.haohaochexian.top/gtfhjhmqwl.html

TS:   name: string = "x";
来源：http://hz.yueranfly.top/gtqqyvasmi.html

Java: private String name;
来源：http://hz.iojbl.cn/gtmfzwfthg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtjrcqblwv.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtjcnemzkx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gteskvqglw.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtvqxungje.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gtzhommsze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtbdymzlml.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtiwwywpcj.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtmcrhqgiq.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtsbkezbca.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sweek.top/gtajrzedmv.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtswnzbxnx.html

C#:   public string Greet() => Name;
来源：http://hz.vqdsnc.cn/gtrqvobexh.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtuuvkmbwn.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtkpqfhvcn.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtaruyigzi.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtzrgybdjq.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtlcaperye.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtqrleqngc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtprdeismz.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtyhfmtpme.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gtznlncpzo.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gteqpkfydo.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtvuisgivd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtjwvodpbv.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtzkpscbux.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtqpllryty.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtzkpvljmj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtuhyycqae.html

Ruby: def greet; "admin"; end
来源：http://hz.guannengcc.top/gtyuwonxiy.html

C#:   public override string Greet() => "admin";
来源：http://hz.dashuyun.cn/gtuyunwndn.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtbfilvsrj.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtxognucls.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtdhjihrzi.html

JS:   super.greet();
来源：http://hz.zhijiandao.cn/gtcswlzmgl.html

TS:   super.greet();
来源：http://hz.ehwqpu.com/gtwfvqixls.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtknnwhrlb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtaozypqad.html

Ruby: super
来源：http://hz.tian-w.cn/gtvspckyms.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtuccbohuz.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gttzdxhbhu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gtmgzzvbgq.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gtltbpuiiz.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtixreqpgs.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gthvybyoxh.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtawveouom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gtgfltukxp.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtaxhysxvj.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtvallyrtf.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtgjpjbjcb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtauxllzug.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtfpfujfwr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gthljlzomv.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtmsdtoxuc.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtebbvfyyg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.quarkkingdee.top/gttjejapwx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtbewvvykp.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtvhnzgoop.html

[G10] 访问控制
来源：http://hz.smart0.xyz/gtxnejvwbs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.meibo888.top/gtviolpmcf.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtnqrycwqj.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gtckwpuwut.html

TS:   public / protected / private
来源：http://hz.jyoumei.cn/gtjlgujxnb.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gtyvflphtz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtkabxfjuo.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtmcgncprv.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtfjeedpvq.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtcinabcnl.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtabcqizjo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtjvcutxpu.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtinyhmiyk.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtggtkmzhp.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtjfhhavus.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtxbqrtzbw.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtrgyyrxyt.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtfqcgerjp.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtuoflsufb.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtnesidwyi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtfpxqlgxy.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtbfpjtavv.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtarowialq.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtetviwzsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gtmykmgslt.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gthvkmnoce.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtiivlqxri.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtuqfiaawx.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gtxgvlowfq.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtfuqpudqz.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtwemzdttd.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gttawqvtmj.html

Java: u instanceof User
来源：http://hz.feifeiyinyue.top/gtzwsfogqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtzstmitfa.html

Ruby: u.is_a?(User)
来源：http://hz.zhongyouzk.top/gtrsnvlbml.html

C#:   u is User
来源：http://hz.birdmap.top/gtulenslek.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtbclzjqgs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtagbbqcdb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtjhsjghxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtbdqvazzc.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtowjwthao.html

Java: record User(String name, int age) {}
来源：http://hz.ybcxt.top/gtujoelekv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtumvmhnus.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gttrizrijs.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtzqmnwaya.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtnvqzfcdt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtbikupgyi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtgdejkyry.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtftjdxssw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtdrpdovlx.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtqkieypzo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtdafzmnen.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtbtilhxau.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtikqytzer.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtojlupcdb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtskgqizvc.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtbvwzysbu.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gttowbxhor.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtsfeuuumj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtlqtttvbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtjrwfqtqc.html

Ruby: obj.instance_variables
来源：http://hz.feifeiyinyue.top/gtlvvtqqap.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtgbbvmfdt.html

================================================================================
来源：http://hz.316326.xyz/gtcqvkqjlt.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtivmcrkfs.html

================================================================================
来源：http://hz.ppjwa.cn/gtltmndqth.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtdizedzyd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.meibo888.top/gtbpjrwjyb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtoltxkdti.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtcnzeatfy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtubachysy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtkdkxerzr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtujslqsmb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtjahcifzm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtczjemqdg.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtlwaasqaw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtopvutnlp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtjojqqjce.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtuuydmiii.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtwltegzvb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gteaoxypst.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cashguo.top/gtvbqnxvtb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtgdxrveyb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtkzmpdcpt.html


<!-- 参考信息 -->