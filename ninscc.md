代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yangfankeji.com/gtayshiplf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj202588.top/gtgrccoymy.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtypmycicr.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gthfxxkhmz.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtkahslgeb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtqunqpghc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtzfmwnalo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtkwbwezur.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtzvvguybg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtyheallce.html

C#:   1234567.ToString("N0")
来源：http://hz.svipenyu.cn/gtmowihmmg.html

[E17] 首字母大写
来源：http://hz.gaohongyu789.top/gtehlgzgzv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tianlin.xyz/gtvbzanqnm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yueranfly.top/gtyopkeymk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gthlczvdjm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtwfovdlul.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtdrvmatnk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.316326.xyz/gtyuipkicp.html

Ruby: s.capitalize
来源：http://hz.ydjk.org.cn/gtpswohadn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtdjmcurdt.html

[E18] 模板占位符替换
来源：http://hz.aizwys.cn/gtwerpsbcw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtagmgogfp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gthqjofkgx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtyukfgojx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gttcfypnka.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xylfe.cn/gtxyeianen.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtyezdyytq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtatbvbvlb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj202588.top/gtraywgroi.html

[E19] 多行文本按行拆分
来源：http://hz.cucudq.cn/gtuatpuqkl.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtrfmhfllv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gttrnjnbsk.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtgpwgtzma.html

TS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtjcseehbi.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtulmintqe.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtpniccsto.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtjajglrfp.html

C#:   s.Split('\n')
来源：http://hz.yongpay.top/gtusgswqfu.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtodfabvvw.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtdkxxgfva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gtwuywbawx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtrgreagpy.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gtrdbfirdn.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtuypfosux.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtronkxaom.html

Ruby: if s.empty?
来源：http://hz.sysykeji.top/gtmnupwimk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtqpriscmn.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtcuxqyshk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fzhhl.top/gtwsejhmzz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtjrjvjqto.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtvfsfsdud.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtvcbgijcq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtsrjhvqay.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtwdentuds.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhijiandao.cn/gtuufvodyx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gtnrnxflol.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtkmxucfxy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtqaxbkmkx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtqfgtbhmy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtdlvkbynw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtadwoletn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guowangkeji.top/gtruicmppg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daxiang520.top/gtbnbmbzod.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gttehtyuax.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtsubjclpw.html

================================================================================
来源：http://hz.vqdsnc.cn/gteebrjiey.html

F. 文件与目录
来源：http://hz.sxryk.cn/gtjkjngdpd.html

================================================================================
来源：http://hz.shzxlz.cn/gtagbmaxjq.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtdeaafrlo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnxiangtu.top/gtdgjeregt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtzufyiwoe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ywan-chungtsiang.top/gtdnhwnhmg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zycfv.cn/gtrcakvtow.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtzphnvxcg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtuuvvkrkv.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtsjatlimt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtslgqlwov.html

[F02] 逐行读取文件
来源：http://hz.yvedp.cn/gtbeqszxmw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jyoumei.cn/gtiuyjuqnb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtjqzphshv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtvljsoflb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtijhddecy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtemocitqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydzc1.top/gtednzubgw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuetiantiany.cn/gtkxpxiptb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ivvv.top/gtklsqyvtz.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtdvlnknhn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtirzyytzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtojcjikcc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gttpcqhhre.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gthjsikadz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtpmhanqti.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtglcnmlou.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtftkucmve.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gtrxbkzvmu.html

[F04] 追加写入文件
来源：http://hz.jinyuanbaomall.cn/gtzhrlugvf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtayjclxmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtzkfqeonk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtzioraizj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtxdjjcxmd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtsopdhqsv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtpgmtqnjg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtwqtvrklt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtngjyapaa.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gteemqmklv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gtjcwzkvot.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtjldxykof.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtmyabnmsq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtrhopmmby.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtrvjbdyrc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtzbckcoqv.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmmvqoovk.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtmpvxksmz.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtfugkmrhp.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtaosqhoey.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gtqxmheksy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtkjifqaba.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtrudsydxi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtameqjfih.html

Go:   os.Remove("a.txt")
来源：http://hz.0kj1m.cn/gtfnhdimpy.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gtumvycxjq.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtzctmnhmr.html

[F07] 创建目录（含多级）
来源：http://hz.gzhubu.top/gtrxzjiyod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtfywkdvir.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gzhubu.top/gtupugnzml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtrzkconsg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtszcsvawu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtlultmnse.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtczpsprjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gtnuwpdjpj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258.top/gtzgqbabrv.html

[F08] 遍历目录
来源：http://hz.nwbrower.top/gtpvfwljom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pycfn.com/gtbwqsogvd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dianchejie.cn/gttshcnoln.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtyqdsgwbj.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtbjiqsumc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtslsxohod.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtffwfhqvg.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtlztktiyj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtzoeqfmfm.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtshhpddqs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pengpengdd.cyou/gtihvexdnt.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtdjbiywyw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtxuylkcdj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gttjmdqmig.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtgkcdazfa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtmmtiodqz.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtjyjgczes.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenzaomai.com/gthrdrqhmy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtuxlldinp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gttwpqznye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtiypwywtj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtswnsntik.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtqdwnjoaq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gtddxbrzuy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtsnniabpd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtfymxyioy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtfkzyelvp.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtsikdovqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtqfqyxofl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtwivsnykc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gttwbcxeeu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtfoeyyyyt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxuanxn.top/gtqpgqbsoq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtxxexczgq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtghauacjw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtyddxxvjh.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtcgybykzg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtqtaabwtb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtdtfkqcuh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuanzhike.top/gtwrqqakna.html

TS:   // 同上
来源：http://hz.yj20258.top/gtiznpbkgh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtvftuador.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtehiplqda.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtvhkwciob.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sysykeji.top/gthakkjqjr.html

================================================================================
来源：http://hz.iojbl.cn/gtmodmazkw.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtcxnxddku.html

================================================================================
来源：http://hz.fengsongda.top/gtzamzoztg.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtjmbkrnjm.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtdnbaumqp.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gtqzoshgbp.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtwavrurvj.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtyqqrcsxr.html

Java: class User {}
来源：http://hz.tanke756.top/gtpzywrbwy.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtnlenqoii.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtwaclffhp.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtzjntymme.html

[G02] 构造函数
来源：http://hz.cheryme.top/gtbbjamqsc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtqpyqkyps.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtuyfcpwxf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtfkyfksty.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtuuimxohg.html

Java: User(String name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtsbvktfgk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtgafrzdrv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuetiantiany.cn/gtbfczkzto.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtuzthqhhy.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtgyqmjqwh.html

Py:   self.name = "x"
来源：http://hz.xinyue.icu/gtqlpyewba.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtpsycoazj.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtpltcbjpf.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtlsstyzai.html

Java: private String name;
来源：http://hz.zhengqikj.top/gtjeqychtx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtvtadcsnw.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtdybrnuoj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gogol.net.cn/gtpxndelax.html

[G04] 定义方法
来源：http://hz.ydjk.org.cn/gtdgypotnb.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gtytdwvrfe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtsvedsoyh.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtcoqldlrq.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtbixkpbwr.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtbvpuivya.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtynivtuza.html

Ruby: def greet; @name; end
来源：http://hz.ydjk.org.cn/gtydubeayy.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtzlwpvjjf.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtbrduvkaj.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtofkazwur.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtlbqibuxb.html

JS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtzjiylalg.html

TS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtpovygxlo.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtwssozkxf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.feifeiyinyue.top/gtwulztsot.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtlgxzzdil.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtvfrjywif.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtjdyomfvu.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtxyrplwwl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtwgxutmqj.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtjilivzbg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtbnexcrvy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtlzulangk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gtnuhpmddp.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtzfeneilz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yanxiufei.cn/gtqlemjsfb.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtdnfxbnii.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtyednstzk.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtkhifehvb.html

JS:   super.greet();
来源：http://hz.sweek.top/gtqpcnvelr.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtvmqqjidv.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtouxzlmbr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.haohaochexian.top/gtcqgxvlam.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtoueaasso.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtxqcedpex.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtafkjvvvb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.svipenyu.cn/gtdcxiqiwo.html

PHP:  public static function f() {}
来源：http://hz.jianghu66.top/gtgqtdautk.html

JS:   static f() {}
来源：http://hz.52xcode.cn/gtbzryopuh.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gterveofwi.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtfgqjkvjx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zycfv.cn/gtqrulpodi.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtxmmhdcxj.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtqigiyzid.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtncnjxseq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhongyouzk.top/gtmsitlsew.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtnkhlhtrv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtghnbewtl.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtgvjvsbgt.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtglmgbhmx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtlqeydoeu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtpsznhniy.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtvxhnwaqm.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtxmccxtkr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtbiahicwg.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtguctvthj.html

JS:   #private 字段；其余公开
来源：http://hz.hfpthk.cn/gtougdpqtp.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtenkxtruv.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtjvtbruas.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtgnhjotyo.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtcxoftplq.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtnhfscbrf.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtibulnsko.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtpchxbfrd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtekuerrew.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtoazyypmr.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gteputfipp.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtwrlyfaxj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtrssjuxzr.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtkajrxghh.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gttriptytb.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtkcoaxfmi.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtibrwktmm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtjznidndw.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtnnpxubmn.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtxiiiwqpz.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtgpgmxboa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtabdfsogu.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtaftlpqez.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gtnsxxiqpj.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gtmjjhjuzb.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtcuhqcval.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtgnrzjadh.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtomzjjevh.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtymsmghsi.html

Java: u instanceof User
来源：http://hz.cqqwz.cn/gtpprjlmpp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtqeqrevgo.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtwxqbesvr.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtnqegdcui.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtispyhvbw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gteuktddht.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj202588.top/gtyxqriedq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtueuplivi.html


<!-- 参考信息 -->