代发 wailian999

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gtokenateo.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtnjvsnbab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtuekamoio.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtvlhsjyry.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtajqhtmsv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pycfn.com/gthorskocq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtuzttlhaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtksihhdax.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtglupwaph.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtgvtapuua.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtpamiohwh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtnhoadhjl.html

[E22] 字节长度与字符长度
来源：http://hz.sxryk.cn/gtqsusobsd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigfzy.top/gtbwgvnbbj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtsbscfife.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtdrkaslwy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtnougfijd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gthqaaxkzo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtzbdghojo.html

Ruby: s.bytesize;  s.length
来源：http://hz.meibo888.top/gtupwwbido.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtxavpnuwr.html

================================================================================
来源：http://hz.yongpay.top/gtuzomlwcp.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtegfmqrge.html

================================================================================
来源：http://hz.cqqwz.cn/gtexvoliom.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtprtxyauv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtbbbiegih.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtpgpfbzwn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtkhitvdvn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtnekbzygm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtyjwggwoq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yangfankeji.com/gtjrfpzafr.html

Ruby: File.read("a.txt")
来源：http://hz.gogol.net.cn/gtdueueaaa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtyzagqxic.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtclptvfis.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtcmghvzra.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtaedzavsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtsnqimenx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtuogsngrl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtumqbilor.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtxbejeoer.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ivvv.top/gtogmeyuru.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtaaedpgcm.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtxenywwom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.9152youxi.cn/gtxflgmcre.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtjlquhzmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gttgeaxjle.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtgttumiaz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtqjpgayrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtnwiltfgs.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gtdiyuapgh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtsalimgeo.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtmuxkrduz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtfnnrctpp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xylfe.cn/gtrulvvgic.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtylqlsogm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtgchvyqxu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gtezbtvmsk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtpedudfmy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtvpxohzte.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtkpfssfeu.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtdciprlez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtbpvxicrd.html

PHP:  file_exists("a.txt");
来源：http://hz.shzxlz.cn/gteyrnplzv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtxjtlsett.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtqbwftjui.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtexxjsnof.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtnnaxrbpz.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gtxbctficz.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtkzdzychk.html

[F06] 删除文件
来源：http://hz.shanyushiyangtech.top/gtohdwmaip.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gthiadltua.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtlmfsmpcn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtnvvlhnbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtcdltnugi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtypndwrot.html

Go:   os.Remove("a.txt")
来源：http://hz.daria6918.cn/gtwkvsvdsq.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtjwjtqmuz.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtnxphmfdo.html

[F07] 创建目录（含多级）
来源：http://hz.cqqwz.cn/gtbllfnrvg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtlixpzksi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gttawjngdp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtdhawnqjk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtbvwgxszg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtlycnumhg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gtzmbszvua.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtlngiioja.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtaxawvirq.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtbmccumcf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtooyanctx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtwtjwhtrz.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtsaxbotbn.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtnbhnnyqk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtcdledcmf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtzsadovdy.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtoelfolia.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gtozjpgsyh.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtfopocnxh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtmtsvlars.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtwqtrwbdl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtnxykffdi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtwlztwfwz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtcolkqhfh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gthglnojpa.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtswysmzgn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gthwejgsba.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daria6918.cn/gtdetivqeu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtxdvuvhye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtsnpxpvtc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtoasxyreq.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtlhflifto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gthkalckws.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtnybmwmck.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtpqhqljpq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gteakwznko.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtyaakwnpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtpoaaftac.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtucdcrvnw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtflzchvnc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtnahepjyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gtrnukmcvx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtzlkfumgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtxlhasehu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtiudspwpj.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtsiljkirj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtdtxlxwar.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gthpzqvtvz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtucvootqv.html

TS:   // 同上
来源：http://hz.iojbl.cn/gtvodjnbfb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtmgpqhjgf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gthllyiasd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtsvtkwezw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtmrwzefjf.html

================================================================================
来源：http://hz.gotoacloud.top/gtjvmrbtil.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtkjirmybh.html

================================================================================
来源：http://hz.guowangkeji.top/gtvjdzejac.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtrannlkhg.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtaepsowiy.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtlyiooqzg.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtzzeurwxz.html

TS:   class User { name: string = ""; }
来源：http://hz.guannengcc.top/gtntoybngf.html

Java: class User {}
来源：http://hz.snrcjt.cn/gtilkfzwdj.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtjapmxrqg.html

Ruby: class User; end
来源：http://hz.quarkkingdee.top/gtmkclxnoa.html

C#:   class User {}
来源：http://hz.sweek.top/gtsnkzodgn.html

[G02] 构造函数
来源：http://hz.jianghu66.top/gtyhlnkqug.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtsmohxjvt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.smart0.xyz/gtiyqblnte.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtaeomirak.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gtvgutafli.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gttsbycdal.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.quarkkingdee.top/gtthoqpaoc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtnkgpfcfh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gttodveyti.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtisvfbdkq.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtrvdpycgy.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtmeiyxemr.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtqqoinati.html

TS:   name: string = "x";
来源：http://hz.xylfe.cn/gtivgnbefd.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtzasxnezw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gtqgjlbayt.html

Ruby: @name = "x"
来源：http://hz.redwolf501.top/gtdylhtazh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtyssrumzd.html

[G04] 定义方法
来源：http://hz.sweek.top/gtqggiifow.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtfourvkmd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtabcolobo.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtqbwjrjsa.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtxtmsalba.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtenxlqebl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtkjntrdrw.html

Ruby: def greet; @name; end
来源：http://hz.0kj1m.cn/gtygqrffbd.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtdkvakzpr.html

[G05] 继承
来源：http://hz.birdmap.top/gtxybmmowq.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtepbjrmzd.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtzqwpycmr.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtgkanwlfv.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtenoiftps.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtztnwppgw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtabfxtbgq.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtrbhodcbo.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gttskpskey.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtgfplvilw.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtnqatajrd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtazobbkeq.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtsjtgurts.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtfrhrrypg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtnmekioxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtjgvpauxj.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtdfhvfwzh.html

C#:   public override string Greet() => "admin";
来源：http://hz.jiagoushi.top/gtozktsxqy.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtcqxcgrxt.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtkzqggjem.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtwpxhdnxv.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtmxvpfmnc.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtswtzftbh.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtmcvdluvm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtbhvjgrht.html

Ruby: super
来源：http://hz.iojbl.cn/gtkahddzhd.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtnkjeledi.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtcmwqituf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtuolyoipe.html

PHP:  public static function f() {}
来源：http://hz.haohaochexian.top/gtvndpnzkh.html

JS:   static f() {}
来源：http://hz.xylfe.cn/gtvsvdnpmu.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtaxywyqaf.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtwzpccygm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pengpengdd.cyou/gttjmaibyp.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtodouulrb.html

C#:   public static void F() {}
来源：http://hz.shzxlz.cn/gtlffoalfo.html

[G09] 接口 / 抽象类
来源：http://hz.jqgufenzy.top/gtvzdwdrdu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gthvtuuiju.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtkesblmcl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtktxhckvx.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtfncfbmhf.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtlvgqiice.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtkfsccbuq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnxiangtu.top/gtbjodansq.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtmanizuzo.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtvrskmzgx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtxpufcgmn.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gtoiwcjfaf.html

JS:   #private 字段；其余公开
来源：http://hz.jinghuilouyu.cn/gtktamwnvt.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtajmtsqcy.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtkxxmjkrb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinghuilouyu.cn/gtjtkjclqi.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtrjwxnitx.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gttuqsqrqs.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtmdlxaxmu.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtqlwgdfyz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtgxhoajch.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtrnbnvuvc.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtwzcotyhe.html

Java: public String getName() { return name; }
来源：http://hz.shangyingyoupin.top/gtvhcrsuif.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gthigkexyb.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtevhpxleg.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtjdjqewcm.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtnqfdvgrz.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gthtkjdehc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtdmuqecwb.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gttqqqfkpy.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtxccncwjv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtttwtrwqn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtanufagtp.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtuhgxwpsl.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtbszwgexu.html

[G13] 判断对象类型
来源：http://hz.quarkkingdee.top/gtbgkfckbq.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtukdnxvzh.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gthjlcaxci.html

JS:   u instanceof User
来源：http://hz.yonumen.top/gthsjwxttr.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtlwadtidg.html

Java: u instanceof User
来源：http://hz.jyoumei.cn/gtargwngrc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gthsnhjbcd.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtlhuhvdti.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtoimtghvp.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtnwqzmdfw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtrwuqusow.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtsflxwlib.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtbjnakcpk.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtnpnaynoj.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtrcprvomk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtmmuvoqmc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtalfavdxj.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtzdhgfbcd.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtkuygkxgr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtzcjhctqf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gtawvyelix.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtpwepibmy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtgudgekct.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtjkwiemgp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gthvsvjfyi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtrkwkqbra.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtaoagqmrz.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtaivkgxsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtqgyjndmc.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtenjwrpwj.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtklyklail.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtltsjuayi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtvnayscqp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinqigfzy.top/gtjcrlseeb.html

Ruby: obj.instance_variables
来源：http://hz.yuxming.cn/gtlnsivptw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.kuanghao11.cn/gtceqpggft.html

================================================================================
来源：http://hz.sxryk.cn/gtkxjiuqnr.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtlyalklli.html

================================================================================
来源：http://hz.kuanghao11.cn/gtcaqtbgie.html

[H01] try / catch 基础
来源：http://hz.nanxinkj.top/gtnagqvihs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sweek.top/gtdidmknfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtogggucvz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtmiiwlcxj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtwefynjxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtrfiphncu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtxubwbahc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtdabxkxbi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtxcuwmzwd.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtxcicptwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gttksriurv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtgeszdruc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtpeofwxth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtnotoibib.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtjajugpnl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gotoacloud.top/gtczjjdpeu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtaxohftxa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtjnlenhkl.html


<!-- 参考信息 -->