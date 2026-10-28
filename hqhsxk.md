代发 wailian999

[E18] 模板占位符替换
来源：http://hz.quarkkingdee.top/gtmzsmnxga.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuanzx.com/gtgdkjdtjq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtmsaqljfq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtvsdjabql.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtrjweihku.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtruwebxgq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtcptzguyf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtpqywyknh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtrqouxrfg.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtqlqddczl.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtckrapavy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gttqfwsidy.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtxijedyol.html

TS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtiyhnsizy.html

Java: s.lines().toList()
来源：http://hz.yj20258.top/gtfmmgorvw.html

Go:   strings.Split(s, "\n")
来源：http://hz.sufxvd.cn/gtzchxslpr.html

Ruby: s.lines
来源：http://hz.hongshengwenyu.top/gttidofekm.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtclpdbyal.html

[E20] 判断字符串是否为空
来源：http://hz.smart0.xyz/gtssamifgn.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtqwylndjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gttwonjaum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtzjkuhtmp.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtpbpmxfwz.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtdtyofemy.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtjbiccsrd.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gtivoyhivg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtczskcmvq.html

[E21] 超长截断加省略号
来源：http://hz.gogol.net.cn/gtnnbaxsvw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtpuufdxic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gaohongyu789.top/gtepgtbfdl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gthbuiguoq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtbtecejut.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtefwnoarg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtszsxcmek.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtjjfqardq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tianlin.xyz/gtfbtebotk.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtuukaxapb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtjfotjewo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtgclauizk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtlrgsoevy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtcdqbptlt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtrbxurbod.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gtbxltjscp.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtogqstoxh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtlbbbpbuc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtaujenwcw.html

F. 文件与目录
来源：http://hz.havefunace.top/gtrwkxdtee.html

================================================================================
来源：http://hz.ehwqpu.com/gtlqohcoyi.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtlkrqkpjf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtkfxoypmh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtbmgijizn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtvfunktkf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtngpeifub.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtupocewvq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.andypj.xyz/gtgbkwttmo.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtmgdeoznk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtzmmetbjf.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtejrlofha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtxjbunolo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gtlahuxhbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtiwekhila.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtwlodbtwl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtkvhvdnqq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtwbhybgnl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sxryk.cn/gtlxovhogc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtxfllspsj.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtltootvhd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gtaruxmski.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtwrhpwzqm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtvxykifyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtojbtqosa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gttubtqkyy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtqdrebxln.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtvkmstryp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtlkrdhmui.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtjnxqujmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtnylekidc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hfpthk.cn/gtgfaosonm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtvghyfdxy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtmclqirek.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sxryk.cn/gtlnndlqps.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtdaxaqjrc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtlmckgenb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtmavmsord.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhijiandao.cn/gtgtcwplvu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtajilbwmc.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gtqnlvtljd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtudfknmsj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtgyeplxtt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gttipvzfiz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtpicnfskd.html

Ruby: File.exist?("a.txt")
来源：http://hz.yongpay.top/gtfolckrtd.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtdhozgsvp.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtxnylvamy.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtofcgebxy.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtpambhhba.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtfzkwlkdu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtrkmovzyh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gthayurlck.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtaaawssoj.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtrhrrzsbv.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtgvpqumqi.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gthbqpohsv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtxvuejcsm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gzhubu.top/gtqltehppc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtbekpkyuj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtopclblgn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtfhmdwjpl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtxdjannjp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtkifzdksw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtfwllulza.html

[F08] 遍历目录
来源：http://hz.redwolf501.top/gtrdrcdhwq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtinkxcxfs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtxkqltfqj.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtppeetfwu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtaznvpkzz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtkykfjvle.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fengsongda.top/gtsglljjvp.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gttpwuqarv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtomsrcmri.html

[F09] 获取文件大小
来源：http://hz.gzhubu.top/gtpydorfqo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtmmxedzbw.html

PHP:  filesize("a.txt");
来源：http://hz.havefunace.top/gtmhckcdxj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gttgrobgvz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtzcscewdg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtovhsxwht.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtuyrrjqdi.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtnldecimy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gteseqjhcv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtdeffwktk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtthhiifni.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtyddtrukq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtyztaipqe.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtppehyanu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtzitastfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtlscjeaxl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtyyhqwxkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtfgefgskv.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtpaoaooje.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtchozzfot.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtnddkeudj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtcibjyxle.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtefnnpddl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtjjqnzvad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtyggknuxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtfdntyisf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtjknppmpk.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtjdqhkcmh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtlfckhcvu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtgnzgyned.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtzdfwpdjr.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtuytsmqeh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtavyjwpya.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtwotewhia.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtmhhjbnzm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtdilblvgn.html

================================================================================
来源：http://hz.sweek.top/gtupremhyj.html

G. 面向对象
来源：http://hz.andypj.xyz/gtozhyyuej.html

================================================================================
来源：http://hz.daxiang520.top/gtzckfzmuy.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gthuuofisy.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtkiiochjk.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gtnneyqsqu.html

JS:   class User {}
来源：http://hz.birdmap.top/gtrvxfrbzb.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtdsrzpscp.html

Java: class User {}
来源：http://hz.birdmap.top/gttwfduxoh.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gtbfloruqp.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gttorrkcia.html

C#:   class User {}
来源：http://hz.guowangkeji.top/gtzboimmni.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gttkexlqfh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtlqwxnmys.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtmrspiloi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtxaovhmkn.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtvrschfid.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtacugqwvk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtzjoedlld.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.c1oappe.top/gtjqvqhedx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtizveafcy.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtwefxyfzz.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtzagmanmk.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtpjwwyrcw.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtqwwxogmn.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtayqvzyfl.html

Java: private String name;
来源：http://hz.yj20258.top/gtteahigve.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gthcaxkbwq.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtnugcobry.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtftnabymi.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtslfoettv.html

Py:   def greet(self): return self.name
来源：http://hz.cqqwz.cn/gtqkoklqzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtptglzrip.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtlibefygl.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtprjumpst.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtaxgnjktr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sxryk.cn/gtfljykkra.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtlwnkqitt.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtbraxkciy.html

[G05] 继承
来源：http://hz.tian-w.cn/gtpmvdrfwg.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gturmqetkb.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtryswumiy.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtgzcvlnxl.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gthjdicjkb.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtahvmtkbe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtpxllrive.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtajrudqrz.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtazemlkxy.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtaoghjcuw.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtkwafgemh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtvqwbowio.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtytshczcr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtradjakfq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtaawcwpzz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtzuflsnqt.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtqnjxmdsn.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtokzwqjjp.html

[G07] 调用父类方法
来源：http://hz.yuanzhike.top/gtzrkqzkgh.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtdhoewryg.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtaivcvmak.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtszctvewi.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtggnbjbbc.html

Java: super.greet();
来源：http://hz.yj20258.top/gtevugiher.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtiotifayr.html

Ruby: super
来源：http://hz.shuidangran.top/gtgsudukmu.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtokndugbl.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtymwzrnnq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gthprkycjn.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtgezucuty.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtbbqnayxd.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtkmopponj.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtpjjivbwh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gteiujisub.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtszydhwsu.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gttrbfisia.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gteuhwcfpy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtwyrxiiga.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtkzdzkqws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gttjityphm.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtjuyjdwfn.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gtzrxoxprh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtedezahwz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtpllfhula.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtvdyamweh.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtesctnpno.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtmlkuiyba.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtjeaxgrvd.html

JS:   #private 字段；其余公开
来源：http://hz.zhiwuduotai.top/gtcicoxowi.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtlwxqafoo.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtqwwtrmgk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yueranfly.top/gtuvooljom.html

Ruby: public / protected / private
来源：http://hz.shangyingyoupin.top/gtwebzprne.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtveqckspx.html

[G11] getter / setter
来源：http://hz.hongshengwenyu.top/gtzgadmoki.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtbrcpvnwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtwhjbkrxu.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtvjasagfg.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gthqcereyh.html

Java: public String getName() { return name; }
来源：http://hz.dashuyun.cn/gtdzqcqlbm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtiitksleh.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtniwkypix.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtvypxpazt.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtonmepfxb.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtvmqstuoe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtytkspnvd.html

JS:   toString() { return this.name; }
来源：http://hz.jiagoushi.top/gtbguxlehn.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtudqqngqk.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtsszdhqpw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtecctqflq.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtjcgtoefh.html

C#:   public override string ToString() => Name;
来源：http://hz.gotoacloud.top/gtqwatmrjb.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtpfrctkqv.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtcorybuak.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtdwxnllap.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtspnzzwli.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtzgdonfji.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtqfwekqth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtnktwylqq.html

Ruby: u.is_a?(User)
来源：http://hz.yuanzhike.top/gtjgfsemyv.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtgvtmkuqt.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gtiwfxtwld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gthlsbscgd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gtoctpeoob.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtbkldsqiz.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtppvfkkjy.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtiftosait.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtdjhlqrje.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtwihqqnpv.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtorxjnccx.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtxhegdamt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtbaxlzvsv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtbkmmxetq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtbhjdpzee.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtyknmxclg.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtkaavxpwi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtmmlgyajx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xylfe.cn/gtpwptelkb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtnkfsbeju.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gthcrwvsfm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtjxkhghoq.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtqvunostv.html

JS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtmoajxlek.html

TS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtjzdabmkd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtgjmsakje.html


<!-- 参考信息 -->