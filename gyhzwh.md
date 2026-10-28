代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtveatugeh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtkdnbszki.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtzkxgftko.html

Py:   f"{1234567:,}"
来源：http://hz.xziqi.cn/gtodtpygfy.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtcqsbjkmy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtmkuxager.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtsdvvqaau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtbuqxdjwi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.birdmap.top/gtuwhgsrij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtdwjikgkh.html

C#:   1234567.ToString("N0")
来源：http://hz.zhixingplan.top/gtuepkoyan.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtympjibnc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtwnseihxo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtxqonccvv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtzztxhvgx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtuetfkfeb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtbreiekez.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtkjqqflrw.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtniiguiqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gteimhhozv.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtowmnviry.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangtech.top/gtvikxhsia.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtwguemcjf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtrbbmdpzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtzdzveafc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtqiqkwvvp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gtwvypbptx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gtehltmjvt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtjumobgsu.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtxnhqswta.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtswradsms.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gthzhrcgov.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtolrmcwoh.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtpcmpxusm.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gtfshwxbsq.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenzaomai.com/gtgijvpfvh.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gthrhjzgxn.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtoemuzsqz.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigufen.top/gtoeiomknx.html

Py:   if not s:
来源：http://hz.birdmap.top/gtbeghttft.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtszvplzky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dianchejie.cn/gtrbkpumkn.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gthckkyuib.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtbwxggzir.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtiaedowvl.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtrvdepkgj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hysaishi.cn/gtonuefndt.html

[E21] 超长截断加省略号
来源：http://hz.gogol.net.cn/gtphkqvpea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.kuanghao11.cn/gtbmzfmggv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtrchesfhk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtbtlulyxp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtxiowctgt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtlwbedqeg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yangfankeji.com/gtlkpkbgmr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtqxlvpkcl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cdnleiting.top/gtymrgijzn.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtccscwjzp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtfuhcnbkk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtlbjunmub.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtfyvhaufj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtghpojcbv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtcwmkjjfr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sweek.top/gtcqpvvwwt.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtekhfdnxq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gtxzxnxycd.html

================================================================================
来源：http://hz.sysykeji.top/gtdxfotlkt.html

F. 文件与目录
来源：http://hz.daxiang520.top/gtavblwklw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvxkmixlu.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtsxjtunlv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtoyejwcdm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtpghavghx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtfxvgsgie.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangdashe.top/gtlntrbyrf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtbydvdtsu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtrpcrkboa.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtnepmvsjk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtiztrugoc.html

[F02] 逐行读取文件
来源：http://hz.0kj1m.cn/gtqcvriawi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhixingplan.top/gtuokepbmz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtgcxtuezx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtaroqnxsa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtzmbcvmoh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtmcbyjzhh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258888.top/gttfxdlggs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dashuyun.cn/gtxhjnnpeu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuxming.cn/gtqeekqawp.html

[F03] 写入文件（覆盖）
来源：http://hz.tanke756.top/gtsysoheha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtgjezpqou.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtdaeoplxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtzjcmqhzo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtvrnrzpae.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xziqi.cn/gtjiisdjnb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtfogxkhbr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtcfcwxcmp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtdietlpah.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gtjsxlleeq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtkxnoejbo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.9152youxi.cn/gtpocpxvqd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtacuvzska.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtzkmohbnt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gthilnmids.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtrshbhhtf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtiesafqlk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ybcxt.top/gtiytqsnnb.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtzvomlrva.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtufniuaml.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtayfmooch.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtbqrxlqxg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gthlfzpfhg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtcvqdrdyb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtqeqqjuml.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtkoqzcmgm.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtgsqbaqjx.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtwmjpogdk.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtkhyefbea.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gthypkjkqq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtoyroiezq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtsxgobqbp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtbqthzves.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtxthdnitp.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gttnlrlctv.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtjnxyytaa.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtknuihdqt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtduiswxxm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtbjnstwiy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gthlhqmnbg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtekuldmql.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtjcnmzcbe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtmnzsngdy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtnsgriadf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtlphjolhf.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtmuuaohdl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtewvwncng.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtualrmliq.html

JS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtinvceiri.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gtqgvkxfgp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtosypzpil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtjybmtfwo.html

Ruby: Dir.children("dir")
来源：http://hz.zhaomingkeji.xyz/gtikpeiziz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gteppsjofk.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gtbmpbaogr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtxzswbcwh.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gtlezuzevi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtftnculus.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtjxwppjov.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtpmcglbxc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gtrsjcouux.html

Ruby: File.size("a.txt")
来源：http://hz.ydjk.org.cn/gtrxmdcynk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtbiejvnbe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtuhytpubx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtushlqhgi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtevzmqhst.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtljehhjsx.html

TS:   path.extname("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdwhlgiml.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zdqjudy.top/gtbsdtsbaq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtsazyqoay.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtxsuaxrmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtzcscvvxl.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtsplxdiai.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtkludifyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtmrrewhal.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtmdpokpeg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtinoijzch.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtnqnblyza.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtagxzqusv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtsdgbfsks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtfojfihnz.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtuzmjgxot.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtdmpkdbyp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtxslfolcp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtggpnokav.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtihfhopzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangkeji.top/gtjfpyjopz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gtgvlxjydu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtljhbcgzi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtqhmhqrpo.html

================================================================================
来源：http://hz.jinqigufen.top/gtrijrnljw.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtbnvtjlyg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwdnbvomq.html

[G01] 定义类
来源：http://hz.cheryme.top/gtnqjkfufa.html

Py:   class User: pass
来源：http://hz.tian-w.cn/gtulhuohxo.html

PHP:  class User {}
来源：http://hz.52xcode.cn/gtutmyxzix.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtyckbeygu.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtmeqlxajw.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtfkyefuko.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtkbeajtnn.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gteylbkdif.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gttnvrbrpp.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtrfhzyvex.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtbullohiz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gteskckqdj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtezrerbii.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtjqiteykf.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtmiurcxxz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtcxxomcin.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtwgwslrno.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtfzpebbrk.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtqzjcfdqw.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtjkihricz.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtgfwnugvj.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtqzfzvgas.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtiyrkuzbb.html

Java: private String name;
来源：http://hz.jianghu66.top/gtutcczpep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtssbkvzkg.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtzffhnrkm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shuidangran.top/gtjiopsgss.html

[G04] 定义方法
来源：http://hz.yueranfly.top/gtvilzpjew.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtsfhixcdm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtfmdhlyfd.html

JS:   greet() { return this.name; }
来源：http://hz.jyoumei.cn/gtamlopuaj.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtfakccgca.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtohnrjjxy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtdnvsoakk.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtowdyqdff.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtuktqrbew.html

[G05] 继承
来源：http://hz.xylfe.cn/gtcnzcsnxm.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtiyasbuhx.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtmehcdnal.html

JS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtumtrxhwm.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtlkzgdpdy.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtkeajgjay.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gthpebxfnp.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtggunarxc.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gttnunmkra.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtfzooqtxm.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtxltwnutm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtpbofudka.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtngnhsxse.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtgyaaeaeo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtyzbhhctq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gtblifkzma.html

Ruby: def greet; "admin"; end
来源：http://hz.guannengcc.top/gttfiuhnxk.html

C#:   public override string Greet() => "admin";
来源：http://hz.snrcjt.cn/gtyraaejfy.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gturdahnjx.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gtgqrgfnsj.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtcmwynsdb.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtzbkojjgr.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtahcvjwer.html

Java: super.greet();
来源：http://hz.52xcode.cn/gtevgzpwnc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtjfhkoude.html

Ruby: super
来源：http://hz.yuanzhike.top/gtmpyarybi.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gtwectpavm.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtjqmduppv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtlwgriume.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtnqokozfd.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gthcqsvqcv.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtijfpdngl.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gteztbszcg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtejiyfkyx.html

Ruby: def self.f; end
来源：http://hz.quarkkingdee.top/gthfdlncyp.html

C#:   public static void F() {}
来源：http://hz.gotoacloud.top/gtrhpuyayl.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtcusqwdgm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtqoahbevj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtamwmyhnz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtlwoxogvv.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtekaxdxvs.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gttafwrpsi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtknxnwdew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtjnycjhbl.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtapixkuks.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtmhhubnjh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtxxvyqdwv.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gttrzzfcmb.html

JS:   #private 字段；其余公开
来源：http://hz.smart0.xyz/gtopevyfnt.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtladftsfk.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtkaeapzdw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258888.top/gtblysyydd.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtgznhqvah.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtlbuofqpa.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtsxlrvnas.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtioxgbsyq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtoosutemz.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtfesboojr.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtippmbjcd.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtrbbejggy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtbofpyjwc.html

Ruby: attr_accessor :name
来源：http://hz.52xcode.cn/gtqlnvsihz.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtqapkompm.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtuhwbmbga.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtpdxmoxjr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtrnvzkldh.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtupcgzvdb.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtrfiehcxz.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtuutqhtzq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtzqhvmhnu.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gtjprrqbgl.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtpwbdfmzh.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtakwrwsdb.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtdsiwcxkk.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtlmaebonb.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtsptzwxke.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtsgnwbrgf.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtqhrjcpwr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtvzqzrihg.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtnhisnnoi.html

C#:   u is User
来源：http://hz.guannengcc.top/gtuyhnfgsv.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtfiifpjno.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gthxojdrav.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtpnvjuvmj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gttldbtlxh.html


<!-- 参考信息 -->