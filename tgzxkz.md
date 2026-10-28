代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnqzz.top/gtjeqlejgo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shzxlz.cn/gtqecdnbto.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gtjhjyjkwk.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtmoaacehj.html

PHP:  number_format(1234567);
来源：http://hz.yuxming.cn/gtuqmqitph.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gticaxadkn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtknnfvsee.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yvedp.cn/gthotljvrw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtlgkqutqq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtbueexnsa.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gthpxnubhk.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gterahahaa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtynjoljbi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtspnthaht.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtjizpxwmq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtdscyqmod.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xingfuxueyuan.xyz/gtldyhucun.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gttrtxyndb.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtipzxkwxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtzvcsdhpv.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtrbqlucbm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tanke756.top/gtrzqkozlx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtykqyqteh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtqzyvdnfm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtysjdnfup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tian-w.cn/gttwafsduc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gtwkbsoydo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtzcavptzt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtjbmyjxbq.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtieohlata.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gthelgvejg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtyjwbvykw.html

JS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtxhvrqjpy.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtpkyhvlcz.html

Java: s.lines().toList()
来源：http://hz.xuanzx.com/gtpplwavqa.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtuxqjxjcb.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtoifgiomu.html

C#:   s.Split('\n')
来源：http://hz.sxryk.cn/gtsuclkitc.html

[E20] 判断字符串是否为空
来源：http://hz.smart0.xyz/gthknnruxf.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtzcntldoj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtssygpcqu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtwmbrcmuy.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtmevkihoy.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtbqtfrvbx.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtpqqddrnq.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtcjpxhcad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtllkvowaw.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtpqbgmkzw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuanzhike.top/gtxujcvgtf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtulryheba.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtpxugkzzu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtekxdfnem.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtlypvfrxt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtxykmoyfe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yangfankeji.com/gtzsbqdjnw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtksttykwl.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtywfaetzk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigfzy.top/gtbzfmqshv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtlfbrxmuf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtcodhwgma.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gtnnbkejyt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtnsscepsc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.vqdsnc.cn/gtfoniifqg.html

Ruby: s.bytesize;  s.length
来源：http://hz.yongpay.top/gtkgeepzdu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtexumklwr.html

================================================================================
来源：http://hz.yongpay.top/gtqbcsdfyu.html

F. 文件与目录
来源：http://hz.316326.xyz/gtqopstsnh.html

================================================================================
来源：http://hz.cucudq.cn/gtzhhyvqov.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtlposolxs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtjegetebj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.kuanghao11.cn/gtubexwdqh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gtyfpsrmxd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtyiyxjxtf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtsnnvbzwl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258888.top/gtylglnssv.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtrhwnionm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gthyhhopzs.html

[F02] 逐行读取文件
来源：http://hz.shuidangran.top/gtwvzfjyus.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gteypedknh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtazpidrcy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtkhcjdvvl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gtuvtwvpms.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtmkznbscz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtttakbchr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cheryme.top/gtmpjgonjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guannengcc.top/gtlesruyln.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtnncnxgxg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gttjfdrwyd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtaluipaqi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtmbzyibpc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtdmsanzsf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtsjtovdgm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtxubcdcfh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtnyujnvro.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtdmhtbuea.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtprrihqcb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtqjobnaxw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtznelccrl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtijuzbeoi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtcpofayuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtjtdcbxaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtwkmnkihc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtqovoaxnr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtdfzevpxi.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtskawffui.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtqknrnlio.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gttlivtryd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtjtzysfvl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtcfieijcg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtrxhkwlzh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cdnleiting.top/gtqwpyxeig.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtefprzdmu.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtogpklmab.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtqcmcuywb.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtdphogszt.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gttwujngtl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtzquokeyx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtesheelxj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtczjvtruz.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtjohulgbp.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtucnndeid.html

C#:   File.Delete("a.txt");
来源：http://hz.xinyue.icu/gtgmanysmd.html

[F07] 创建目录（含多级）
来源：http://hz.daxiang520.top/gtguqvywgn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtqtefejhm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgfzy.top/gthirkujhf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtnmzzlcsx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtirqxevvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtriwevaxz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.316326.xyz/gtocicsxyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xingfuxueyuan.xyz/gtnccwegxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zdqjudy.top/gtnvpefdhm.html

[F08] 遍历目录
来源：http://hz.pengpengdd.cyou/gttxaegzel.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtrmlslgum.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtvkevhanj.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtopjxvzyk.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtpwhaiidb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtwcfaavlc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtlcdcfiwo.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtnyuyftig.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtzshgfrrt.html

[F09] 获取文件大小
来源：http://hz.guannengcc.top/gtuxludiby.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtdmzfprxb.html

PHP:  filesize("a.txt");
来源：http://hz.wangshuangyany.cn/gthjkiyakd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtntcorzth.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtnzmqrfho.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtxeczmtdv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtrhdgfgre.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtgkshnudg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtgplzwqoq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.havefunace.top/gtbzwdusdf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtcxdkbijv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gtyenpexxy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtjtgslcqh.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gthypqchjq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtkaasiyzj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtuebrmwss.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtntwoyajm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtkdpckbbf.html

[F11] 复制与移动文件
来源：http://hz.jinqigfzy.top/gtygxmjcmm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtzjqewhdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xylfe.cn/gtxphenbnl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtfwlvdnof.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtnhrzbwyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258888.top/gtrqejfjru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtfvysfftw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtxtpmlnhm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtuejogrwo.html

[F12] CSV 读写
来源：http://hz.jinyuanbaomall.cn/gtgmulzpaj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtkzhdwcpp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtfzjpgwlh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtbsipnzny.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtnnbjrabn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gtmkhnizpp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ppjwa.cn/gtewtggqsf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gtbtppyrbk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtwgxudaok.html

================================================================================
来源：http://hz.gotoacloud.top/gttwjoarad.html

G. 面向对象
来源：http://hz.snrcjt.cn/gtllemaepa.html

================================================================================
来源：http://hz.xziqi.cn/gtqrcdhvqf.html

[G01] 定义类
来源：http://hz.xinyue.icu/gtypimlmkx.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtmntwwnlb.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtacnesomg.html

JS:   class User {}
来源：http://hz.yongpay.top/gtdwwjnvqb.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gthlvulgyg.html

Java: class User {}
来源：http://hz.cheryme.top/gtbcbdmmfq.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtcikxknes.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtpckjduvu.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtjyjbekqu.html

[G02] 构造函数
来源：http://hz.sysykeji.top/gtvvmyrqrw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtflpnvugw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gtbtpeioyl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtiptlqxql.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtxwyirgwg.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtjffsrxju.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtqrptzfdi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtzsuvbnbk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydjk.org.cn/gtzjrghvxx.html

[G03] 实例属性
来源：http://hz.yuxming.cn/gtqaqvvfpx.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtfzjjdgtb.html

PHP:  public string $name = "x";
来源：http://hz.yangfankeji.com/gtqacgmqep.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtttqoyisw.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtvnmumjhx.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtnpccyson.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtsvozqbfc.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gttucbovon.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gteujumbcq.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtlaiifwwp.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtbmsuexem.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtdnovoxvv.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtyanqjvqi.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtzcqvmset.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtfsnjbnkl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gttdjxpkbu.html

Ruby: def greet; @name; end
来源：http://hz.xuetiantiany.cn/gtochzwvhk.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtqhlikgea.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gtxahsxlsq.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtkbwmkvid.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtspotohwe.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtkvzlwzeo.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtbrqtlqlf.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gtobcvcspp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtnovlvpeh.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gttwwxrzxr.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtfdihjodp.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtxikujtkg.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtudpjukng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtjscagrhq.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtjgfpuxwy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtoojtmkhc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtdrmxxaye.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtvrrxsydh.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtoxhnfosv.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtjvwqhcfw.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtqijklgab.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gteeedyigs.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gttqjslnzr.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtvxvlnorr.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtfwojhdzu.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gtldhldwrf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtusmlhqlz.html

Ruby: super
来源：http://hz.hywenlv.cn/gtdresdcto.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtccgjnbwz.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtsroqwlps.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhoulong.xyz/gthjztaehf.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtiqrpofej.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtzcuzljfs.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtouynnuwr.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gtjmrjsemf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtlkplinxb.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtnzuhkten.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtzhlzqorn.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtvvwywvvc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tian-w.cn/gtobvqjlqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtynhdhljx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtjpnqwwgl.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gttorppbll.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtesmulplj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gthtktrwoa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtzeqcnlbn.html

C#:   interface IShape { double Area(); }
来源：http://hz.sxryk.cn/gtpqnxmsju.html

[G10] 访问控制
来源：http://hz.hnqzz.top/gtkpqpqjrx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtifrvqbxp.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtvixmlezd.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtnffuizlw.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gttulhkibs.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtefwuwtjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtydazxxyj.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtugueitqm.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtxqgrbvyb.html

[G11] getter / setter
来源：http://hz.fzhhl.top/gtyhcrttmf.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtjyysfubr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtatpliyky.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtnmdcfews.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtkvpufkyn.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtpggxgmlf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtcjjhxqpv.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtubxmalqu.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gtnchequws.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtkcxojvqi.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258888.top/gtrsivnaew.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gteefwhzvn.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtekqrwndz.html

TS:   toString(): string { return this.name; }
来源：http://hz.gzhubu.top/gtayhlrgpp.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtbamzfdxo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtyztiagal.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtpdbqpnbs.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgfzy.top/gtxjfsawii.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtmsvrepji.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtxavdpnea.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtejfaynxr.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtvgghpdoi.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtphcdqjvw.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtkbzzkwui.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gttnpxglbc.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtppetbhfs.html

C#:   u is User
来源：http://hz.tianlin.xyz/gtqtzfdpep.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtgxwmroyu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtcwpqcqaw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtndyylzpg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtptpbnalh.html


<!-- 参考信息 -->