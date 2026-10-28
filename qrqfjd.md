代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtamuwogyy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtrnoqzcrr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtrgxrohoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtqaixypsa.html

[E22] 字节长度与字符长度
来源：http://hz.xingfuxueyuan.xyz/gtyjyjpirv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtqvxoxxlc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtzpphboso.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtzjwfoglp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtsmeoctzh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.havefunace.top/gtqfajwsxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtflpdornt.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtbcrkgwnx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtcyttlbbr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttatpvtyl.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtxwwdkdjg.html

================================================================================
来源：http://hz.jinqigfzy.top/gthuycfodz.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtrsqgqtay.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sysykeji.top/gtrxygnttb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtdskzvxim.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtzpydyvxp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dianchejie.cn/gtjreghtak.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtyijotktf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydzc1.top/gtnwqtibqr.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtglwqrnoc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtmykjbuco.html

[F02] 逐行读取文件
来源：http://hz.fengsongda.top/gtwikdclfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtfbdaevez.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtxapqzaqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtdtqvobst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtlroxlocl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gttngxdwxv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtywharevw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shangyingyoupin.top/gtqxhqhkzw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gtpynyipik.html

[F03] 写入文件（覆盖）
来源：http://hz.zdqjudy.top/gtlnatpoqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtqkfznbeu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtynmfdteu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtsgtatytl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtuykvamck.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtaapatzzz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtvebmodly.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.haohaochexian.top/gtnxenrnnx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtaffhzpon.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtekdzurpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtxpdbfphu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtsldzxybs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtqcvlqvdi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtdtztmqgl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dashuyun.cn/gtqmtavjgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gtpxtqhbdk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtlqotiotb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtlusnzdko.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtujzgsers.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnqzz.top/gtguzytjse.html

PHP:  file_exists("a.txt");
来源：http://hz.xylfe.cn/gtzryioxun.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gthvbnigdc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gthgfdcmxb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtzrsafemv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fzhhl.top/gtzphxhaam.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtjkpwoebm.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gttkgamyis.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtwswxelqy.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtebbfnewc.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtpnlvxxmu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gthcravptj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtmuwxwxfi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtbsoydbec.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gtxpvurukt.html

Ruby: File.delete("a.txt")
来源：http://hz.cheryme.top/gtokoycswe.html

C#:   File.Delete("a.txt");
来源：http://hz.jlsjyb.cn/gtcfairvmk.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtumoxkakf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtdelbqcre.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gttbuqmdck.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtptjnkdca.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtkkcwqmeg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtstkiivbt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtvvaefxld.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtwcvclcdf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtihedtpmp.html

[F08] 遍历目录
来源：http://hz.jlsjyb.cn/gtppueupyv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fzhhl.top/gtsioalfuu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtcgxsmgap.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtrqalvicl.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtxlbkhqin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtiqeefuog.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtmailfqwl.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtujoguisi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhaomingkeji.xyz/gtlzwiulzn.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gttyotlutq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtssqbvaah.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtnxyyeemg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtbbeawske.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gttxoxxpgt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gttwxozzal.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtbfibwnzb.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtmkpsetrl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tian-w.cn/gtewrbojki.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtwmcqckgk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtptnheoyd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gtcrtwsugo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gturagjfyr.html

TS:   path.extname("a.txt")
来源：http://hz.guannengcc.top/gtyseoyerw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtdtzorklx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtbojnxkto.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtnyhxppwj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtndlhvbsb.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gthrecybru.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtnvfstkna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtjcnorhtu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtkwdmwrwz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtdytaujxc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtmgbxhduu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtziudccwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtdktwgraf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtqxgznsig.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtykpoozfc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtmbhieyyf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gtqcgewuxb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtspwgkggd.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtochakvpb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtqctexcfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnxiangtu.top/gtzbgswtva.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtihkaleie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gtfnsautxn.html

================================================================================
来源：http://hz.jyoumei.cn/gtbsnrknwb.html

G. 面向对象
来源：http://hz.yongpay.top/gtaxiycrpk.html

================================================================================
来源：http://hz.cucudq.cn/gttolswpix.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtwqjoewfh.html

Py:   class User: pass
来源：http://hz.hysaishi.cn/gtkxvzgynb.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gthwfqcubj.html

JS:   class User {}
来源：http://hz.316326.xyz/gtkbydslxj.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtzciakigj.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtsefjsrnj.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtwnldhcph.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtdrgpnilt.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gtogkjsrry.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtpewvgomm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yonumen.top/gtrzebmtgy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtuahnmswq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtbtfxizbw.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gthkjiufeo.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtzlpkmwzg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yangfankeji.com/gtkkmbrelh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtrnktrcbu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtikhlqizn.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtjtyusjqe.html

Py:   self.name = "x"
来源：http://hz.cucudq.cn/gtqbhfwedn.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtneucjpvc.html

JS:   this.name = "x";
来源：http://hz.svipenyu.cn/gtacvaldrj.html

TS:   name: string = "x";
来源：http://hz.yvedp.cn/gtcgzymurp.html

Java: private String name;
来源：http://hz.yj20258888.top/gtdiqurfuh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtoufzarpq.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtjlvdkzuu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtvmrkiwie.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtsbpmbbmh.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtekyqxodu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtpavxpnxc.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtmawvmqgu.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtdvcmiipz.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtjerdpezg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gttrlcwpwu.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtrlgkadtg.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtyanmnadn.html

[G05] 继承
来源：http://hz.316326.xyz/gtbrxaeami.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtaqkeqpzx.html

PHP:  class Admin extends User {}
来源：http://hz.aizwys.cn/gtcgjzucqf.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gttumyynhs.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtwqjroreh.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtzbswpvwn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtiwmxbrkf.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gttzoqzfjl.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gtbhqfcetv.html

[G06] 重写方法
来源：http://hz.cheryme.top/gtznjskimu.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtwgsurrpy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtercqbnma.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtrqdorvpg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtevauyycm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtgcypulyt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gtfdmxagmz.html

Ruby: def greet; "admin"; end
来源：http://hz.xylfe.cn/gtaflavxdn.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtqxkfdkrg.html

[G07] 调用父类方法
来源：http://hz.dashuyun.cn/gtbprrqumd.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtcqqvnfjz.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtdchnkyla.html

JS:   super.greet();
来源：http://hz.yj202588.top/gthmypdrot.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtxtooeoor.html

Java: super.greet();
来源：http://hz.cashguo.top/gtmjxulvpa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtvdcngvcd.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtruahkxdx.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtrhelmlga.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtbqysojxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtdbmyptvg.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtdwetwxrv.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtzootyeyq.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gthhcjltqr.html

Java: static void f() {}
来源：http://hz.vqdsnc.cn/gtjzhxqhue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gtboejrmiu.html

Ruby: def self.f; end
来源：http://hz.haohaochexian.top/gtigvyvklm.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtgvwtelhx.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtkyetbwsd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtbpalyaxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtipqwyghc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtwgneraic.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtsdqyyryr.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtpnlyomgi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gtmekxqefw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtwxgpjyqt.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtztcxxcvb.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtadsuhkzc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtsxxezodp.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtloytcyqb.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtwvpyawgr.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtfiqadygn.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtvopzprzt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtnwvkyeko.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtitiighth.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtmcygsnej.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtjaircaqs.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtwpbgqgfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtmaxxigdg.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtagdjcgob.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtxmaxuuho.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtucoizgwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtihijimqw.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtthrmxgxf.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtskjlbghn.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtrvejsest.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtemqgcyjj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtbwnupfbq.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gthymritzd.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtschekbum.html

Java: @Override public String toString() { return name; }
来源：http://hz.smart0.xyz/gtlmsunpbf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtsruogxkg.html

Ruby: def to_s; @name; end
来源：http://hz.zhixingplan.top/gtgnbacxel.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtkxofkqce.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtkbveiwhl.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtvofjqatr.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtefkrhnnq.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtdhjdoktw.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtrxxpdipd.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtimccbyvu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtcabtwazm.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtorgbbedo.html

C#:   u is User
来源：http://hz.daria6918.cn/gtmdymahxt.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gtpkneeqso.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtiyxcjnyx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtfjverlxw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtewndrwdt.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gtjcfolaae.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtiviswixs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtfdvyuxhg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtxirjirtb.html

C#:   record User(string Name, int Age);
来源：http://hz.yongpay.top/gtuxxrbmrs.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtrhzjtmia.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtbxvijwxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtnxerxvsw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gttekfclru.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gttqxbuntl.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtnpswdujj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtickiucez.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtqmlmveup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtsofivppm.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtjejnefwy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtpckkvhfp.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtbykflwrt.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtmvzgwbvi.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtypytttxd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtfhoqgpop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.9152youxi.cn/gtpsaopfhn.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtvcgvnilv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gttgrzzsyb.html

================================================================================
来源：http://hz.chenlongwang.top/gtfzqhejlr.html

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtpbuzmixp.html

================================================================================
来源：http://hz.c1oappe.top/gtofzquwgc.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gtgvszgetn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtotwqqvei.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtepwtcqin.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtuuzvbwnq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtqblxzaqg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aizwys.cn/gtdebdeywp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sysykeji.top/gtggkmhyhf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtyqnjfgjo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gticynbaxn.html

[H02] finally / ensure 收尾
来源：http://hz.wangshuangyany.cn/gtgfvyioiz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtrgstftvz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtigqthujk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtheyrihtl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gttqfdzsfv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtaenmdiww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gtxwcbcfsy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtynwcvitc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtdligulxd.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtgaxgvpec.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtzqtgkdzt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtvbvjhgwa.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gttxqerqhg.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtpjwxvwnm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtxpefzlvm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtacojqmse.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtvepdthdc.html


<!-- 参考信息 -->