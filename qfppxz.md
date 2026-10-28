代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtgwyvfcsg.html

[E19] 多行文本按行拆分
来源：http://hz.jyoumei.cn/gtncgfhcmm.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gteangupah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtlilavvhf.html

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtxmzpupfa.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtzlofrxvb.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtnkltipcn.html

Go:   strings.Split(s, "\n")
来源：http://hz.zdqjudy.top/gtkrfsgrzc.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtpqkasjmn.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtqljrtrky.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gthwujwzsu.html

Py:   if not s:
来源：http://hz.ydzc1.top/gtqpbsisxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtgibaztnf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gtoszyjihr.html

TS:   if (s === "") {}
来源：http://hz.guannengcc.top/gtnfdjspbt.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtqxynjdjh.html

Go:   if s == "" {}
来源：http://hz.xziqi.cn/gtxfpoqagc.html

Ruby: if s.empty?
来源：http://hz.ppjwa.cn/gtohbqshsx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtgyqomrlr.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtnhfzmmxa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtuyyyctvz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtbtshmaro.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtyjjrnopl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtujknujkc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtowhhrpqe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jianghu66.top/gtdvnxhctz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtqtrtavie.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.52xcode.cn/gtpfdvlpiy.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtcpisvvoj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gthhrtnnyo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtnzyxqefm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtossucwbr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtyfmlyhcp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gtuxvwzuvi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.svipenyu.cn/gtrjbxcsoz.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtnupqxpxb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtbwmvlsab.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjyrmoigi.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gthsfdzblg.html

================================================================================
来源：http://hz.aizwys.cn/gtuhzxidzp.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gtxuahrynn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gteggfgyty.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtxpzplppa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtsbhgzipt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtytpqsosq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gthimtacbv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gthavyifha.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtmlofiazz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtblurbcnb.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtzaulcggc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtkefpudpl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtzbkidvly.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtcpsrthid.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtayfrtlvr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtngjyanpq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtheagknhu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guowangkeji.top/gtydkpawej.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtxbzdiwup.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtwhcxsqmk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gttqmsaozn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtqpwxnrxx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtlybomzqk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtalfudcnd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtdnqxidpl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtwsmckwsf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtricuqdak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xinyue.icu/gtqstkywrn.html

[F04] 追加写入文件
来源：http://hz.feifeiyinyue.top/gtyjgxcdio.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fzhhl.top/gtokjoffya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtgfrtkyvg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtjavpvxav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtmyvddlnl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gteuqawoop.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shzxlz.cn/gtvrcaiktw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtkdgmqqht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtdjzhwwrt.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtpohlezcq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtoxtsycue.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtnsupqwbn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtgifhxblq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtkifuvnef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtqzgjrhjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gzhubu.top/gtvfphyuml.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtkkebnmbp.html

C#:   File.Exists("a.txt")
来源：http://hz.chenlongwang.top/gtnzrlqskg.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtylfioadl.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtawugexoi.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtwtsameji.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtmjssitfb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtsloygscp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtaqlxpzxr.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtzjzyoaxv.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtuhusicou.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgufenzy.top/gtfzdegeyg.html

[F07] 创建目录（含多级）
来源：http://hz.ywan-chungtsiang.top/gtwwuckpkb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtakqdrvvn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtmyaxhmlr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtkxiosntt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtrcpmmhwo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtuaenumum.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangkeji.top/gtzwcqpisn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtfsdbxisw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtohtfbmpf.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtfsmwuacp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aibaodan.cn/gthpmqafzs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtuobjmbua.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtskpuaziw.html

TS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtplvidjlp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtwixcfstg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtddgpopek.html

Ruby: Dir.children("dir")
来源：http://hz.iojbl.cn/gtkllzratx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.316326.xyz/gtaajxynyg.html

[F09] 获取文件大小
来源：http://hz.yueranfly.top/gtwqhfaisj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtljnhpxjy.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtlfyujlgt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gthmaazcvl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtrdkmhnfg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtmglfzkbi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtaxotqojx.html

Ruby: File.size("a.txt")
来源：http://hz.feifeiyinyue.top/gtkigkjcsd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtjdwzzxle.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtxocrirps.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtifddpqte.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtpmdulgeh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtvqnjrcuu.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtvlcafhfc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtxoyamlhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtttyxijah.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtdrhttpsz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtlqmzvduv.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtyrfnzjfi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtrxcnvvio.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtgbmnqwyk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gttmobjrgx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtnhtiwjgf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtocexcnxh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtaamcljmp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtcxmppico.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtnyyglgaq.html

[F12] CSV 读写
来源：http://hz.jinghuilouyu.cn/gtzuqvxffb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtjycxecdi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.9152youxi.cn/gtpddcmqut.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtsiqgxlac.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtxwddrcmw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtsszsuqdd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtofmpyjds.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtmuortmyn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtjzqnpuoe.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrhnqtahr.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtlzwziwxa.html

================================================================================
来源：http://hz.redwolf501.top/gthzfdxqpr.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gtqzvkabnh.html

Py:   class User: pass
来源：http://hz.havefunace.top/gttrktxrkg.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gthgchugji.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtczcpqzga.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gteojcydme.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtjfivgwcs.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtpaukxqxw.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtlgjwiaad.html

C#:   class User {}
来源：http://hz.cashguo.top/gtyhttmuaj.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtrfakfwtv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tianlin.xyz/gtuzvexgyl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gttgrzgiwd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtpnocrciq.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gtwnmcoggi.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtlhjoxixk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gthpejvnwx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtmbhmyccr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtjprbzjyq.html

[G03] 实例属性
来源：http://hz.jinyuanbaomall.cn/gtlghpbbnx.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gthhgyrqbp.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtqztryawz.html

JS:   this.name = "x";
来源：http://hz.hfpthk.cn/gtogrbybmt.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtunrvgktw.html

Java: private String name;
来源：http://hz.hammf.cn/gtjwiienwl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhongyouzk.top/gtsoxcwoqn.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtaqxkrptv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtxpotxmkq.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtglruwiji.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtbzpnubls.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtyuopiihw.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gthmosnnft.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gttijusdnq.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtarzkcfah.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtbigsrfuv.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtjkxdcsyu.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtfrwugqtn.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gthpakcwas.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtibjayrfd.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtnviqovgo.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtkienyknp.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtoikgadir.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtopgqgcts.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhixingplan.top/gtcbihhiay.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtbecacysn.html

C#:   class Admin : User {}
来源：http://hz.zhixingplan.top/gthnrsrxxh.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtfwydcbpd.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtitscxybr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtumnowskl.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtlcwkibxk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtmcduqpsx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtwcecewid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jiagoushi.top/gtxzxorfhq.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtgrdpijly.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtvqqwvoke.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gttmtpvimu.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtvarwncvp.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtjmnqgxiv.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtygczgcyv.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtvmstsyce.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtrjrexptl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtatehoavo.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gtcvgqzyfx.html

C#:   base.Greet();
来源：http://hz.sufxvd.cn/gtydkrwwty.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtccxcngzd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtkgmpoahf.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtqzmwsycy.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtqiitqweg.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtsqyudkui.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gttfeekhaw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gttfbfxyrb.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtfqblyktm.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtxjjxifxo.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtqqedpoad.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtpbjczfwq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtsgsnedvv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtbcaudlad.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtmanpkmih.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtkmuecppf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtxzufgjtb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gtggutrrrj.html

C#:   interface IShape { double Area(); }
来源：http://hz.sxryk.cn/gtexqnapdc.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtqharbnqh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtwgsyxprs.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtauoxmkmb.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtoxhhosfi.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtaeqvscok.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtsgbddvij.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtwxlqbgce.html

Ruby: public / protected / private
来源：http://hz.zdqjudy.top/gtpboiusfd.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gthvudlbye.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtzzwhxces.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtikgeisaj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtkmcmggxg.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtjeyaycuu.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtizofxouh.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtbowfvlrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtifpvpjrq.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtqbmcczzy.html

C#:   public string Name { get; set; }
来源：http://hz.svipenyu.cn/gtclnxjtrz.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtegzdxqua.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gteclxdxal.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtfmcoyyuz.html

JS:   toString() { return this.name; }
来源：http://hz.havefunace.top/gtbidjxkss.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtuqjqddjv.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtiwehxnie.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtaapcwjxt.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtfsrukpno.html

C#:   public override string ToString() => Name;
来源：http://hz.sufxvd.cn/gtywrkhaah.html

[G13] 判断对象类型
来源：http://hz.shangyingyoupin.top/gttqkrujui.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtfulsggoa.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtfybwekkc.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gtkxzcbgeg.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gtfwzadjwu.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtdidymdcx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtjlksomgz.html

Ruby: u.is_a?(User)
来源：http://hz.andypj.xyz/gtmratukkj.html

C#:   u is User
来源：http://hz.aizwys.cn/gtcdvwveps.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtuirnthsa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gttawzsrfu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtfjvmxshe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtzcsobyjg.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtxndyqptr.html

Java: record User(String name, int age) {}
来源：http://hz.dashuyun.cn/gtzraklxhe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtkyyshmgq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtpoujzjxn.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtdzdvmkgm.html

[G15] 枚举
来源：http://hz.meibo888.top/gthtpttfec.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtectiujve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.316326.xyz/gtoypvypgv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtzlygvuua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtpqikjaou.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtybgqqjko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gtyepwmkib.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtsiopjqhy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtfotqnvyr.html

[G16] 对象转数组 / 字典
来源：http://hz.xuanzx.com/gtdjbnqiqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtcriadkmm.html

PHP:  get_object_vars($obj);
来源：http://hz.yuxming.cn/gthqbdqhjx.html

JS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtehbricnd.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtezjiwcli.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtpbldfzef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhijiandao.cn/gttaqewrpy.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtcxpatnhu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtnflxowht.html

================================================================================
来源：http://hz.hnqzz.top/gtoktjvxve.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtdvpvcbga.html

================================================================================
来源：http://hz.pycfn.com/gtjrquinup.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtvbzjyxnl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtwvkpwqfi.html


<!-- 参考信息 -->