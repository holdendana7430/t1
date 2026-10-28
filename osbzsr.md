代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtnilscxqq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.fzhhl.top/gthrtecpfc.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtqmxxkbtc.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtfiwdwomu.html

Go:   if s == "" {}
来源：http://hz.sweek.top/gtjhmypoui.html

Ruby: if s.empty?
来源：http://hz.xingfuxueyuan.xyz/gtbqtjuyal.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhongyouzk.top/gtyhnuhnby.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtxrwwuete.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtyaokqzmh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhiwuduotai.top/gttwizoazn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtozdqjsgu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtmnpphrdz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtbchwhwtn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.c1oappe.top/gtfxqnzkfd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuanzhike.top/gtvufwxnsn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtcxuaagxn.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtgpznuwsz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtdhvbwbez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtsucgukfe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtvnhdyqtj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtqkuhbqcf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtruzoudhw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.c1oappe.top/gtxgrwlfiv.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gthvuiycbi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtkdrsrwzj.html

================================================================================
来源：http://hz.pycfn.com/gtsqzhkeqe.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtstadkvgs.html

================================================================================
来源：http://hz.guowangkeji.top/gtncquuake.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtmvnnxkoe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sysykeji.top/gtxuwyrosh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtiujwypod.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yonumen.top/gtgxoxpnml.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtkffwagip.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtdwmouzro.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtucixaydq.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtzriwxoyz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.316326.xyz/gtqmculkwp.html

[F02] 逐行读取文件
来源：http://hz.hammf.cn/gtdqdnkgms.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gtuqwoowyw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtzcfycbbh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gttwecbpnu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtursetsaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtinahbctt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gaohongyu789.top/gtlxyocwcy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtrtsyondg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgufenzy.top/gtiqczwwyf.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigfzy.top/gtpotugxby.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtdleerrkv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydzc1.top/gtockrnexw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtejbwxcva.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtxyqvwvxu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtndayruqm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtmawskfvr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangkeji.top/gtqivcnheg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtmccchiau.html

[F04] 追加写入文件
来源：http://hz.iojbl.cn/gtzmellezn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnxiangtu.top/gtydfzkbrp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtdmysvbht.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtsthuexpa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtvlyabkui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zycfv.cn/gtxudolorf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ppjwa.cn/gtijowwuui.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangtech.top/gtyryrtzfl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dianchejie.cn/gtmkqgyrrt.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtlydxurwp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtyopqlqio.html

PHP:  file_exists("a.txt");
来源：http://hz.snrcjt.cn/gtgdufcvas.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtlquosdav.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtxrhltdjm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtqsnfiuiy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtnmqecwxr.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtzpwludqp.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtytmpvrye.html

[F06] 删除文件
来源：http://hz.zycfv.cn/gtjpbwwdvg.html

Py:   os.remove("a.txt")
来源：http://hz.gogol.net.cn/gttwlnogqn.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtpfcauzrp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtziqxbwvo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtiueetoxd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtihxixeqj.html

Go:   os.Remove("a.txt")
来源：http://hz.tianlin.xyz/gtuzhxnaoo.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtggtagaaj.html

C#:   File.Delete("a.txt");
来源：http://hz.guowangkeji.top/gtjgdpmoki.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtybhwazjm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtivjfoadi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuanzx.com/gtqkgjeukj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtvxjqimuu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtipficpox.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gtpwklxlub.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtndgrodds.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtaenmmomp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtnvbzyjlb.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtunnpdptq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gzhubu.top/gtdwtbdbav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuxming.cn/gtbwqgwlrv.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gttrbavthl.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtyjuoponr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtpeziunup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtmnswnhqj.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtbiycjpcc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtgbrfadwf.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtenpnmmor.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtymdeavgk.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtchuycwzr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtasicnzwh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtoblhxdkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtnhaxifrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258.top/gtstutgxlc.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtcfrezlwm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.andypj.xyz/gtlzbwtyre.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtsgzuryip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtqkwmyxqf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtmsdmffwr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtrbhbjhxo.html

TS:   path.extname("a.txt")
来源：http://hz.birdmap.top/gtjkqzkxee.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtahojerqe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtgpxtnmgj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtcersnacc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtmqmhuezo.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtyemmspjj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtgnzbebgy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtiyvrpsvt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtwirfinsi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtalqbsubp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tanke756.top/gtvwsauepx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtesedplhn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtgecnrmvr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aibaodan.cn/gtublskizu.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtdxmajrrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtlhyenckn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shangyingyoupin.top/gtmgcguyic.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtmptvvita.html

TS:   // 同上
来源：http://hz.wangshuangyany.cn/gtxwxizsuh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj202588.top/gtvabowotl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtwtmmbgog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtchdyldfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangshuangyany.cn/gtkmgpchnm.html

================================================================================
来源：http://hz.0kj1m.cn/gttqpgsoks.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtnanastkb.html

================================================================================
来源：http://hz.9152youxi.cn/gtvjvxwzje.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtxlcuwiel.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gttxpsmjjt.html

PHP:  class User {}
来源：http://hz.52xcode.cn/gtovnyocod.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtnpxayxor.html

TS:   class User { name: string = ""; }
来源：http://hz.316326.xyz/gtojsmlqdw.html

Java: class User {}
来源：http://hz.smart0.xyz/gtfvccpmjk.html

Go:   type User struct { Name string }
来源：http://hz.tian-w.cn/gtdshnapte.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtkkglpegs.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtlioknpua.html

[G02] 构造函数
来源：http://hz.fzhhl.top/gtoxfffcni.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yueranfly.top/gtoredpxxu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtilrqfvqk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtumlpwfab.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtechpsncc.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtmomacqfd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtojliescw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtdnxbnjuo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtobonhcgr.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gthkwrnxjk.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gteksctuaz.html

PHP:  public string $name = "x";
来源：http://hz.cheryme.top/gtzlyaarcn.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtmctalarv.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtrsvdbfgi.html

Java: private String name;
来源：http://hz.xylfe.cn/gtswndbrkw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtalojwmrk.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtxdgaurvo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gzhubu.top/gtxsowiaxw.html

[G04] 定义方法
来源：http://hz.jyoumei.cn/gtlntqxceq.html

Py:   def greet(self): return self.name
来源：http://hz.hongshengwenyu.top/gtkncqshfo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtkqhcztqu.html

JS:   greet() { return this.name; }
来源：http://hz.nanxuanxn.top/gtwobzomsb.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtlajngcxk.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtvpimnkxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gtshgjuyfl.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtprhuxgwb.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gttkmvnled.html

[G05] 继承
来源：http://hz.yangfankeji.com/gtannyywiz.html

Py:   class Admin(User): pass
来源：http://hz.0kj1m.cn/gtwotgpsbi.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtqepaqons.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtmcdkzosr.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtlxshftuy.html

Java: class Admin extends User {}
来源：http://hz.shzxlz.cn/gtcnjunsbi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtlwhsrhpo.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtnpfonnmj.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtyoejlckl.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtuskssaya.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtvwojlqzy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtgkkerwbc.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtczmbyjom.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtcecmlyya.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtyifhcgmv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtzshezozm.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gtycddssnv.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gttpeqnrey.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtpslpgyez.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gtlyvwacmh.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gtrmovwmnu.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtscslljbt.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtmhnjbedz.html

Java: super.greet();
来源：http://hz.316326.xyz/gtcqkjvdwn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtnmomudzp.html

Ruby: super
来源：http://hz.birdmap.top/gtcxbljqyp.html

C#:   base.Greet();
来源：http://hz.zhongyouzk.top/gtypxasfyy.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtgkecssti.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtspykrapk.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtgrvfijvg.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtwitaxyvh.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtrghpvrjc.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtuirfipvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtxdqedhjk.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gtoaenjnod.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gthouukyqj.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtkirbstyk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtsqwgimvz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtfiyexyts.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtpvbokfab.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gttjvidntx.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtxydqeuwj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhijiandao.cn/gtnyneomvu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtdosacrwr.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtcmeaxmaq.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gtmuraffpq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuxming.cn/gtetzzizqn.html

PHP:  public / protected / private
来源：http://hz.xylfe.cn/gtdwdmdmzg.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtzhhqiscl.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtiyvsqszh.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtfitnklty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtrylwdbsh.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtupwgdigx.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtlcmaaixk.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtmyodetfq.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtvrayeeyn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtwpseqyvz.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gthigywqzf.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtvkmmpgso.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtdjnvtcvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtfquhoqwv.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtgffvbpqc.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtodufaaea.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtjtjqroav.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtmfzzagff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtfyqklbqh.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtzsmutwvb.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtxlomuccr.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtzvqqlwni.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.andypj.xyz/gtslvgwjbr.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtduqvprhq.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtpiimwxzv.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtllctfyzw.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtagqaatoa.html

PHP:  $u instanceof User
来源：http://hz.kuanghao11.cn/gtiguprplj.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtwfddvdgh.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtotzgsqsb.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtwumzslwz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxinkj.top/gttgpbaruu.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtdbfxrwqu.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtxyzaiuhw.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtqxnxbvgf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cashguo.top/gtahrbtzsj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gogol.net.cn/gtgilcdulu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtqykvpqim.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtrtitlybf.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtitqfcdys.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gteycqtkkh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gtqkurehcb.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtoiryusov.html

[G15] 枚举
来源：http://hz.yonumen.top/gtsvscpsxf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtxuhtrrpx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.redwolf501.top/gtevtrdfeh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtehlwytqw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtqlberkru.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtrvdyfhag.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.vqdsnc.cn/gtjaznmajq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtxwcfcrxx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtvhcgxnft.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtdmfbsqco.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtrcglgafq.html

PHP:  get_object_vars($obj);
来源：http://hz.yanxiufei.cn/gtgeofhvig.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtocgpjqik.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gteywopdcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtvazjdexo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtgahmjvfq.html

Ruby: obj.instance_variables
来源：http://hz.dashuyun.cn/gtfzlapryr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtdwzomuoa.html

================================================================================
来源：http://hz.wangdashe.top/gtwrbtblxg.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtclvrthtb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrlulylmp.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtguevjnwv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gtauftwjgj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtocobbbgs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtfwzrbmux.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtxyivkwqc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtmhkuvnxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenlongwang.top/gtwyffmrvr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtfhzyfhjy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtauvtahoo.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtokfwzkhj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtxwgfrsbh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtwrozrffo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtgvpuovka.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtjsxvvhxr.html


<!-- 参考信息 -->