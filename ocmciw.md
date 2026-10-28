代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gtuacpzhwo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtyjfjlppp.html

TS:   if (s === "") {}
来源：http://hz.tian-w.cn/gthivrbgcz.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtkhwykoqt.html

Go:   if s == "" {}
来源：http://hz.redwolf501.top/gtlztndubp.html

Ruby: if s.empty?
来源：http://hz.nwbrower.top/gthbhvhvdn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pycfn.com/gtzjsbnrxd.html

[E21] 超长截断加省略号
来源：http://hz.zhengqikj.top/gtgqddzcgw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtgkmatbxl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtekevheyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtsphnaikb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtjycxefhb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtqewjvpry.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtkhbsfvem.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gthpijnxzr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtbeiequuk.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtvkoeiraa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtukpzgihw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtsqivccpi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtxrxptifw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtmqnkyicv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xinyue.icu/gtczelkvgb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtuyhnnmfp.html

Ruby: s.bytesize;  s.length
来源：http://hz.iojbl.cn/gtsgkbombr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtfxcnzlrd.html

================================================================================
来源：http://hz.iojbl.cn/gtdafpurpl.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtdujfpxbl.html

================================================================================
来源：http://hz.xziqi.cn/gtnhwikjem.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtzwqpewjj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtyjvqkwlb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtlipjvsuv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtrdyxmngi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xinyue.icu/gtkvbjtdns.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtcicwrcfz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtyumvpumf.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtqykzddzx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtrjgfbsjd.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtodbivlxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shzxlz.cn/gtvlfxbkgl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtdgmejxjv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtpapuleqm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtgqmompjr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtuqysvrtw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtxhavltjt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtbszsxizi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yvedp.cn/gthztuxxaj.html

[F03] 写入文件（覆盖）
来源：http://hz.sysykeji.top/gtrlbmdnzt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtsywodowr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtehidldbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtdrutvjsp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtszdonkac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gteicmuaim.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtehnghgnc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtylpumewq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtpeupkdgo.html

[F04] 追加写入文件
来源：http://hz.cashguo.top/gtwhtbflit.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gtwxfzscss.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guowangkeji.top/gtgfcjraig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtizurtdib.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtpnmoodlr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.quarkkingdee.top/gtlzuztvlu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtammkbzbz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangshuangyany.cn/gtakofynao.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtfhyoyejt.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gtgcxllfur.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtvmouunfj.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtldkbmima.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtstnrawch.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtrwzgrmez.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtvigklsdj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangtech.top/gtqalauvtz.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtgknwujya.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtxphosqaq.html

[F06] 删除文件
来源：http://hz.svipenyu.cn/gtgjunapfo.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtnhdojlkj.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtjnynjhmm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbzkdjomc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtjaaeezye.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtjfhdobor.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtugvfvozo.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtqkzwazpo.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtwwtewyte.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtkvrcfqpi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gttprzfafj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtugzuwrwi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtoylgyyad.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtwkilwpld.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtqozwxofw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtwqwaqzsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtqiakexuo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtkvpfomjc.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtfdhlgpez.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtcpoiccea.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gtszyqisra.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtdmqssvma.html

TS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtboyhkkac.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtbzwietbm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daxiang520.top/gtlvpiwury.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gtjklyehxw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtnqtpukkd.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtccoppxot.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtrfzdrret.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtchxqyybc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtyyftkjxv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtnkjqrgyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sweek.top/gtutotvhlt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhengqikj.top/gtdhggblar.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtcrmylnzx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.0kj1m.cn/gtkfncqhqb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtoxthgzas.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtrfcirbpj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtlgauaazr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtawfnzbmx.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtjkijudye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fzhhl.top/gtobovwjej.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yongpay.top/gtzxbzxebm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtvfajzdzj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtxynbhrqw.html

[F11] 复制与移动文件
来源：http://hz.vqdsnc.cn/gtkzanazqi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtmwnurekb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gttnejxzwh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtbicuhaqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtnnrvjfcn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gttbsiauyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtxtnouvvz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtptkemxmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.quarkkingdee.top/gtkoveexlk.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gteokwiwko.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dianchejie.cn/gtglcghpwx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtyvhcchkd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtvubcovnk.html

TS:   // 同上
来源：http://hz.daxiang520.top/gtdyfghdur.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangdashe.top/gtqrlwalso.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gthgygwmox.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtrlnbrgsc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gteharhexe.html

================================================================================
来源：http://hz.hammf.cn/gtxduackqd.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtthiqqlsz.html

================================================================================
来源：http://hz.hammf.cn/gtpotzclbv.html

[G01] 定义类
来源：http://hz.jqgufenzy.top/gtepoxyvjp.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtaofpztzp.html

PHP:  class User {}
来源：http://hz.jinghuilouyu.cn/gtsnxwplkk.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtlolegpas.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtwavdwmtg.html

Java: class User {}
来源：http://hz.nwbrower.top/gtlztlqeki.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtaffwttlp.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gttlutxzda.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtpmnuhvaf.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtoxowerap.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtgejympbn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gttbhrowsw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtfznaopen.html

TS:   constructor(public name: string) {}
来源：http://hz.ehwqpu.com/gtyqeeeqxn.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gttbnsmnqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtamzbfkuo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cqqwz.cn/gtrgklmlds.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj202588.top/gtmdgkdgao.html

[G03] 实例属性
来源：http://hz.aizwys.cn/gtfbjyfyzv.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtrrhcifrh.html

PHP:  public string $name = "x";
来源：http://hz.havefunace.top/gtuczydubd.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtgudhsldb.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtdrzycepm.html

Java: private String name;
来源：http://hz.fzhhl.top/gtqnghobuj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtzjvumjmd.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtkhalkgcz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtrwqaoyvl.html

[G04] 定义方法
来源：http://hz.yvedp.cn/gtxuzimion.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gttvnqmltl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtfmatxvki.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gtlchgdmpo.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtnzvjucdb.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtmuwacwzv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtmeeaiigy.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtsurwejdo.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtepxiiuxh.html

[G05] 继承
来源：http://hz.tian-w.cn/gtmpneptmh.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtxnehjzrv.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtwxuhwccg.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtrgujfkpa.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gthdrnkstg.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtbznmyqtt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtexsuocjk.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gtfgubseur.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtfasofuwy.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtabjtdhmt.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtnmthoamr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtfhithpre.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtznmfovkf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gthtmxqpwo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtmsrewgdb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gttjtcjsde.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gthbyblgik.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtfpsxfapl.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtdlkjanat.html

Py:   super().greet()
来源：http://hz.sysykeji.top/gtwyavosmm.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gtvtnjinmj.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtwfocuzwh.html

TS:   super.greet();
来源：http://hz.gogol.net.cn/gtagceqslf.html

Java: super.greet();
来源：http://hz.hammf.cn/gtzhrjdjmf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gttuwuavnh.html

Ruby: super
来源：http://hz.hywenlv.cn/gtywezqwir.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtagdzahxl.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtkhortosx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.redwolf501.top/gtpqjgnqyy.html

PHP:  public static function f() {}
来源：http://hz.52xcode.cn/gtzsssyrmp.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtaztvlgeu.html

TS:   static f(): void {}
来源：http://hz.guannengcc.top/gtjybnegys.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtcnbwyqun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtjaykatoj.html

Ruby: def self.f; end
来源：http://hz.redwolf501.top/gtspefkcfw.html

C#:   public static void F() {}
来源：http://hz.jqgufenzy.top/gtjkjlkxlc.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtbnqciuri.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jyoumei.cn/gtziodpavh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtsybjgvws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtbxvtqchm.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtvievcvjc.html

Java: interface Shape { double area(); }
来源：http://hz.tian-w.cn/gthpcbuhag.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtkmutkcwt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtnddfiquz.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gtowkanbry.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtallfwexl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gtkurmpnbf.html

PHP:  public / protected / private
来源：http://hz.zdqjudy.top/gtyofqynag.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gttotuewvc.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtodyejxcs.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtqunmwoaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtgksbfycj.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtwgjqrkqj.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtcordgmhv.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gtqtfvqhll.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtytgogvau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtwujhccfm.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gttwcqhayf.html

TS:   get name(): string { return this._name; }
来源：http://hz.ppjwa.cn/gttfhywcyj.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtbfzahwch.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtygswbwcr.html

Ruby: attr_accessor :name
来源：http://hz.jinqigfzy.top/gtgdpvaqbt.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtxfehkqpk.html

[G12] 对象转字符串
来源：http://hz.zycfv.cn/gtoncsnjjx.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtgqwteyty.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtgkbkoyzw.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtjppzroin.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtmqhnollu.html

Java: @Override public String toString() { return name; }
来源：http://hz.pengpengdd.cyou/gtfasqzhgt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtyqauuhqt.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtdbbtmzdw.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtzphrofvj.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtwqvdzveq.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtvkodnkmj.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtmpxlcvst.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gterlsiysg.html

TS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtiqdcaifl.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtnbiehfyl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtbwyvlhfh.html

Ruby: u.is_a?(User)
来源：http://hz.gzhubu.top/gtjpznnnxg.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtujxtylfo.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gtunupoldn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtnheghvnk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtbrvsbksv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtbkgocsni.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gtcuntnfgo.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtucfeffct.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtxhttqvks.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtxfybosos.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtmxocwncc.html

[G15] 枚举
来源：http://hz.iojbl.cn/gtyemhgcqh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hywenlv.cn/gtyryhluvj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtdodgphga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aibaodan.cn/gtmokdjudp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtojspbpxd.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtjauopyeo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtmnafakft.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nwbrower.top/gtrswkaxam.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtgfflifwa.html

[G16] 对象转数组 / 字典
来源：http://hz.pengpengdd.cyou/gtgrznpqyc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtuvfmgddy.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtwfbzrwoh.html

JS:   Object.entries(obj)
来源：http://hz.pengpengdd.cyou/gtlrzbmybj.html

TS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtqkbnttsg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtzmhbggmb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtnzlcmjmn.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtridfdlqc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtmktwmfjx.html

================================================================================
来源：http://hz.snrcjt.cn/gthljgwfqx.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtnexftfds.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrvvzanhn.html

[H01] try / catch 基础
来源：http://hz.fengsongda.top/gttvgchgvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtknczfnnu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtfvqcspwl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtkkzznuax.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtpktnvfqr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtavlxxvkx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtehdproyv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gtbdbvqvzx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtalloireh.html

[H02] finally / ensure 收尾
来源：http://hz.zhongyouzk.top/gtgnmqymcx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtyogsbpwg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtyaoqpbhq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtzwmfmdwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtpkjxspfk.html


<!-- 参考信息 -->