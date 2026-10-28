代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtbdvlsfnn.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtfyzlqmno.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtdfxfvjrs.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangkeji.top/gtvpqvrafo.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtqlxomrvn.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gtoswqeyvg.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtfukohxzk.html

Py:   if not s:
来源：http://hz.gzhubu.top/gtdphnopag.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtacxpomir.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtzzksfzjq.html

TS:   if (s === "") {}
来源：http://hz.tanke756.top/gtztuiwcko.html

Java: if (s.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtsqkmxrbu.html

Go:   if s == "" {}
来源：http://hz.jianghu66.top/gtsixhyyid.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtreplqjvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhijiandao.cn/gtdubrysse.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtbqugnkpd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtemnjuvdp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtivrajzga.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtvapehkal.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtlwswdozr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtththckzh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtumiqjszt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtouxxxuvj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gtuwfkjdto.html

[E22] 字节长度与字符长度
来源：http://hz.xuetiantiany.cn/gtwaczmcpk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtbcfotqjb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtuooftfxa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtsdhkhqor.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtbptfwuqt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xylfe.cn/gtbjkomcvw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtbelgwgaz.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtqxbgevow.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtgtlefoej.html

================================================================================
来源：http://hz.daria6918.cn/gtklkfkhrd.html

F. 文件与目录
来源：http://hz.hywenlv.cn/gteeaqkvyr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrandqjxw.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtkkzkjgyo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtpckscprb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtdxjtrevd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtfwksljza.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gtlnbfqiqp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtbetmkxeh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtmteyjdvd.html

Ruby: File.read("a.txt")
来源：http://hz.pycfn.com/gtwxhaleqb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.52xcode.cn/gtijmnywmm.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gthxbykhdh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtewpcagij.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gttsecgcvt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtxecgazht.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtcwvxfege.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtovttjkcj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtftdjhanx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtkjfrfmpb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.andypj.xyz/gtihauoctk.html

[F03] 写入文件（覆盖）
来源：http://hz.snrcjt.cn/gtqifipzor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtcatvioml.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtgdnkinky.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtsbjrassp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtpsdwbudj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtyllcwlka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtuutopxot.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtpjsbgull.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtekdwxrly.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gttmeeorpf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtgfwxjkab.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtwverjjwd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtkjiorzlq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtughkyyfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtdcfulqhn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtgtmmeptv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtbxnzxcvb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtfuuzqxbh.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtcxfdeeya.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtnjbpjnyn.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtvjnidzow.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gthhggfcov.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtvrnmtzup.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtygtawzdh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtgmcldrwq.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtchfpkmcw.html

C#:   File.Exists("a.txt")
来源：http://hz.redwolf501.top/gtwgbxdpgm.html

[F06] 删除文件
来源：http://hz.wangshuangyany.cn/gtsxymefov.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtjyaevkqt.html

PHP:  unlink("a.txt");
来源：http://hz.chenjidiqi.icu/gtyucykyvc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtdyiozwvk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtcwbashgh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtoaezcoej.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtivelbail.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtnjlfzchd.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtxthdewpi.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtevcfrnbe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gthubspxux.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gtkjwbqrza.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtwphrxdji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtbibllfzv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtbpfsqkux.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangshuangyany.cn/gtzeufogar.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtjdjmwpmo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtvvvorcyz.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtwbvuddvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yongpay.top/gtwgiahtsi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtfoyihxsr.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtsyxjakny.html

TS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtrqtdeukh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtzkczbhry.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtngagehfq.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gttlzyatmv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gtubpinlrj.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtnkxltudk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.redwolf501.top/gttqasybdl.html

PHP:  filesize("a.txt");
来源：http://hz.chenjidiqi.icu/gtnaldratq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtkmnutkhe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtqulrljio.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtkwrhttkf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yangfankeji.com/gtkjaubrop.html

Ruby: File.size("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqujkbety.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgufenzy.top/gthjtszkby.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtcjktvqtp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtcytvmmky.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtmnkgmttj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtzlhawwgd.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtecrspnws.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gthlluzeww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtrxrajawb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtobgdcrqw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtdgwicobn.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtwofpkrci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtsocwwiti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtjpbjxkrv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gttjmqarke.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gthnpeguor.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtyjbnmzsg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.vqdsnc.cn/gttzrelcoy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gticqkddls.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtfsyyhnxm.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtbdsslxsu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtqddwemul.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtkdehhsld.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuxming.cn/gtxovxpvxt.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtcsnslxcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtlwbfdzaq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gthbvlvlsc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gthorcvdmj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.smart0.xyz/gtempndarf.html

================================================================================
来源：http://hz.dashuyun.cn/gtsctzrlne.html

G. 面向对象
来源：http://hz.jqgufenzy.top/gtbzbdqjyk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuyahdgli.html

[G01] 定义类
来源：http://hz.jlsjyb.cn/gtjurorfvz.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtzkumjxjh.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtphboslae.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gtfnjnadjt.html

TS:   class User { name: string = ""; }
来源：http://hz.zhongyouzk.top/gtxrbzwzaq.html

Java: class User {}
来源：http://hz.cucudq.cn/gtcygptchk.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtycmvithz.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtojecodbr.html

C#:   class User {}
来源：http://hz.aibaodan.cn/gtftmmagui.html

[G02] 构造函数
来源：http://hz.yj20258.top/gttjnbrxps.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtbnkytsrm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtldlokrpq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtrhnmjgkn.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtkuwitfht.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtwoahakvk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtpmrcqxoe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gttyouqjft.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtgjyyeadf.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtzdwhzbwu.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtpadsopaz.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gtpatbiuhr.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gtpwgsglyb.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtqmtbzdup.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtlozmdpgy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtkwncriaz.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gtguvwqqpp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtkhzjxhfo.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtvnjoqeqt.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtjzcxcbdx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtdddluned.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gteouhkqhz.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtaxrrowfy.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtqaggvdkt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtvvpfixue.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtxwabxrhw.html

C#:   public string Greet() => Name;
来源：http://hz.redwolf501.top/gtuheznkrm.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtrawxhvck.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtkcnthwhz.html

PHP:  class Admin extends User {}
来源：http://hz.daxiang520.top/gtjceteqwh.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtbtrvyeaa.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtuoiwikkv.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtkqjuoopq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtvtuvgeyo.html

Ruby: class Admin < User; end
来源：http://hz.0kj1m.cn/gtetzziyrn.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtopbxjgam.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gttwxgcejn.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtynyaxmjh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtlxokjokn.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtrpoyiewp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtvwcleynv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtkurxdsgv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtypaumbbu.html

Ruby: def greet; "admin"; end
来源：http://hz.havefunace.top/gthbqkioef.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gticjgmixb.html

[G07] 调用父类方法
来源：http://hz.yongpay.top/gtxsxbbnhk.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gttxhjkcji.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtzgowbvsy.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtdgomyfyn.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtanltugkd.html

Java: super.greet();
来源：http://hz.jqgfzy.top/gtokaghlzp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.haohaochexian.top/gtxvqsglhz.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtlyzwcwvn.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtwlomkoyj.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gthnozqmvc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.0kj1m.cn/gttuvdfhqq.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtrxonooho.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gtmwqovekk.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtqkynipmc.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtiztgvcsf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtkhtfsfew.html

Ruby: def self.f; end
来源：http://hz.xuetiantiany.cn/gtqqnymeyp.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtdpuwmxdc.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtkluscebo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtrffwvcmh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.quarkkingdee.top/gtissminjh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtbuwksmmy.html

TS:   interface Shape { area(): number; }
来源：http://hz.shangyingyoupin.top/gtmbabsyjt.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtppdjojbk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gtmvltmvzf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtvkhqnirz.html

C#:   interface IShape { double Area(); }
来源：http://hz.quarkkingdee.top/gteygtbosc.html

[G10] 访问控制
来源：http://hz.havefunace.top/gtwlwflxdu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtmmlcwzod.html

PHP:  public / protected / private
来源：http://hz.iojbl.cn/gtnkhrshww.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gthgxvlutq.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtmvtqyyas.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtjfrxmlvr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtthfszgub.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gtjuvkpftx.html

C#:   public / protected / private / internal
来源：http://hz.chenzaomai.com/gtuaqwprgr.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtibwxhhej.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtilirepkf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtyxnkuqxd.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtlknfjkbd.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtkoikhpxw.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtztyextur.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtdvdphmzw.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gttsnsztmq.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtsaztdiip.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtnfngsfvs.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtbqnfuqoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtdjeqrynd.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtcxlpzqze.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gthkmnyriy.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtifihuqhc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtxppbegmz.html

Ruby: def to_s; @name; end
来源：http://hz.yuxming.cn/gtajujwofy.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtfydwgwxo.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtpnatqhom.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtjwujgbdo.html

PHP:  $u instanceof User
来源：http://hz.snrcjt.cn/gtutblpjgx.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtcdtoiebo.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtgyywjxxc.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtegoqkzvd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtecriwruf.html

Ruby: u.is_a?(User)
来源：http://hz.ppjwa.cn/gtugbbmbdy.html

C#:   u is User
来源：http://hz.yvedp.cn/gtxkfqrfoy.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtwdhqnbeu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtrsxhorri.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtjmqczrpm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtfaarwsja.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtydormtbb.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtqkliuben.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtafrykpxs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtnrulbads.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtlbglgktw.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtpwxbazyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.9152youxi.cn/gtbiszteoh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtohrptgch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtttuyzcjo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtyqvtyuyy.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtphrkjbmy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtruwvwshw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtujmqsrvf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtthpgjpck.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gtftswybfo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtguiydklt.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtpquctwzc.html

JS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtclufjifm.html

TS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtyglnzele.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtuvbrahvv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtssufpfex.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtygtbynvi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gttnwvwkhz.html

================================================================================
来源：http://hz.xylfe.cn/gtgxghrner.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtfjaffbaa.html

================================================================================
来源：http://hz.jinqigufen.top/gtktsjnvii.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gthnyceyuz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtizmwtelz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtlhfgkirm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtublpboyq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtxjrcxtdr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtrtzpqtwd.html


<!-- 参考信息 -->