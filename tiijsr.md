代发 wailian999

Ruby: s.lines
来源：http://hz.yonumen.top/gtmmjykwzr.html

C#:   s.Split('\n')
来源：http://hz.316326.xyz/gtvmcbrfss.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtygiakcwe.html

Py:   if not s:
来源：http://hz.nanxinkj.top/gtmzlfwybs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtcpeqanef.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtplpumxxn.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtkeqjblel.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtawgttaau.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtxeugxypc.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtmwxyucop.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtvpewrnwn.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtanbbxccc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhiwuduotai.top/gthlkehjqc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtwewcnfrt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtpggtjixd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtothrxobr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gttmeoropn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtkmcqwhkr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtfegricly.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.iojbl.cn/gttmepypiu.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gttjkdlxqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtsjtxbhmn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtvpqtlvwd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtqofohdfz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtzsmniiqm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtgnooygvc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtsiqcvyve.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gtaowfevct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhaomingkeji.xyz/gtzxgqhxuu.html

================================================================================
来源：http://hz.yangfankeji.com/gtvwfocwrn.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtaldqtknc.html

================================================================================
来源：http://hz.redwolf501.top/gtidfxaskb.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gttnffawax.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtdgyxyhtz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtgohuatic.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtblgrnsab.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtomqnccno.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtprrkfbza.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtqnrdprto.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtmtbnehug.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhiwuduotai.top/gtzzsdoynx.html

[F02] 逐行读取文件
来源：http://hz.sxryk.cn/gthxcmmhcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtkwchkehb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtyubclstq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtftvikdlb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gthshwgflr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtggkpcgel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gtlzgspdfx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtlarawrhf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtrejdlgqv.html

[F03] 写入文件（覆盖）
来源：http://hz.wangdashe.top/gtghdmtdsa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtojpqqnat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtbzadugah.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtdeusekpt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtyqrftcef.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.haohaochexian.top/gtgfgdafnr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtvkniafyr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtuudjkspr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtbwttywgm.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gteyynxqmn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtovvfkkzd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtzoiofmgs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtzdisxbij.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtrivrywwt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtxhfrysfl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtugptjtkj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtaohvxpci.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtnrmmurkc.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtqppywhzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gtptrzwbcz.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gtxfarxxco.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtbxlvookq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtajmynvop.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gticcnegul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtxznwdvke.html

Ruby: File.exist?("a.txt")
来源：http://hz.ybcxt.top/gtpyfoexad.html

C#:   File.Exists("a.txt")
来源：http://hz.xylfe.cn/gttyiuzozx.html

[F06] 删除文件
来源：http://hz.tanke756.top/gtwrnzedkl.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtwkxgcysy.html

PHP:  unlink("a.txt");
来源：http://hz.jiagoushi.top/gtdkaxkroa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtohgtlmdm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtqqvhmoiq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtjomwgqtz.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtivxbcxwn.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxinkj.top/gtsduhgwbk.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtyxekiotm.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtlijveand.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtxryrajiy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.vqdsnc.cn/gtgkcvrjpn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtwtbhdffg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtfiajfibd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gtlpiclxwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangshuangyany.cn/gtuavfeejw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjfxy.top/gtqtdeemza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtguehzxav.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtgcxrafjr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aibaodan.cn/gtuojugckl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtqyrzrccg.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtxrmjpevo.html

TS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtjjhzppqd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtwmsowkuf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtcidwoonb.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gtfhbbkyym.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gaohongyu789.top/gtoucihohe.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtcsqdlgke.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtfyrveunf.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtckxnxabn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gteidekgmi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtipdjsjoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtjgycumvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtxnuqimtr.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtzzfniexo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtgcfqfvrz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtwqaokvaf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtgqzqvgag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtlhmjhure.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtggbqdrds.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtcyvndvmm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtcrsbfyak.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtuanblnty.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtcjxxiiyr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtyugzlvrt.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtvffpgaxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtymyhqvpl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtzbpoikiq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxumcptsv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtzexuwaga.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtjeilzacb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtppylysea.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrlrcbzzm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtsuqlpbrv.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtmgqyfknq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtmfqiwfda.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtnfcbonlf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtmlacxfym.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtffpvrfqt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtvcjofmxx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cucudq.cn/gtibzmytsf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtviwtwaob.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtszelhpkp.html

================================================================================
来源：http://hz.ppjwa.cn/gtdupbqkgr.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtcustnjpl.html

================================================================================
来源：http://hz.nwbrower.top/gtmnignnbl.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtmpjvhlac.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtzgvfpjgg.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gtxgnwwbfk.html

JS:   class User {}
来源：http://hz.yuxming.cn/gtxjiynjyk.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigufen.top/gtmyoejnli.html

Java: class User {}
来源：http://hz.daria6918.cn/gtlehayifz.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtvhgwiccg.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtejuzfimg.html

C#:   class User {}
来源：http://hz.chenjidiqi.icu/gtzkrgejxd.html

[G02] 构造函数
来源：http://hz.haohaochexian.top/gtaxyunpvp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtkhgfqkjz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dashuyun.cn/gtmlxlcyfb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtfghvpicm.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtuqtvqlxq.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtiilwbwnz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtvbphxvus.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtchcxcekp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtmkggbsre.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtguqaosbg.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtkagvpeld.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtphpoazpg.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gtuuuayhlp.html

TS:   name: string = "x";
来源：http://hz.hfpthk.cn/gtpdlmcthn.html

Java: private String name;
来源：http://hz.smart0.xyz/gtawjgfwtk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigufen.top/gtatkxfmyp.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtwfrhdwwi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtjkiigojv.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtxucfelep.html

Py:   def greet(self): return self.name
来源：http://hz.daria6918.cn/gtjwxcgpad.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtlmfrujxq.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtncbczrkc.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtmclyimyg.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtcetjmame.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtciahlzii.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtcbcaipcp.html

C#:   public string Greet() => Name;
来源：http://hz.fzhhl.top/gtpcwrbagv.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtujsifkfu.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtyoujbzxv.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtknatuzet.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtezijhwsx.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtooqmbwls.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtolokfazd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gterobefia.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtmgioayds.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtcsxbpatg.html

[G06] 重写方法
来源：http://hz.52xcode.cn/gtwicsedmk.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtujqhphcs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtesccckvj.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtuqcffpjl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtywpttotx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtowczsafl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtalnvtlwi.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtjntaabws.html

C#:   public override string Greet() => "admin";
来源：http://hz.gogol.net.cn/gtfqmapnea.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtnghdoaui.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gtlfwrenfy.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gtnjhtyzgz.html

JS:   super.greet();
来源：http://hz.daria6918.cn/gtxzzyqlkq.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtetkwkfrl.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtzwvivdjs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cheryme.top/gtnhcpcfvr.html

Ruby: super
来源：http://hz.andypj.xyz/gtwfbzikfa.html

C#:   base.Greet();
来源：http://hz.cqqwz.cn/gtnxlqwior.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtwbzvamso.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtlndcjgxr.html

PHP:  public static function f() {}
来源：http://hz.aibaodan.cn/gtexkluipu.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gthpymzcox.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtjrcmswfl.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtxbvdfget.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aizwys.cn/gtxlfzhvdo.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtlfrjlmff.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtvxmflxyz.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtkqiteiym.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhijiandao.cn/gtysygsjgo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.feifeiyinyue.top/gtejgcmxgx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258888.top/gtzclluljn.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtalrukzqq.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtqniqsndo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hongshengwenyu.top/gtxfwdsjnf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtvtswluqo.html

C#:   interface IShape { double Area(); }
来源：http://hz.sysykeji.top/gtaxbhjvgt.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtdnqgiraw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.meibo888.top/gtiaeccoeh.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtyacvmnfp.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtygapatop.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gttispqrna.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtffogggpp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gtxxhurevb.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtrptzqsde.html

C#:   public / protected / private / internal
来源：http://hz.yuxming.cn/gtindeqbyt.html

[G11] getter / setter
来源：http://hz.pycfn.com/gtihhlfqce.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtjmalgttn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtxyfhccyp.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtlugoatci.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtedtougfq.html

Java: public String getName() { return name; }
来源：http://hz.fzhhl.top/gtmhqdizcp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtgeuilvbu.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtxcsudyqx.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtpmetjjth.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtuhnugbpm.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtqaytdnvt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtogcxcemj.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtjuiddckb.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtayaypctf.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtmzdtuyav.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtquctgqfp.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtohhznbtu.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtgwxnnvcx.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtbojgaxgj.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtessbowlk.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtmonjzylq.html

JS:   u instanceof User
来源：http://hz.yongpay.top/gtlvygjmji.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtwevtwcuw.html

Java: u instanceof User
来源：http://hz.sweek.top/gtdklmerxo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtslrnlgmt.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gttaycywxg.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtqzwcrkbu.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtypijfsdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtrsgyubct.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtjtrfoxsh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtpysdnvjf.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtsdcldlke.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtdtfmyqxt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtobcfwngs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtscdenrkd.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gttqtodsqy.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtedikhptv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtoqumphqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtfbmzorlu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gtdqilymiu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtrnpyccjp.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gthtgxgkgx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtmrdieuby.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtspbbgzug.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtqkdlptju.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtdupdxbsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtazexeitq.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gteqasfrkn.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtnwrmqilx.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtflzpskrr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gteiidnumu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gteofyofjd.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtayjrxnij.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtbtswfdpw.html

================================================================================
来源：http://hz.tanke756.top/gtskucbcbl.html

H. 异常与错误处理
来源：http://hz.vqdsnc.cn/gtzbycnfnv.html

================================================================================
来源：http://hz.dianchejie.cn/gtmkmfracp.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtruqyfbtw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenzaomai.com/gtumfudlib.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtferxcbkf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtyjarrkvv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtkutnvhku.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guannengcc.top/gtnpqfejqz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuxming.cn/gtwzdwekts.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtyagmyfpo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sysykeji.top/gtbjekenrw.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtlnoxzehb.html


<!-- 参考信息 -->