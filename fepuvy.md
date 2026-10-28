代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fengsongda.top/gtznxmighd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtqxzdgalc.html

[E16] 数字千分位
来源：http://hz.shanyushiyangkeji.top/gtnysjvsmu.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtobnncjht.html

PHP:  number_format(1234567);
来源：http://hz.yonumen.top/gtjcuwdlud.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtjohplcqb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtxouquuej.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guowangkeji.top/gttmifzsmr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhongyouzk.top/gttxybegso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258.top/gtwaqfustg.html

C#:   1234567.ToString("N0")
来源：http://hz.cashguo.top/gtxeaiurnt.html

[E17] 首字母大写
来源：http://hz.ivvv.top/gthecrzsjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gthofxyiuk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtrvqftfzn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtmmqziath.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gthocmfhsi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtbsngfzwv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtopzqbmid.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtjlcoeelz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtfqchatzd.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtbaxmocxs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtdodeoqdc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtqdanqkls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtckpvzzoa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtliwlubho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtzvrxxqlc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtcwtzvjzn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtkzzanwxv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtetxoieem.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtinkoomuo.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtehavsfwe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shzxlz.cn/gtudmcjvvl.html

JS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtdxdrmpls.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtivkakczt.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtsweowgmv.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtycuqnemj.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtmjhftplp.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtckcuoanx.html

[E20] 判断字符串是否为空
来源：http://hz.smart0.xyz/gtikvdlgus.html

Py:   if not s:
来源：http://hz.ybcxt.top/gtxaijxfxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtknonyjds.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gthtixkcrz.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtxcbdxlwq.html

Java: if (s.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gthdktdtvm.html

Go:   if s == "" {}
来源：http://hz.chenzaomai.com/gtwfncqadi.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtqfbqnqbl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtldfrjdcl.html

[E21] 超长截断加省略号
来源：http://hz.tanke756.top/gtsvfkupgv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtypkxolhn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtibhrphyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtekoyjozv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtvwgzccpl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtkwbkpmkq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtouxcejtg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtooojzsaj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtjypitada.html

[E22] 字节长度与字符长度
来源：http://hz.ybcxt.top/gtsnlxwuty.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jiagoushi.top/gtpjqpdapo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtuefafdpw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtuybgupmf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtipyjbpqa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtwrinykxy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jianghu66.top/gtrbliimbt.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtnfdbohgo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtldlbedjf.html

================================================================================
来源：http://hz.zhixingplan.top/gtleonkmoq.html

F. 文件与目录
来源：http://hz.yonumen.top/gtsifmjjqu.html

================================================================================
来源：http://hz.xinyue.icu/gtdaqsabys.html

[F01] 读取整个文件
来源：http://hz.hysaishi.cn/gtmeemycmf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtcpvjorqa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtmqfpcubn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtkkrufgxl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtgotgutyt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtoscmoofn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtiitodonx.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigfzy.top/gtnxtlavnf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.mhx1999.top/gtsfakrbmc.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gttotlgony.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtmkewkrub.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pengpengdd.cyou/gtpimnblst.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtvpgydbyk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtcoiajdrd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtysjqbfnt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtfwxdtcxj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtucoeqgkn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtzotbycrn.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtpzfmspmb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtgmlxrabl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ivvv.top/gtbfolojmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtijbazuyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtadxnaehj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtfhupwkac.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtbslmyrhz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtuprtwlyp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtxvozfzau.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtlutwenzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtcokvbhzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtynvdnlvc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtkpepxmcj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtmkrayltw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtlvrzeuhs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtmpwnkhee.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtegsrzzcm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtbsigzxiy.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtarnuznig.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtltesdfsb.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtpsgxhbjj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtrvkoixxx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxqcgikaa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtkejfvhcl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.havefunace.top/gtmjqswsnn.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtzzumqbpd.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtdgcjnizg.html

[F06] 删除文件
来源：http://hz.cheryme.top/gtsqubfpla.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtsqsbtcxt.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtabrgovfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtfnbfgava.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtimgifwci.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtzmgvnsiv.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtsigahqcd.html

Ruby: File.delete("a.txt")
来源：http://hz.pengpengdd.cyou/gtqwcqhvdu.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtnaadizvm.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtjxbmvzgu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.0kj1m.cn/gtbrgtvrxc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gthdyiwnob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtljvoojkc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtyorfqfuw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtemwcbphm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtbgfatvgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtkydgxokz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtwqtoqzbu.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gtqfvertgh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtoiqibffp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gotoacloud.top/gtwipdspdd.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtkaynbxhk.html

TS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtyhmmxcwl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tian-w.cn/gtpyvuuefl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtxldqjymd.html

Ruby: Dir.children("dir")
来源：http://hz.iojbl.cn/gttfdckfgt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.316326.xyz/gtjzwwkqli.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtmqbetbuy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtgzsaqixp.html

PHP:  filesize("a.txt");
来源：http://hz.havefunace.top/gtsmgvnbou.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtxijaqufd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtdaoglomo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtjaojbtqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gtogjwqdjw.html

Ruby: File.size("a.txt")
来源：http://hz.cashguo.top/gtouzkmzpr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtmknenuhh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tianlin.xyz/gtfzmdhdnu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtvrrezooh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtfhjtbgut.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtzjftcves.html

TS:   path.extname("a.txt")
来源：http://hz.yvedp.cn/gtlkpfgbwb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtaobpnkxl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gttuxggspe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtmswwwzma.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtxumhxatg.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtmvrprjbg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtekuasfnb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtadywvvwi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtapdqhbxm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtdkgycqjk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gthzynfcas.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtddbsfkpn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtrznnqcuf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtwxugjrdx.html

[F12] CSV 读写
来源：http://hz.hywenlv.cn/gtiygkvvli.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtuoahzfwy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tian-w.cn/gtxqhojfpg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuxming.cn/gtrlrdubmq.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtluksjcxt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtxfzpmjkt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gtayqazddv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtncezkapa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtrolqhwow.html

================================================================================
来源：http://hz.cqqwz.cn/gtkotfdhcc.html

G. 面向对象
来源：http://hz.cucudq.cn/gtfbrowwof.html

================================================================================
来源：http://hz.haohaochexian.top/gtpzzwagcl.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtazlcrkqq.html

Py:   class User: pass
来源：http://hz.cashguo.top/gtyawtqakt.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtklyiwvql.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gtjwrlsyzl.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtklcoklxr.html

Java: class User {}
来源：http://hz.ivvv.top/gtrjellvoc.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtvuktvrng.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtavpfblvo.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtyqikxnwa.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtohsjkvra.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtojlgxgbc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gttcqpzany.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtkatutwho.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtablaxiuu.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtcfyikzaw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtnzrcaufo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtnjzlifky.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gthzizxudq.html

[G03] 实例属性
来源：http://hz.gzhubu.top/gtlchpjjzr.html

Py:   self.name = "x"
来源：http://hz.nwbrower.top/gttwgkkvmq.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtebpjfziv.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtsltwtjcu.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gtpssuhrub.html

Java: private String name;
来源：http://hz.gogol.net.cn/gtvabtgloi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtmaolnjau.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtltinsvsk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtniidwbgn.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtqjvwspkl.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtpgletgpb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtqamounql.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtlwvalfih.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtwywvghei.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtgbnutnyi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtapwgcbvk.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtlvexisfu.html

C#:   public string Greet() => Name;
来源：http://hz.yuxming.cn/gtxzqysrlu.html

[G05] 继承
来源：http://hz.52xcode.cn/gtjzxajkkc.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtqqtpqmuv.html

PHP:  class Admin extends User {}
来源：http://hz.haohaochexian.top/gtuvzahwfk.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtxiawjngk.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtrrvnxihm.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtwktuncov.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtgikujiri.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtrvpbjsmf.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtxxkcsmew.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtfxnfanzk.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtlfbrcyhh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtyrvdqhhd.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtonrserrf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gttlrcrtqp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtmcaganhe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtcrntambf.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtmlqcqefx.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtljctedqo.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtxefkzpkj.html

Py:   super().greet()
来源：http://hz.yuanzhike.top/gtwtvpqwqz.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtagfvnehc.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtglnlaivu.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtaycdnauy.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtyftlbmhm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtfkifjenn.html

Ruby: super
来源：http://hz.zycfv.cn/gtnslbklob.html

C#:   base.Greet();
来源：http://hz.jinyuanbaomall.cn/gtnhapjbon.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtautcosow.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtjmlwaoec.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtzuqflooy.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtxyugpwoa.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtewhngxvw.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtolthoepe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtqbteendw.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtyhsipwsq.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtnqedelms.html

[G09] 接口 / 抽象类
来源：http://hz.nanxinkj.top/gtjxeexzhr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtjnkhdyhq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuxming.cn/gtmdopkkbf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigfzy.top/gtdxiemnwv.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtznejtdbd.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtcjeqaiht.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guannengcc.top/gtmwaltrcu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtrdezauga.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtqzscgltk.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtlijnpdmx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtgvumxtdk.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtodnajztb.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtzxbvbwsd.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtgsjdzzbq.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtqbstwsju.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtknumbpuw.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtazapknnt.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gteskhcleh.html

[G11] getter / setter
来源：http://hz.shuidangran.top/gteuxfiqzf.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtlaxbwiwm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtdmrwxrly.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtnazurqrx.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtyiljtecw.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtgtdenkju.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gtpwykkfcw.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtvwymjkpe.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtoeulpclo.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtqzhjtpov.html

Py:   def __str__(self): return self.name
来源：http://hz.meibo888.top/gttzorzhdw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtomstgbkh.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtskfujrhu.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtyfsngpnn.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtjzuhommj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtyswqsobu.html

Ruby: def to_s; @name; end
来源：http://hz.vqdsnc.cn/gtxtedgatj.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtjcdavacj.html

[G13] 判断对象类型
来源：http://hz.nwbrower.top/gtylpltglr.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtbumgauyh.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtqpihqrcz.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtyphgvxsr.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtnfgarfeg.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gttpfxjmyw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtnmdcerii.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtwbbmqqvy.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtqtnihnqe.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtijtxmamv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtknntpdmt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gthdouguwn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.vqdsnc.cn/gtsjtbdbhe.html


<!-- 参考信息 -->