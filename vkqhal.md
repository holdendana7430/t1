代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hammf.cn/gtjzbkpdnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gttuwkurnc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtzhuqbhes.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtxroskwxq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.havefunace.top/gteqksyllc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuetiantiany.cn/gtrxkyerfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtrdivhdia.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtslqgvijv.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtobuksaxl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gthuvtiifr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtirxyrehs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtjzjjiqjo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtjtcrgcsf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtzkzemqnu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cucudq.cn/gtuxwxokkp.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtphegupyr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtetngvtay.html

================================================================================
来源：http://hz.sufxvd.cn/gtjunwofls.html

F. 文件与目录
来源：http://hz.yongpay.top/gtfvkndgnb.html

================================================================================
来源：http://hz.jiagoushi.top/gtfvxxjhjs.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtkkmhimxk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gtmbdqgasd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtpiappzjd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhiwuduotai.top/gtokcisiwc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtagcasymn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtkelwpwyo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtyfgbrpgh.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtiyfemfdd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gaohongyu789.top/gtamdktjdo.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gtqxqysuta.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtjevbwaoa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtfjwvrcod.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtwofcscxg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtlyfdigzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtkufhsdph.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhixingplan.top/gtrjosjjhq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zycfv.cn/gtqoblqcky.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jiagoushi.top/gtqpgzvnrz.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gtmhceggfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gttqqgftse.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gttollgtmw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtnjgokmxg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtsiwpallj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gthkzeetyz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtgljjzkze.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtdskkmqch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtprtoufce.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtsnhjhsih.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtmkhumgxi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yonumen.top/gtbdqbbhcm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtpjplblkn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtbrpoyfoz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtutkbqgkq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtlzrzaxuy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.quarkkingdee.top/gtxlxktnvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtdkdeugmh.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtcqzdffws.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.bjfxy.top/gtfuuhapba.html

PHP:  file_exists("a.txt");
来源：http://hz.cdnleiting.top/gtltinqzwd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtwjyalpab.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtmkbtpstp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtvsotcsah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtfwvjqiyj.html

Ruby: File.exist?("a.txt")
来源：http://hz.ybcxt.top/gtxsagndsm.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtzmnlppks.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtnfstpfko.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtuitwwzhw.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtgiybkqwn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtehbxshfl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gttpxnrotx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtypugjtab.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtdywkawsd.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtzmbmzntx.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gttrpcarub.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtuzusihtu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtbhfcqqoy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtixqbbhmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtrgpogptk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtzvvhfcqh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtapmaemac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtsunsfdbw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gttcpmmcfd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtpotvzsbo.html

[F08] 遍历目录
来源：http://hz.pycfn.com/gtdspknojf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gtyvtjjsig.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtqjlggnoh.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gthgdqtdls.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtibsaijdn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtinwevkos.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gtcktuooiv.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtsxegoivo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtflugzqbu.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtrnjjgbbi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cqqwz.cn/gtkbyhrqvr.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtdyvuqkrd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtgxmjldbz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtbwrkhjoq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtopdjrqij.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gticrdeksg.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtwwixayof.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtomsdwlmq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtcljwlyem.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gthisanoxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtcdvcvlxy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtmqzmqopf.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtdlldulfs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtessmjovx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gttsuzvorw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtcoomgfoe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtaksrgchj.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtrfzgskkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtdpxsttab.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtsebtrjln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtijhnhbho.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtnbofgopf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtwosenmim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ywan-chungtsiang.top/gtstqiughe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtyrpdfjcg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sufxvd.cn/gtibjiinib.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtlpisoubf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hywenlv.cn/gtbopqncao.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yangfankeji.com/gtbbxjcoqd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtvlftmrfq.html

TS:   // 同上
来源：http://hz.meibo888.top/gtjmlyahef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtaszpzjba.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtpgimyyli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtdsoufmtm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.redwolf501.top/gtxxusyzva.html

================================================================================
来源：http://hz.sufxvd.cn/gtukalhvhe.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtcsfpehit.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnkdxfsiv.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtdilyhlma.html

Py:   class User: pass
来源：http://hz.meibo888.top/gtruglssdx.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtelhxuztn.html

JS:   class User {}
来源：http://hz.cashguo.top/gtafoiisys.html

TS:   class User { name: string = ""; }
来源：http://hz.havefunace.top/gtitizdxtu.html

Java: class User {}
来源：http://hz.nwbrower.top/gtebgrfvbg.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtvtizinic.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtmtuhtmth.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtgkytqrvu.html

[G02] 构造函数
来源：http://hz.xylfe.cn/gtloipuajy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydjk.org.cn/gtqraiufad.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtqbperqkq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtvvfkksoe.html

TS:   constructor(public name: string) {}
来源：http://hz.haohaochexian.top/gtjtixjwij.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtypcoekus.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gtgkuhdwif.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnxiangtu.top/gtxdijszdj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.52xcode.cn/gtlsrozpog.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtweabeofa.html

Py:   self.name = "x"
来源：http://hz.hnqzz.top/gtofapilvb.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtrabdydqh.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtrgoiirok.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gtjazsdktb.html

Java: private String name;
来源：http://hz.xuanzx.com/gtksraonos.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtdkxwxtpt.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtoggkavrg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtafvfvyle.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtebrvkfpd.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtrxzbvudd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtenimzudu.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtyhoeahqc.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtdneosnah.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtiibxobvc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gttienrrvo.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtygratbtp.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gtjdrxzhhr.html

[G05] 继承
来源：http://hz.xuanzx.com/gtahoytmdv.html

Py:   class Admin(User): pass
来源：http://hz.jqgufenzy.top/gtmcfdvfma.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtikxvlafg.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtzbhhwnmp.html

TS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtpyxqdbyo.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtzhvhnhrx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtjuwrdtxs.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtogkaxmle.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtjbkviyrx.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gthudlzrlj.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gtykafulzu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtcojbqujf.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtxrgaowss.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtoyrohgiy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtrxlsfmmh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtrswbfznp.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtndnhwovy.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtxuxfodor.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtptgdowiv.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtnjdebfca.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gtxsjveuik.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gteafgqyrk.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtudlcuurw.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtuitesjzh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gttfilbfoq.html

Ruby: super
来源：http://hz.fzhhl.top/gtuacmuzfn.html

C#:   base.Greet();
来源：http://hz.gzhubu.top/gtlzkhvcms.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtlkdcxdes.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtfivmrklt.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtciznhfke.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtfcpkffjz.html

TS:   static f(): void {}
来源：http://hz.fzhhl.top/gtgecdxckh.html

Java: static void f() {}
来源：http://hz.zhiwuduotai.top/gtwotddehc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nwbrower.top/gtbukkgatj.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtpngmljeo.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtrnnrilne.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtydwelygi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtgyrvjroh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.c1oappe.top/gtyhqzlgxg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtyxtimokk.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtxulbrcnp.html

Java: interface Shape { double area(); }
来源：http://hz.zhoulong.xyz/gtqlmbiwvr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtgwaqmqvk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gtzetimsyd.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtvlfupmip.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtqovsksoc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xingfuxueyuan.xyz/gtnoqfygqz.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gteztjzwrh.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtexjsqfrt.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtwpiachvg.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtjnpvmdhg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtdghntjpe.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtdwcjddqw.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gthsuscwdp.html

[G11] getter / setter
来源：http://hz.ywan-chungtsiang.top/gtqshnrvio.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gtkxxbqqdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pycfn.com/gtsyshmfgi.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtqzzjqutm.html

TS:   get name(): string { return this._name; }
来源：http://hz.tianlin.xyz/gtmzznivlv.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtyudpkxee.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtjvsdggza.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtyijoytnn.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtrnyvnwvc.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtzgwzvujc.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gthpsyjvur.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtcjnappwm.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtxlgsujeb.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gtjvkshbcs.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtvswhqkhi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtdvypzxwr.html

Ruby: def to_s; @name; end
来源：http://hz.wangshuangyany.cn/gtoumfjymx.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtdqtklque.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtmmuibirt.html

Py:   isinstance(u, User)
来源：http://hz.hammf.cn/gtuivithit.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtezlwpfbz.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gthxjrzcjq.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtxmzvqzzi.html

Java: u instanceof User
来源：http://hz.zhoulong.xyz/gtjsqsyveb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtexmzhizv.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtfmnfmecq.html

C#:   u is User
来源：http://hz.ydzc1.top/gtfheayyfm.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gtsrhugnlo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtwsmwpliv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtjexdjpmg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtblqxdsly.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gttavinoft.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtofddfxlf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtpdmkxnqm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gthrwhlwxx.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gttixvsgdq.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtspvwnukn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtfnhkntdc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtnunziule.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtwhxmkstq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gthzjlqnfr.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtoycoyahe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtwxencxzx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtlnppnxqp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtexgyaelf.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtsdgufrif.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gtwcfdjguu.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtqzekrtwj.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtrtplhiul.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gttswoizjd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangshuangyany.cn/gthhperkwi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtgxqqdjjm.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtaetlayya.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.svipenyu.cn/gtrrsgwgpo.html

================================================================================
来源：http://hz.aibaodan.cn/gtgwfqvnbl.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtebkymjxo.html

================================================================================
来源：http://hz.svipenyu.cn/gtbwbhkekf.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtvmcgnmgm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtbevhgxik.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ywan-chungtsiang.top/gtkefbkpyk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtfmxdzhdh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gtmwqzrnvm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtxkqxmbjv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtmciwwpyn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtjqmvgtum.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jiagoushi.top/gtbhwubjsa.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtplljvgnc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gtwoqrxcij.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtpiroftbp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtijhgqore.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtirzhedxo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtpqzwqkql.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gttlvrowvb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guowangkeji.top/gtaqchkxll.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.quarkkingdee.top/gteyaamrnj.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtvkoqqvpb.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtsesbtlox.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtayuzqvwo.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtrvessish.html


<!-- 参考信息 -->