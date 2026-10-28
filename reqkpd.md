代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.birdmap.top/gtfgfucbsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtmjdnbzvj.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtjrkdtvgf.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtobytalzg.html

Go:   if s == "" {}
来源：http://hz.yvedp.cn/gtyzwftjpv.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtddwynper.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtnefllhzs.html

[E21] 超长截断加省略号
来源：http://hz.havefunace.top/gtxrvdvhil.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtcnuwszdr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtzibkihhc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtbibmjjdr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtbvdotftg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtlgufnaxr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtuurjnkyx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gttwsiuxfu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gtydhnylow.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtbveknujb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtczgybdar.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtnsqphwrh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtukqncwyf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtyhnibfna.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hywenlv.cn/gtlfcgqtfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtssxbylfv.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtnlwsifml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtjivtalru.html

================================================================================
来源：http://hz.iojbl.cn/gthuhfelrh.html

F. 文件与目录
来源：http://hz.pycfn.com/gtjziozttw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgidgakaz.html

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtunzbbfzn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtzuzsncdh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtyjczcwwa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtgvasxmqz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gthamqicvq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtoyeeijoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtpztzixbd.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtfjtruknz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtbzcpbfmj.html

[F02] 逐行读取文件
来源：http://hz.guannengcc.top/gturdicbjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gttwkuzppi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.0kj1m.cn/gtbjguknve.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtrxkdyvex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtozivaslw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtqqomwlyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtizgtmdxn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gttnzxttos.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ppjwa.cn/gtgtdesmej.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtbjffslue.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtdpuwwfcy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtomsgvtkv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtftvixdph.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtxxzscojv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtjaxodnos.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.andypj.xyz/gtnftjwjii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtmchrmpfg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtulkprvhq.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtifkbfahp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhoulong.xyz/gtqacnmixm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtrburxmgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gthmrhgjfe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtrxgedhup.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtnbvdjwnc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtcbxjpxmg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtcengeolp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtshzjuqpi.html

[F05] 判断文件或目录是否存在
来源：http://hz.jyoumei.cn/gtqfrxgjpi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtarfjivdo.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gttmfudgbe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtsoynseiw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtxxzjbxqg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gthrxdsebb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtxzcwzibf.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gtckgwfttb.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtttfjuohz.html

[F06] 删除文件
来源：http://hz.yongpay.top/gtrvlvgrsk.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtxrswynnr.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtczimwmlg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtebtcperd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtrjnyiako.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtxusrafay.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtyhdapnva.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtdaylurwk.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtykcblomv.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtxieqgure.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtwiskfgui.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtehilsfwz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtwvqsqvem.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtriimuoqr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtgzstciwq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtupzbbrwc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtremljhbz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fengsongda.top/gtlcuabpjo.html

[F08] 遍历目录
来源：http://hz.aibaodan.cn/gtykdiqwdo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yangfankeji.com/gtgwzvzxxa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtjcrugnbb.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtjpdviopk.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtnumoxonk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtotwlofct.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtcifulicf.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtdyxshfru.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtqymlqhtg.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtmbcgkjwm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtkaneoohu.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtbwcexsvw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtojbfkmgo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtomsitegc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtztpkqian.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtxyupjxva.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtkzcregwx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtbkvzwbbz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtsrokeuyr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gthlnjwsay.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gteuamkqki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtcuuubvea.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtrlqcxeet.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gtmgqyoswc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtjamerxpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtktejwhdv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtiljsvtlw.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtqdqqfjlr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtczklcmzj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gttujrjduw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtfinywvqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtjeoqpwvd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtpjtkwjzk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtyrrkswig.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtcbrdrltc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sufxvd.cn/gtnybarsvu.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtkppvucpw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cdnleiting.top/gtdgkrqcri.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtrvlhkwnk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtinmzcist.html

TS:   // 同上
来源：http://hz.cucudq.cn/gtmxxlgtbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gteekdxqyn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtmaidijpr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dianchejie.cn/gtckfklczt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hammf.cn/gtoecphmcl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnogtmgqw.html

G. 面向对象
来源：http://hz.sufxvd.cn/gtvntqusau.html

================================================================================
来源：http://hz.jianghu66.top/gtemkywmuo.html

[G01] 定义类
来源：http://hz.mhx1999.top/gtyelozsmj.html

Py:   class User: pass
来源：http://hz.zhongyouzk.top/gtrpitmudg.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtjzcbbfcq.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtibkeimey.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtchxdjmyg.html

Java: class User {}
来源：http://hz.zhoulong.xyz/gtmzftidls.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gttvycnjgr.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtmffgcnjg.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtqnzahoco.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtumcqpeav.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtqvoxahig.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gtqgounddh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtgqtsjqjo.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtjxndxdkw.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gttcxbkoms.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtgwnfoohp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtqtsmylyw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtzvyiybuw.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtmqkjokbf.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtuombssst.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtlchhcqlb.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gtocmsfmdc.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtiylusldo.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtugvttixm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtowkjraqj.html

Ruby: @name = "x"
来源：http://hz.shuidangran.top/gtktyyimcr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtweddvlmm.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtmilzlbeh.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtnwkgarkp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtirnsurze.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtewdsetht.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtyabrcrkm.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtgsfpjpoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtppvivfwq.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtgxiqdgdi.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtfxgzszua.html

[G05] 继承
来源：http://hz.xuanzx.com/gtiakkumvk.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtjnlcdomn.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtnvzzgpqv.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtqczxtier.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtepxgaswf.html

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtujzzqgwq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtxexhokwm.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gtkdgyaqaj.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtqxawokbz.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gttxfreoen.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtdlopbxnr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtagqlnecm.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtqosfbifp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtswdzxjyd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtmegdkdue.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gttwomaodx.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtwpgxgtjc.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gthgcznwqe.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtkqrchart.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gthlatbkru.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtksnefewi.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtroqxagmm.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtyzhssrbc.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtrelfhzqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtdfnfknyc.html

Ruby: super
来源：http://hz.aibaodan.cn/gtnvirecwe.html

C#:   base.Greet();
来源：http://hz.andypj.xyz/gtqjjliryi.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtpjlenyot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtvercllru.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtrsndkbmv.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtxdjsotdb.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gthoiwvnfw.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtrlmejtji.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sufxvd.cn/gtdpdrskjd.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtnbbskbgp.html

C#:   public static void F() {}
来源：http://hz.zycfv.cn/gtudemqitx.html

[G09] 接口 / 抽象类
来源：http://hz.zhoulong.xyz/gthhuomtkf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangshuangyany.cn/gtobendsry.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtqwgqztbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtkjmtiiov.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtbzukhhwp.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtjbngmwvj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigufen.top/gtwpavrchf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gtfhsrpyeg.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtatkfaepg.html

[G10] 访问控制
来源：http://hz.dashuyun.cn/gtzizndqaj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gthynajkjr.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gtxgccsset.html

JS:   #private 字段；其余公开
来源：http://hz.birdmap.top/gtfprfreri.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtqhpdkqar.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtwuohfrqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtjtlwosoy.html

Ruby: public / protected / private
来源：http://hz.jqgfzy.top/gtctevmglk.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtwvmnflvn.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gtqaqaqwzk.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gthouzhczl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtekwxripz.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtklctgwsq.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtelnuvize.html

Java: public String getName() { return name; }
来源：http://hz.yuanzhike.top/gteksufegm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gttgimblgz.html

Ruby: attr_accessor :name
来源：http://hz.yangfankeji.com/gtivtcmwhd.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtyrssxezk.html

[G12] 对象转字符串
来源：http://hz.nanxuanxn.top/gtkowtvqqw.html

Py:   def __str__(self): return self.name
来源：http://hz.chenzaomai.com/gtmcuapnpy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtxsuexght.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtwdbzdjma.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtcjudtugi.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtlmuhovzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gthgffivey.html

Ruby: def to_s; @name; end
来源：http://hz.yangfankeji.com/gtcpxrlwlc.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtkacufvlf.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtkrcjefhd.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gtellhbpmj.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtfsdpangi.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtqtzjjhvu.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtfvxhurme.html

Java: u instanceof User
来源：http://hz.shangyingyoupin.top/gtzuhqxmka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtgcrgsgnu.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtujcnwlov.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtjhozwphe.html

[G14] 数据类 / record
来源：http://hz.yangfankeji.com/gtwtbhcwpt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtamsvseyc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtkwisqijd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtcekiijng.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gtujsjchno.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtozjtpjup.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtstgqkwvx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtmonqdlps.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtabdxojup.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtqrmtgtse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtizyoyzbz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtwllcnrow.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sweek.top/gtieqckzni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtphnzgqfw.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtomyfzbuv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtlitfycho.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtzwutdhuy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtcuvrbhnu.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtmzjbgizw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hysaishi.cn/gttnekdoii.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtqkqzmllb.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtjineadsp.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtpcidtiml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtpiqzygbs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtdnkgxshl.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtxzahfzus.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtbgiquyev.html

================================================================================
来源：http://hz.smart0.xyz/gtwrisbthk.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtdglwmnkz.html

================================================================================
来源：http://hz.hnqzz.top/gtlqkrkvoe.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtsvxplvdq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangtech.top/gtfybqikue.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtglxgomcj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtntwyzeng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gttpvklixd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtcicowvaj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtpnklpejq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pengpengdd.cyou/gtvpdplbuc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtfjkllain.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtviudfmuv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtyfijzwma.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtqmwvljuq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtispebtjs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtdxausewt.html


<!-- 参考信息 -->