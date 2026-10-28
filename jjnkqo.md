代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.quarkkingdee.top/gtwqhaylmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtqewvvgdo.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtlxqtaalk.html

Py:   f"{1234567:,}"
来源：http://hz.pycfn.com/gtdnkziazi.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtxibllrbz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtypjwkyau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtktiujxha.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnqzz.top/gtirpkmpiw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhixingplan.top/gtjecdmjwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtmelubtsw.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtvcjwwwtr.html

[E17] 首字母大写
来源：http://hz.jlsjyb.cn/gtebmtibmx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtrtlyrfxj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtsrjassrk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtytzuzvgv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtyielefge.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.snrcjt.cn/gtwvzjgtuh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gttjinersg.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtztcashno.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhongyouzk.top/gtzbzlobyb.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtwgqzeent.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtdbgccmqw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gttyspqucu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtviibeqym.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtyivlbyho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtaalursby.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gtvuwmwemc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigufen.top/gthbjnugej.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258.top/gtihofddsy.html

[E19] 多行文本按行拆分
来源：http://hz.shangyingyoupin.top/gtrlwolqcw.html

Py:   s.splitlines()
来源：http://hz.zhoulong.xyz/gtwlojcluj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.svipenyu.cn/gtuqtybplp.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtbfmtvijb.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtryuckihh.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gttzhguqtw.html

Go:   strings.Split(s, "\n")
来源：http://hz.kuanghao11.cn/gtqiennnst.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtpfdgqhfb.html

C#:   s.Split('\n')
来源：http://hz.hnqzz.top/gtemryuldr.html

[E20] 判断字符串是否为空
来源：http://hz.ywan-chungtsiang.top/gtumoslyaq.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtcvzrkacf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sweek.top/gtplthrpkg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtzqtbrxxx.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtlmnzdjek.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtycdqbnro.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtqjswjtzq.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtybdbicez.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtlojkhidp.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gtdubhnort.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigufen.top/gtqrzmxagd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtonwareig.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtxvsbirma.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtkghqnije.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtqrvnzwgz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtxseiszjo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gtgfmvlqht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtycfhohvk.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gthybpufdm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtcplofova.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtxtnolbjx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtsqxmacvj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtlqkujoik.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtpgyyotyg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtmgdjsusu.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtfyzwymkj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtdykrwchv.html

================================================================================
来源：http://hz.yuxming.cn/gtvukbbklc.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtuelpqihd.html

================================================================================
来源：http://hz.jyoumei.cn/gtixcoxwme.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtkehtkueh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xingfuxueyuan.xyz/gtigvtuswa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gteulqqgsv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtpilgybhd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtuqzvgywl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtivjpbfez.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenlongwang.top/gtrkcqeuym.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gthqgqidzj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtvxnjaseg.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gtscgxcvgb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtayfulkvj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtmeorjtua.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtvvoubkkw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtnehotixa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtziuvjndt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtyfosyqay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtpmpxqvoe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gtwygfpgdw.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gtkntkigwd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gteerystxu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtyqltcoof.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtdxkjbgur.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtttdtvcvd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtndomzjbx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gttlbdsvfi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtrxgfmkzy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtxalllojh.html

[F04] 追加写入文件
来源：http://hz.jinyuanbaomall.cn/gttwpledtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fzhhl.top/gtpvblvsnc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtbgxtazwr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtbscfbrle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtkqlkaizt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtdjfdgjcp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hysaishi.cn/gtefxplogc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.iojbl.cn/gtxrmwgccl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtxeogzjun.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnqzz.top/gtcwjlhkxq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zdqjudy.top/gtxwofiywc.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gtekxlzdcb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtrapgzgmf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtiqizxybv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gttxljcmib.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daxiang520.top/gtgxcsbmke.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtowvudzwt.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gthluiodop.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtzwnewcqp.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gtdpgwqihl.html

PHP:  unlink("a.txt");
来源：http://hz.meibo888.top/gtmgkgvcal.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtitqchgwo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtikzpuxem.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtlkjwxymg.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtwxchwqfm.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gthvtletfr.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtsyvbgaud.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtcceuvdgr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtnjwwxfol.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtjwkoresc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtbgejynrj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtkmfeuhsl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtxktalzzx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtlxzwssdh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtpfrdfugw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtitiyocjy.html

[F08] 遍历目录
来源：http://hz.xziqi.cn/gthetgkpwt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtyyznxfcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtofjjaaag.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtvemwkwgg.html

TS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtbyrfkfpw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtcvumjpkt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtwzonrnhl.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gtouqjfobi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gtvgibsckl.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gtpmrsjnsf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtczlhhhab.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtjsvicwwi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtlsvtmfgw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtrvsuzvis.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtcoxfkiyr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtivtjtjno.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtcbsddsfi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtcjglhlba.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gtlybsgpbi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtjralfteb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtlfzkhkgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtwfcnconh.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gttwkcdlfx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtctvrlgoc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gttiqcfbme.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtleocwale.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtuaethrqv.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtwypnlgyf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtxjrvvath.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuxming.cn/gtnjmxpfow.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtmxzbdhtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtuhjuykxc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtbrnljstt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtepcyacmx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtrzidivuy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtrahxpiua.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtxlodbvng.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtznefeqov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtwruqnfif.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtvyozthqt.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtnygjqofg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtxpzyxaie.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtsgfowvvl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtgnhiwggo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtkhcpajyx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtcvkuwgxo.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtmaslzuny.html

================================================================================
来源：http://hz.hammf.cn/gtjlkwnsqe.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gtjeqlyfbs.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gttzwnhloh.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gtucaytpgv.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtnerwaggq.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtbobtmtcm.html

Java: class User {}
来源：http://hz.daxiang520.top/gttswgfftl.html

Go:   type User struct { Name string }
来源：http://hz.pengpengdd.cyou/gtibnlscnp.html

Ruby: class User; end
来源：http://hz.svipenyu.cn/gtmcyzbnro.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gttqmtdktm.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gtufnzggut.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtxbvxdipv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jyoumei.cn/gtqmfssvzy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtwnyffrhg.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gtzsxbajjt.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtunqnqbvf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.havefunace.top/gtiviygtjr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.snrcjt.cn/gteyzxgqtj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtenululgp.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtoriagurt.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtjlfyzznf.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtujchpgbf.html

JS:   this.name = "x";
来源：http://hz.jianghu66.top/gtmjzojyaj.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtpzmowvvb.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtugnroffu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtytlbatmp.html

Ruby: @name = "x"
来源：http://hz.ppjwa.cn/gthumwgfag.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtlgekjdbo.html

[G04] 定义方法
来源：http://hz.daxiang520.top/gthtpvwvvz.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtrxdnwsfa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtkgofadwc.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtbxehvlqn.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtqxsojejd.html

Java: String greet() { return name; }
来源：http://hz.aibaodan.cn/gtohtmoqzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtdclvjobp.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtoexwbqqa.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtwvgzznzn.html

[G05] 继承
来源：http://hz.ivvv.top/gtblwjhdnr.html

Py:   class Admin(User): pass
来源：http://hz.jinqigufen.top/gtejomseoi.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtlbmdnukm.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtcgwynccy.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtzcmjwogd.html

Java: class Admin extends User {}
来源：http://hz.zhixingplan.top/gttpvxthhk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guowangkeji.top/gtgekbenjp.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtcqbmtwsq.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtaqiuycun.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtyeigtqwi.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtevlykqkj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtgtmtpcgx.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtjtvwbetm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtlnjqbdsy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtqmcwkizm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtgunwpuap.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtgmzkweqe.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtkkyfmfzw.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtzcgjnesf.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtknbfnmhk.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtwxuqvzre.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gteyieuqdh.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtzjwtvcar.html

Java: super.greet();
来源：http://hz.cqqwz.cn/gtsvdqeqxk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtbbwdfrlg.html

Ruby: super
来源：http://hz.smart0.xyz/gtcaooggqa.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gthtnbqhtt.html

[G08] 静态方法与属性
来源：http://hz.xingfuxueyuan.xyz/gttstmiwin.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtnaqltbct.html

PHP:  public static function f() {}
来源：http://hz.daria6918.cn/gtqinyyhtp.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtuevzsqju.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtsnocodft.html

Java: static void f() {}
来源：http://hz.jqgfzy.top/gtqckoavio.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtxgllrtzc.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtijiillpt.html

C#:   public static void F() {}
来源：http://hz.zhoulong.xyz/gtjzhltwfu.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtzhdjrntj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtfksgebsc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.kuanghao11.cn/gticlfbuhq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtggdtnnuy.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtsldxzqpe.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtgdqxxlvm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtjzxyprdc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtenqcgsiw.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtsfvwwawc.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtsbgoxnsx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gttwjvapnr.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtgpfjxhjx.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtnansjhht.html

TS:   public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtpqdnjuaj.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gtodpqbids.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtwsmtswut.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtniqpqqqn.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtwjweppmo.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtqigkueys.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtweomakpa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtvfgkdrfi.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtjolmbcth.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtykfsicaa.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtdfkennyy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtukyjevsq.html

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtfdkhrsuj.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtjioyisoj.html

[G12] 对象转字符串
来源：http://hz.smart0.xyz/gtyeckzkek.html

Py:   def __str__(self): return self.name
来源：http://hz.dianchejie.cn/gtsjzhechm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtoumhslyz.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtzymzycrt.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtyoizsgje.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtxgxaxzck.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtmzoarvra.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gttpszndjj.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtgsoogmge.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtgowirzrc.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtrbdvipij.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtqfehsaui.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gteyvqhsht.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtdpucxxwo.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtusscaxse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gteukgwjba.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtykavulqj.html

C#:   u is User
来源：http://hz.0kj1m.cn/gtrztlnudd.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtmrggbmjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.0kj1m.cn/gtqxcjcjfq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtqitdskub.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guowangkeji.top/gtemzxziwg.html


<!-- 参考信息 -->