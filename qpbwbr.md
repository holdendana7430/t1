代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xylfe.cn/gtdyovtirf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtsaxrjvnp.html

[E16] 数字千分位
来源：http://hz.ybcxt.top/gtkkwahmio.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtrxikcsrw.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtkaurivrs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtiyhdquhh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtibprozsg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtbqpdcyyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtxkoqrrrn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gtdlsonkxg.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtiurigcsu.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gtvfufxhkl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtnxrngjcm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.svipenyu.cn/gtdjsgqeup.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtjbswatrd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtowlhfmip.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtqoabuumn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtidqfoxhq.html

Ruby: s.capitalize
来源：http://hz.chenjidiqi.icu/gtxuhkhsfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtcisbzwls.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtknearkgu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gtqpwygwmz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtfsmjfiox.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gttgzmbxes.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtevrcssca.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtoozursdh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtvzgbaqef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tian-w.cn/gtwmyierpc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jyoumei.cn/gtpniukrbg.html

[E19] 多行文本按行拆分
来源：http://hz.316326.xyz/gtzgbksxuw.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtomwygorp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtrbclslmq.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gthgvjxjej.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtvcuqezrk.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gtufxrqqdj.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtqafypdsj.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtofdcwleo.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtlvrryyle.html

[E20] 判断字符串是否为空
来源：http://hz.hammf.cn/gtzdfsvwbu.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtptpllnzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtkeqsxngy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuanzx.com/gtdfutxfhh.html

TS:   if (s === "") {}
来源：http://hz.vqdsnc.cn/gtzmzepfag.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtwxwkrrur.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gtksfhiedp.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtdostpzzn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtzahowsmd.html

[E21] 超长截断加省略号
来源：http://hz.zhengqikj.top/gteiiyqfzt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtaafnhxzj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtjsravicn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtosknogix.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtpfxnhjxb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtlpyyqhmi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtqbrelpkf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtpvdhvvop.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtirljjfxy.html

[E22] 字节长度与字符长度
来源：http://hz.pycfn.com/gtvaeobygw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtzchscmlq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtujxfhmgq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtukqigeow.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtvfzoxjin.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhaomingkeji.xyz/gtjmvofzry.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangkeji.top/gtlsvivqhc.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtxynzsugo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.iojbl.cn/gtinwwkbfn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtizaczfvo.html

F. 文件与目录
来源：http://hz.mhx1999.top/gtejiwthlg.html

================================================================================
来源：http://hz.hywenlv.cn/gtiwnzuxku.html

[F01] 读取整个文件
来源：http://hz.iojbl.cn/gtysayolun.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtefrfqnma.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgufenzy.top/gtiglwfhji.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtfpfjdnni.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtiavkjpqh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtwjjwzqiy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gtzpfzlpgf.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtmhhnsefa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydjk.org.cn/gtadlawatn.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtnkwbvnlq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtqeztcjam.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guannengcc.top/gtpntcksei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtstbegbgt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtnspciivn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtdeqfuttm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xinyue.icu/gtmmeggict.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.svipenyu.cn/gtnxoxrzse.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hysaishi.cn/gtsneoxvhz.html

[F03] 写入文件（覆盖）
来源：http://hz.havefunace.top/gtumkvrzlh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtdfpwsijz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtbdusgftj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtixsqgvrm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtpcgzpqzh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jianghu66.top/gtzlqljlgc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtesonddqh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.havefunace.top/gtybbgiwny.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yonumen.top/gtwfkvqoww.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtbbipnhsz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtlavfnefd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtnvcskxlp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtfivhsfdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtfoxqdqbi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gteoprqbpv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtkbyhrmxo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtnpeyofdn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuxming.cn/gtppyabtkb.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgfzy.top/gtepzvycnw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtkrtiwglk.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtfosqmqud.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtldrbqryq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtczmbkzcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gttgjorutm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gtvvqyozmb.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtlnrvjoog.html

C#:   File.Exists("a.txt")
来源：http://hz.52xcode.cn/gtccoqicxw.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gtnrekchgs.html

Py:   os.remove("a.txt")
来源：http://hz.hysaishi.cn/gtfnxdknqg.html

PHP:  unlink("a.txt");
来源：http://hz.yongpay.top/gthbhliqjg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtyqqymhrn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtlgqngryv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtomhkakru.html

Go:   os.Remove("a.txt")
来源：http://hz.kuanghao11.cn/gtvjaatxwh.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtuyjixgav.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtqcmhngzy.html

[F07] 创建目录（含多级）
来源：http://hz.zhengqikj.top/gtvhhpcqvx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtqbwxvzgu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtvootsxnl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtszcivzpp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtfxmabscc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtrunsebih.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtyztixymu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtqvotpgty.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtabbmoxjj.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtqaxfinrm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtxhbrjmfs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtkxyawdpb.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtsroujkfo.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtfizzxtip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtzidbrcjf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtbgzugyfs.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gthyavxjbe.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtyhfruyqg.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gtuwmjrmwe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtdrprvuni.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtpcrfgpka.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtgsqmkvay.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtubkoorme.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtohzbsvcc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtxpsutzxr.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtlclksuil.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtucgdzibw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtjhfhevky.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtdnosbnaj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtlqtytgsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtoqcilnut.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtyiffgwfj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hammf.cn/gtrvbzzrut.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtydlwvnwp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtpqxvmuqh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtpqhqjuvz.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtobvlnyek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtabshirqf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtecvqolfs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtconrfzlj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtdybegosk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxuanxn.top/gtxvqxeqew.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gaohongyu789.top/gtvbzretqa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtsxriaefb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jyoumei.cn/gtqfzdwdro.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtbrzauejk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtofasiejc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtyvdgpunf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gthymofvqt.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtlcarxfdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pengpengdd.cyou/gtamkwdmdb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtsxmrtdnt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cucudq.cn/gtexxsiwrx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nwbrower.top/gttsxspckk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtosjdqxpg.html

G. 面向对象
来源：http://hz.xylfe.cn/gtjdfzziji.html

================================================================================
来源：http://hz.gaohongyu789.top/gtaczozbxo.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtucwsbnqp.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gttenczfkw.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtmynyxbef.html

JS:   class User {}
来源：http://hz.zhiwuduotai.top/gtoxajhyvz.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtimmmvsoa.html

Java: class User {}
来源：http://hz.zycfv.cn/gtofknwdih.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtvygyoohe.html

Ruby: class User; end
来源：http://hz.zdqjudy.top/gtgtqmnvpw.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtqcjhzpjw.html

[G02] 构造函数
来源：http://hz.yj20258888.top/gtosjotfvs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtdlrxhqmw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydzc1.top/gtgnumhibz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtzsrvzvrl.html

TS:   constructor(public name: string) {}
来源：http://hz.zdqjudy.top/gtrknsdoak.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtfautvoyo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtyxxqxjvg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtacpljbds.html

C#:   public User(string name) { Name = name; }
来源：http://hz.kuanghao11.cn/gtuayjpeaf.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtulfxgvtq.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtnhqkalob.html

PHP:  public string $name = "x";
来源：http://hz.daria6918.cn/gtkfdsnljx.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtxuizapxp.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtmhqvzbmu.html

Java: private String name;
来源：http://hz.cucudq.cn/gtzjezxlls.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtzycoxbwb.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtkchwlzfl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtgtwruvow.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtkiovotkk.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtxzkzdueo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gthezzqrvf.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtfieubhfd.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtnpvaougj.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtylkjdyjt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtgqalmcfo.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtnragqfgm.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtslwaypkn.html

[G05] 继承
来源：http://hz.ivvv.top/gtpxqdjztp.html

Py:   class Admin(User): pass
来源：http://hz.zhixingplan.top/gtmvndcwyh.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtrshextby.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtfjqoxxmi.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gthxqnxrjs.html

Java: class Admin extends User {}
来源：http://hz.ybcxt.top/gtkhflovkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtervendtn.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtilzbkpzs.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtxzdduhfh.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtsokrwbjz.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtcioollot.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtbwylqtcv.html

JS:   greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtbihborpy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtinjndttw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtlidksmqi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yonumen.top/gtpckvzkbs.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtpdyhwmvc.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtlaozeavs.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtiklzcovt.html

Py:   super().greet()
来源：http://hz.yongpay.top/gtouumnkqr.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtmxjiilmb.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtpgpzpbon.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtwdhcekeu.html

Java: super.greet();
来源：http://hz.snrcjt.cn/gtjkfvznas.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtuydnltsr.html

Ruby: super
来源：http://hz.yangfankeji.com/gtnogckvpg.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtuxlvkuhe.html

[G08] 静态方法与属性
来源：http://hz.pengpengdd.cyou/gtgrecbwfs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtiucwqdix.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtfgjpdokh.html

JS:   static f() {}
来源：http://hz.cdnleiting.top/gtgflkipsv.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gttujhxbch.html

Java: static void f() {}
来源：http://hz.vqdsnc.cn/gtevvwhlii.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtrbuamltv.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangkeji.top/gtljmlzzol.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtdcyutpzz.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gtrnayxmyi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtaugoguhl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gthjtehhtl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtiyrbxjih.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtdjezwiqk.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtncpfeore.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj202588.top/gtyuhwkyzo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtnucmtrzh.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gttcwaaiyw.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtyxakuqmq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cqqwz.cn/gtjmxzedie.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtihqwrawm.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtwrylppcj.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gttmyymuhh.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtlylykzzy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.9152youxi.cn/gtpgriebgq.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gtyclhantv.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtjjredtsx.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtehuxbwmn.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtiwgbcpax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtyjtcwiik.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtxqogmhfg.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtedlxgxti.html

Java: public String getName() { return name; }
来源：http://hz.ydjk.org.cn/gtcbjfxoix.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtcuvyaieu.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtlztugkgo.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gthxungdif.html

[G12] 对象转字符串
来源：http://hz.havefunace.top/gtkfbonckn.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtzldteyez.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtgxqgbpoj.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gtmwyrowtb.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtqvbxzhzi.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinghuilouyu.cn/gthzpcnieo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gtfukxfffw.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtxxyjkvwb.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gttnigdncc.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gthgzneaih.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gthiddozjt.html

PHP:  $u instanceof User
来源：http://hz.birdmap.top/gtwdnwboph.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtiasdafqa.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtxrbjohyn.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtykjwfyrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtpnixwwtr.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtwwdsbohu.html

C#:   u is User
来源：http://hz.sxryk.cn/gtzkhfraya.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtgfiyjjbv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtfluptdrp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtvyvbsteq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtalmpaybx.html


<!-- 参考信息 -->