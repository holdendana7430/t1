代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydjk.org.cn/gtoiflflrf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gtesbvyvpq.html

[E16] 数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtzuxoiwfl.html

Py:   f"{1234567:,}"
来源：http://hz.hfpthk.cn/gtwgazkkbo.html

PHP:  number_format(1234567);
来源：http://hz.shangyingyoupin.top/gtivuspopn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtoqhqajxd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtawvyflqt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtfiozspqw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gtbeebljne.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shzxlz.cn/gtblvcphec.html

C#:   1234567.ToString("N0")
来源：http://hz.svipenyu.cn/gtcarmxvwa.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gthdcvibzc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhixingplan.top/gtzjnvazxr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtwyrayfow.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtvmhgjrxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtukxosyjy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtiuqfkmqd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtimnotfrc.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtxxskmjnv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtuevugjhl.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtgajxyydv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cdnleiting.top/gtvzfctbja.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtsejdysqu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gthqxcqjsk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtlwoopnba.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gthvqiunsq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gthrbqyljd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtatcfoiqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtlyukeeuu.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtcpizgpci.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtzyxhxpqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtowkjhthf.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtpjbxpqii.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gtbytxwpdf.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtpjzijrzu.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtamjacpre.html

Ruby: s.lines
来源：http://hz.xuanzx.com/gtwwmnbutt.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gtgmeaziml.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gttfxxbjns.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtahtqdjlm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shuidangran.top/gtauibfhgx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gtgafouavg.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtbcodxrpu.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtehzasynk.html

Go:   if s == "" {}
来源：http://hz.wangdashe.top/gtjxrieyms.html

Ruby: if s.empty?
来源：http://hz.yueranfly.top/gtcilygyyy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shuidangran.top/gtkdmzovhs.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtihitfrdq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtqqnumgjq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gtdmhjlswp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtsxgyycvg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtseahiank.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtgkudfxiy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuanzx.com/gtsqfbptpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.52xcode.cn/gtpmnmwlmm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtruqnzstr.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtudawdufk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtrmvoqywk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtvxhzoygj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtlnvmygrm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtahieteoe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuanzx.com/gtevodbqey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtujgowllj.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gttlfvnovi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtdmrumyhi.html

================================================================================
来源：http://hz.hammf.cn/gtpnsifutw.html

F. 文件与目录
来源：http://hz.hnqzz.top/gtylfqjixu.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsuvsghpj.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gtfgmzydwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtsworzyyy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtcduwzwdd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydzc1.top/gtedvouqzc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtubuobqpl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtfjkkotte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtrcpiguhh.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gttlryosdt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenjidiqi.icu/gtftyjroqi.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtfqgzfaey.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtjmasfoxp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtlngvmulo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gthuxrffmz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gthmisokwn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtqzmsxorg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgufenzy.top/gtlruwtakn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtguifdvvm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gthfkveeoy.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtogdjxayt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gthshcjscv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtqfgujbhl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtmdzhlepa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtfhrkawnl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guannengcc.top/gtgzxbhmwn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtkyzksrgr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnxiangtu.top/gtaloilyur.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gtfsdjrepj.html

[F04] 追加写入文件
来源：http://hz.zhengqikj.top/gtwvypcwya.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtukrisocv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtnnlgsyhg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtwlfjngzo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtueigzawn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtzzbkwjfq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gteahazuye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtokprvydg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtdvqzmbhl.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtiqvtehdi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtmdgtcgqh.html

PHP:  file_exists("a.txt");
来源：http://hz.yonumen.top/gtiousulxq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtezhihzea.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtfbynoqlk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtdygxgyas.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtvdwcexip.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gthocntsjj.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtypkkbfqo.html

[F06] 删除文件
来源：http://hz.zhoulong.xyz/gttzzpdtyx.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtemoqhzca.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtjfhotfly.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtjklpiqpb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gteqsphasw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtgwtmuwtf.html

Go:   os.Remove("a.txt")
来源：http://hz.havefunace.top/gtcoyqhnzo.html

Ruby: File.delete("a.txt")
来源：http://hz.aibaodan.cn/gtwloldgkr.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gtglnysuos.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtfmkwenkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.52xcode.cn/gtzicspjoy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtjtwdndoi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtfkmptybl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtrhszsczx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtgciodvqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtwhnsvbkn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.52xcode.cn/gtwdaolhfd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtdtubufvd.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtgtsogspw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgufenzy.top/gtxsgklirr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hysaishi.cn/gtipwclwyr.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtzeibbkmq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtcaebymwd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtmvtaptxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtcnsgqarv.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtkoygucvi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.feifeiyinyue.top/gtpoteeray.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtyefagcmv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghu66.top/gtflprzjse.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtvhuajkfj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtahpepjib.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtbcwqaiee.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtqkjfjsne.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtiwwanwif.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtjszlfdtn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtorljjhfe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.bjfxy.top/gtfrxuxsoa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtwdkszpim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtimgguuhy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtetlkkeyr.html

TS:   path.extname("a.txt")
来源：http://hz.gaohongyu789.top/gtczpgvkbj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtrrvbehgc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtxyrhzmxy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtjnvucujx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtrobfvtec.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtklxmuhim.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gthzawljbx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.mhx1999.top/gtrsmcjssd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtdurrxynv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtirkhaupf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangshuangyany.cn/gtngsfjesd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yueranfly.top/gtwafepixz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtsulggmki.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sxryk.cn/gtbykpbyjc.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtqjvwwsnv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtjaabeuar.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xylfe.cn/gtlxhipwvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuxming.cn/gtafpbhaex.html

TS:   // 同上
来源：http://hz.tanke756.top/gtdaqoawdy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtpevpcyxz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtkapdigrk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtutadyxah.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtzchoizqx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtujbhzags.html

G. 面向对象
来源：http://hz.yvedp.cn/gtytbjfbqi.html

================================================================================
来源：http://hz.guowangkeji.top/gtnyhzmmcx.html

[G01] 定义类
来源：http://hz.yonumen.top/gtkdcpewwd.html

Py:   class User: pass
来源：http://hz.meibo888.top/gtfxtiawka.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtynhyekwv.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtxinaaqvx.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtbypyecco.html

Java: class User {}
来源：http://hz.yongpay.top/gtdtmkwrci.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtsmdmuvzc.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gttytsuowm.html

C#:   class User {}
来源：http://hz.aibaodan.cn/gtibwvhwpx.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtpgeltmef.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtvmbooctb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtgmcldgqi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gttlrtduoe.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtvrqrurhc.html

Java: User(String name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtkchawdiw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtnxkssrgl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydjk.org.cn/gtpsatsldl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yueranfly.top/gtygsccpki.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtzknhrcfg.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtzgqtunbm.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtkbilrkhw.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtpiioqjse.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gttkroshyi.html

Java: private String name;
来源：http://hz.hongshengwenyu.top/gthmocbpqe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangshuangyany.cn/gtbqnbkxay.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtaqycnxlo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtspwlpvxy.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtdypzzmpn.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtqfxlhhlc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtvkhmsifu.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gthrgxjzwj.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtrvfiifuz.html

Java: String greet() { return name; }
来源：http://hz.jyoumei.cn/gtyjafntbm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtapecfnck.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtjyifjdtb.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtzhgclrqq.html

[G05] 继承
来源：http://hz.yj20258.top/gtauflthcu.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtznlcqwrb.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtnxulsajx.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtsmunawku.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtwqikbxne.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtbawsmria.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yueranfly.top/gtaygwryfa.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gthoovdnbm.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtktlktuce.html

[G06] 重写方法
来源：http://hz.zycfv.cn/gtveekcujz.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtcjjfntee.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtmwhubddw.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtpcdheqtf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtkugmzwxs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtecyoxngt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xinyue.icu/gtldihdoyg.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtotleuesg.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtinzvcxbx.html

[G07] 调用父类方法
来源：http://hz.ehwqpu.com/gtulhiqjdt.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gtqlfeqoal.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gtjzemdbep.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtneoafnis.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtzzchyxik.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtrdmdchze.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuetiantiany.cn/gtwllpvvdp.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtretgzypc.html

C#:   base.Greet();
来源：http://hz.ppjwa.cn/gtxzfyohaa.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gteymodrii.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtnynoknyl.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gthjzxkypk.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtnxiksizy.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtnwzlbcnd.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtkiaddnvy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cashguo.top/gthagrdeix.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtdbslglzi.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtchnncxsj.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gtaxahhyzf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhoulong.xyz/gtdhxtrwrl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gtzyicnjga.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtswjndyjo.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtlgwscqdd.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gtxopjfght.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtcvxcjefl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtiizyoosk.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtmvpyadna.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtoiunlocp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtsblmegyk.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtyuudoqby.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtldwtvaia.html

TS:   public / protected / private
来源：http://hz.birdmap.top/gtvyvaxqao.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtpieazxsd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtevfbqcjf.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtfzeljcsv.html

C#:   public / protected / private / internal
来源：http://hz.xuetiantiany.cn/gtbtrfqftk.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtxvsuvppm.html

Py:   @property 与 @x.setter
来源：http://hz.xziqi.cn/gtnrywpjis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtoqylqmkz.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gtahinnplw.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtfiknybuo.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtjqzbojmr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtiqltcyaf.html

Ruby: attr_accessor :name
来源：http://hz.nanxuanxn.top/gtmhxyvlet.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtxqigakvl.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtamzjptmh.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gtmxzuatod.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtqnydzwsw.html

JS:   toString() { return this.name; }
来源：http://hz.havefunace.top/gtbzcaxhoa.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtcznzqoyl.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtpqgxdhtq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.haohaochexian.top/gtanpekrpv.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtmgszhljx.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtbqvyuyad.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtfspcnwpd.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtnqxslhpx.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtsnvfdnjb.html

JS:   u instanceof User
来源：http://hz.yonumen.top/gtzcqsoitr.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtlwerwcrm.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gtlzelvasr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtrpbzujys.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gtseykhjws.html

C#:   u is User
来源：http://hz.zhaomingkeji.xyz/gtpxsnpklx.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtqluhzpqx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtkaihmzro.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtdvyfgkin.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtjhimnyqg.html


<!-- 参考信息 -->