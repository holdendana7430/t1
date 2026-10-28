代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtfwmyeqor.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gtnguyqgkg.html

C#:   1234567.ToString("N0")
来源：http://hz.guannengcc.top/gtastfrzny.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gtnimsoxqt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.0kj1m.cn/gtmvbfaura.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gthqsjwunu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtekotghxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtgfzeoakv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtzwisimvy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtpesxtars.html

Ruby: s.capitalize
来源：http://hz.tianlin.xyz/gtkeckrkex.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtazffuemh.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtmciseixw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gtzzpjzatb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hammf.cn/gtidnfstmx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtskfnpqmw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gttzkdkpwc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daria6918.cn/gtvounfaed.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtxujvfhnx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangshuangyany.cn/gtaqzscfqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtzbtdfsvh.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtcoyklxwl.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtnzcdszcq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shzxlz.cn/gtlaeudafp.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtjfincmgc.html

TS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtphzjasxl.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtqsxzkqyx.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtmdytqxeq.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtitzghpgt.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gtcvixjlzo.html

[E20] 判断字符串是否为空
来源：http://hz.yangfankeji.com/gtpkunerpa.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtqappcfkb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.52xcode.cn/gtszfvbspw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xinyue.icu/gtfzmfkjqe.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtdnwrgmgw.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtrarlxxhu.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtfsdfffaf.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gtpgqpirhc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtyztsdabd.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtwthdqbuy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xziqi.cn/gtnjvrkzbo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtyoyvffbh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtdjaiivlu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtymoqkjow.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtnnpqnbvz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shzxlz.cn/gtelfjcdri.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtsxlsomvg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtditlwovs.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtaywatqvq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtewbzmsin.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtxreehfgc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtjncbxopm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtomzwugra.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gttbllqqan.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtntlkbpdp.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtswuhtoyh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tian-w.cn/gtcdmwulhz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcwqsqknj.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtijoqzlyl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyeuroukd.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtzchbuifp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtomyuycdl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtipdzfpmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtiupykmwk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtfpnsbvaa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtftrkkvjh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtomodbwec.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtnedldhrr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.0kj1m.cn/gtrwkqfekd.html

[F02] 逐行读取文件
来源：http://hz.meibo888.top/gtbnxfgtod.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtlygbarki.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnxiangtu.top/gtzhpqqlzz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtpidbtjrd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtpcteruag.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtiayfmsel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aibaodan.cn/gtkiepcbdd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sweek.top/gtugihlcpu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gteftxhxss.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtijhuiffc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.c1oappe.top/gtkqyhexsm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtyvxsnlrw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtbixfxwqp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtdkskclry.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtlsasdtpx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtlptbfcpe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jlsjyb.cn/gtnnttgvnl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtnntsuckd.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gtqlvesfpl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhoulong.xyz/gtgxzunaxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtvbgabqya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtohajxbfx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtsndpbjzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xingfuxueyuan.xyz/gtzxvdslck.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtvixrhlqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtdwmtlmfo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtqfmwlpmc.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtvcxtpgig.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtwqqbpsmg.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtjafhlpnh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtsycawoio.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtrgbfvftl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtmttysncd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtezyaqccr.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtrommcmbt.html

C#:   File.Exists("a.txt")
来源：http://hz.zdqjudy.top/gttkypcbag.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtkohkdarm.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtqnuupodm.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gticzujfju.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtuhdccttv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtyukpxrhx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtnkboqtzd.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtsggomdvu.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gttsiblzpj.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtcxtxdycg.html

[F07] 创建目录（含多级）
来源：http://hz.haohaochexian.top/gtjpnlylij.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guannengcc.top/gtvswqbirp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fengsongda.top/gtzkjfhkgq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtucyudbwf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtrnlergru.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuetiantiany.cn/gtdwlpjobk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtsgdiayrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtbojikqnj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtxyerfmqm.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gtrlpxfksb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtbcqmuhbc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aibaodan.cn/gtjbndcndi.html

JS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtenyreuvx.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtyymvuada.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtorpytpej.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guowangkeji.top/gtspateech.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtgaqfxkjk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtvuikznfm.html

[F09] 获取文件大小
来源：http://hz.zdqjudy.top/gthmgefshm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtmafvofna.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtlojmypdm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtrdlydytn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtagliytha.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtomxuhaql.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtkdlgxath.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtpdkkvgyq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtpwztbmyl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtoqbxsoqt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtjjozjquz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtdbpzonyx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtczgigefs.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtyiexhljr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtycmkeglo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dianchejie.cn/gtrhljfyey.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtwqauqfsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtrhtrxvwj.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtxhgwsxyh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gttaklistp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gttmcufhdj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtvpgsruix.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtgzrzspal.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtguogaddl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gthtgahuff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtaibxvzlj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtbtdljskc.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtqupsjvlt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtmmqghjpm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtaoyltapa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhijiandao.cn/gttqpyvxtl.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtyduowjra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.snrcjt.cn/gtvjvfmmye.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtonpxfhhj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtkxqfzmwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtgbxtdqaq.html

================================================================================
来源：http://hz.fengsongda.top/gtieoqdobu.html

G. 面向对象
来源：http://hz.hnqzz.top/gtfhlfwfsu.html

================================================================================
来源：http://hz.ppjwa.cn/gtzkxuuymo.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtnzhbplfu.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtoujdnbzg.html

PHP:  class User {}
来源：http://hz.havefunace.top/gtrzmbuzie.html

JS:   class User {}
来源：http://hz.ydzc1.top/gtwvnmopdt.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtljnoakxx.html

Java: class User {}
来源：http://hz.birdmap.top/gtslzmzweq.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtnfajvdua.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtngewbsca.html

C#:   class User {}
来源：http://hz.shuidangran.top/gtchsferjw.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtuvdsxciw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tanke756.top/gttfjysahk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtvnrvxqve.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gthpfgtdxc.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtpnkvqyrq.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtgvsmrxtq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtgkyixlph.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtqhilhaso.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ywan-chungtsiang.top/gthyppylpj.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtglhvggkl.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gttqzgxcof.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtgrxlppno.html

JS:   this.name = "x";
来源：http://hz.cqqwz.cn/gtuxvvoxco.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtcqnsvvug.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtsizyeazd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtbrzyfgfd.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtgxncpewh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtuaboelzk.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtdtwsjnxf.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtvdftuehy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtobozhdwd.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtvwwvoiak.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtfqtzznxk.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gtsljfqjkr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sweek.top/gtqrpgxtqd.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtjjxvpzls.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtbmwawclh.html

[G05] 继承
来源：http://hz.hnqzz.top/gtlefkuuid.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gthfufdonk.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtectilavk.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtbmuokvkg.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtgcdlpazs.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtohxxuwfc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtqtucnbme.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtgfjhgxbl.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtfgbrpmjh.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtwbfwybvj.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtkxmkjsuw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtzbbwnirx.html

JS:   greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtoxzxsawr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtuehriysl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gteqolkcre.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinghuilouyu.cn/gteprysqkq.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtaclfgzap.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtbvdisfxh.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtbnvorbkh.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtkbjflqjo.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtoozbpeud.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtcxjierco.html

TS:   super.greet();
来源：http://hz.andypj.xyz/gtpeltflts.html

Java: super.greet();
来源：http://hz.jinqigufen.top/gtjvxayhxu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtgydebnkd.html

Ruby: super
来源：http://hz.pycfn.com/gtugckwvif.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gttcnuzupm.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtsthpctxl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cheryme.top/gtiukyjchr.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtgveepret.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtxmdsflaz.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtwkfhocxa.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtcrkmowgi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gtdjccwdgd.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gttnkoloeq.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtgzawtdik.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtppafzidt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtalpsfehr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtzsxudsvj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daxiang520.top/gtsykclqob.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gttutktpmi.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtlpiadwnn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangdashe.top/gtcqglfwnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtumjuyacq.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtthnhzcft.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtvfttamlb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtgawfgrfv.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtnppgyhff.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gtyvmutjxt.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtjnhiezel.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtmyjhkfjf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhongyouzk.top/gthznusxzr.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gteemslsjf.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtracbijaf.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtaqpmcyxd.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtuijlpayp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtmikthvnz.html

JS:   get name() { return this._name; }
来源：http://hz.birdmap.top/gtjfjkguqw.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtpkqyzgwu.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtltuwygdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtqutdbegl.html

Ruby: attr_accessor :name
来源：http://hz.aibaodan.cn/gtkdbvnrml.html

C#:   public string Name { get; set; }
来源：http://hz.ppjwa.cn/gtgjioafbh.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtsrainqzy.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtkossrvvr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtqbchlsla.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtvqocgtga.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtjdkmqglh.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtgxxquesh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gthfhgvdxa.html

Ruby: def to_s; @name; end
来源：http://hz.nanxinkj.top/gtbugraurn.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gttorucavl.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtrgokuigl.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtdaywglgj.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtejqtsfln.html

JS:   u instanceof User
来源：http://hz.cashguo.top/gtttxxmaqu.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gttnvxymsa.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtivywdbrb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtjssnihnl.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtjxyvyapr.html

C#:   u is User
来源：http://hz.yuxming.cn/gtftujbjxe.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtpnpzkjsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtohlbhjuz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnqzz.top/gtvlwqqaaf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtpuamsrvj.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gthmyldjjt.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtgasoacdz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sweek.top/gtrkqgnexg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gttdtvdjfm.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtesgsixcg.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtaxzkzvly.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sufxvd.cn/gtuowaqazp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgufenzy.top/gtxmmwljqo.html


<!-- 参考信息 -->