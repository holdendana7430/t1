代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtyhrnpjan.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtvlhndhns.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtxnitfhaw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtfglvxrvn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtirejhcer.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cheryme.top/gtjsjmkaag.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtifjszfwd.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtnacuocob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jiagoushi.top/gtdnrmxsck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guannengcc.top/gtkpwwjelk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtilwkxvzx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtywmvdwuk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gtvwqijfdr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtdautwczs.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtosqdvtdd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtczuqgjst.html

[E18] 模板占位符替换
来源：http://hz.xuanzx.com/gttcywimzf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtqnklkzmp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtxirrddpv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtckcjqdsf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtzehtlead.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigfzy.top/gtqahdfzke.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.andypj.xyz/gtllrqcfgh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gaohongyu789.top/gtyhjjthhh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nwbrower.top/gtrtikcaia.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtfootqyyw.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtwddtcnsv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtiymojvvw.html

JS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtrlcbxqpl.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtboytwful.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtxivymvqd.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gteonlkfah.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtnigvevpv.html

C#:   s.Split('\n')
来源：http://hz.feifeiyinyue.top/gteogartaf.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258.top/gtvvxpfyvb.html

Py:   if not s:
来源：http://hz.meibo888.top/gtmugwfpyt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gttvpwimuh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gtuvomeyry.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gtnsdyxxna.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuanzx.com/gtmlohnouw.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gteoiwuagz.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtfnjeiwzd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.52xcode.cn/gtvneiavbr.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gtviexnern.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtlmdvprur.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gogol.net.cn/gtmgcjnhpd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtossnwvwc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtulavpsox.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtduanzioq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtyolhmsxr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtigpgjcxf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtkgaekdrk.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gtuljwuvvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtrnamlqwb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtcqqsiudl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtkrwaqwhy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtsovwegfd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gttzvndpyf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtxsmvhmny.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtxujphawe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gttsmmhsmf.html

================================================================================
来源：http://hz.yuanzhike.top/gtfypoeyob.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtidelahhi.html

================================================================================
来源：http://hz.yj20258888.top/gtlzcamjlr.html

[F01] 读取整个文件
来源：http://hz.pengpengdd.cyou/gtwjcnpvpe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtsmnccdzz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtoiwltuqu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtnjylrhir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gtvzzyuvgd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtbnldszed.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtsqepqyhr.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gtmmkysfws.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtyjmomrux.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtzlfiwgmc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gtrfpfehpo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hysaishi.cn/gthafeoytx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtsqsmwddj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtjkiovjet.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtjlwsnvdx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gtzzdefnel.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtspitxiyv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yanxiufei.cn/gtemqwmtzj.html

[F03] 写入文件（覆盖）
来源：http://hz.yanxiufei.cn/gtqapnyfct.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtztsyspyt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sxryk.cn/gtdhohwrmj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gttfirbgvm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtywbehmvd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gthorhkmsj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxinkj.top/gtscqeieox.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtqvqhrpfo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtihxmpsim.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtfpskdrik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shuidangran.top/gtunhkrppi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtphdqgxtq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtjqfidold.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtkaxpwdgm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtajkddlvd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtaflwhngp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtkxiegawt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenzaomai.com/gtwxtbkxqu.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtdlzwxihn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dashuyun.cn/gtuvvgwhdh.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtowxoerdz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtpdsvdmui.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtehuikxne.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtitftbelv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gzhubu.top/gtopvmxaex.html

Ruby: File.exist?("a.txt")
来源：http://hz.pycfn.com/gtpanihxzz.html

C#:   File.Exists("a.txt")
来源：http://hz.cashguo.top/gtscbybafu.html

[F06] 删除文件
来源：http://hz.cdnleiting.top/gtgrsdjdpp.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtxhxsogpb.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtgblmnjlx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtxbkqycit.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtudwbmgap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtgaxyoexa.html

Go:   os.Remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtduysddns.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtudkngshc.html

C#:   File.Delete("a.txt");
来源：http://hz.zycfv.cn/gtggxhohxv.html

[F07] 创建目录（含多级）
来源：http://hz.c1oappe.top/gtmehmxxqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shzxlz.cn/gtxnnnyslr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhixingplan.top/gtknjtjvej.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtnbrjyrkv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtbmdqeanu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtsdadwpll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtfdskknqd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtevcaigvc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtrhxoarrl.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtlqpfzmqf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtcxzwcpav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtsbogbvyk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtvhamxgfp.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtfpqizrtn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtkdsnzvym.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guowangkeji.top/gtbwiddydk.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtrcyaocmz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtfyezisbi.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtumpvcift.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtiaeesldj.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtwjvneyjf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtaxlpqwta.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtwcsepwfm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtseiwyzei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtplelzvqr.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gthyoaoocd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtarrwkbgh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtykgqarwx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtmeeunleo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtyvinhcho.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtmcziibpv.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtadarejwg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtyybgnqch.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtkqugjqgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtvviqsesn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gtheaczswu.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtfixcmunn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtdrinbbmt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtengmrskb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtgawshfmj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtialrojxy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtlrhunsvj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhixingplan.top/gteqohvkex.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtuulzfogg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtwzlqwfbg.html

[F12] CSV 读写
来源：http://hz.cashguo.top/gtjndsveah.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gtrzjhscxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtvocbyxwf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.c1oappe.top/gtvwwecwwy.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtofrdcyqp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gtwipjburb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtesmvqhfc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtlzrejjud.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtwevnazjm.html

================================================================================
来源：http://hz.hysaishi.cn/gtfizwwjeq.html

G. 面向对象
来源：http://hz.sxryk.cn/gtlwemnmgp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtadelubov.html

[G01] 定义类
来源：http://hz.meibo888.top/gtetztzrnx.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtvvouoeqg.html

PHP:  class User {}
来源：http://hz.ywan-chungtsiang.top/gtqwghfmrr.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtphozbyrk.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtguchebhl.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtcgsvylum.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtjzeqtfmg.html

Ruby: class User; end
来源：http://hz.52xcode.cn/gtmzfoicba.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtodteadda.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtxxjjxagh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtrfslelcf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zycfv.cn/gtxwsdgcxg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtlogqwmbj.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtsznznsxb.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtapisfwqo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtbqllqcjk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtujfvxyak.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangtech.top/gtmpuckdsl.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtiqjpobbk.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtwpymgopc.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtsqebnssc.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtypnhsegu.html

TS:   name: string = "x";
来源：http://hz.jqgufenzy.top/gtlizlekvo.html

Java: private String name;
来源：http://hz.hysaishi.cn/gtpdmfvekc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtspwwzrrb.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtyeqpdwgz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtxfdrcnmx.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtsgpwpnsp.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtlgijimdj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gthmvsmdmm.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtdrhbfwpq.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtkrsbnqnj.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtcltxmabd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtuisyyjdn.html

Ruby: def greet; @name; end
来源：http://hz.52xcode.cn/gtgthhgefx.html

C#:   public string Greet() => Name;
来源：http://hz.nanxinkj.top/gtqbbzbgqj.html

[G05] 继承
来源：http://hz.mhx1999.top/gteoatgsic.html

Py:   class Admin(User): pass
来源：http://hz.9152youxi.cn/gtyfyabilg.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtnvfyxkoo.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtgjrsyxdm.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gteomepdgv.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtfucvrdxx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtrmjysbry.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gttrjcbgng.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtokleuyau.html

[G06] 重写方法
来源：http://hz.yonumen.top/gtjfzghrex.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtevjmvxnt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtyfofnycg.html

JS:   greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtjaoxdwci.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtzdfyoody.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtqecdafqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gticmxraxl.html

Ruby: def greet; "admin"; end
来源：http://hz.cheryme.top/gtmlbweopi.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtdxsqeroz.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtknctflxt.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtjwlbvobo.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtxseztzkk.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtkhqucffl.html

TS:   super.greet();
来源：http://hz.guannengcc.top/gtuhzthopq.html

Java: super.greet();
来源：http://hz.mhx1999.top/gtsuqlivar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtersopaqu.html

Ruby: super
来源：http://hz.bjfxy.top/gtiwirwbkb.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtawyhcjan.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtsqlqsqjt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gtpqrujqkm.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtuqzyiqua.html

JS:   static f() {}
来源：http://hz.svipenyu.cn/gtpcakmnny.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtlkncvwdw.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtxfitpgjy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gtmgwdkgtt.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gtddtrhadw.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtzysacbsi.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gtytoxdxfm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtnkjhnaui.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gtaxaicvdp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtyifwvbmt.html

TS:   interface Shape { area(): number; }
来源：http://hz.daria6918.cn/gtjvdbkpgt.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtfafftgth.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jyoumei.cn/gtibbajvhn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtjzgnnurn.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtuilwtxpa.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtplqdfipr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtbojcjqry.html

PHP:  public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtjqxmrxpc.html

JS:   #private 字段；其余公开
来源：http://hz.mhx1999.top/gtdchyeanw.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtrfbrfqoq.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtgeiatuzb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtlemsjmye.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtgslzshim.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtscqznwtj.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtgiormwij.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtakertcoj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtcwhmtubi.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtiicgdemt.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gttpvutjeb.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gthlpzpiga.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtyszthrmo.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gtfybgjbxy.html

C#:   public string Name { get; set; }
来源：http://hz.zycfv.cn/gtrtudshmc.html

[G12] 对象转字符串
来源：http://hz.jinqigufen.top/gttcefuleb.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtswimbbmt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtmtznnjag.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtujhgxadj.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtogfivhrq.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtrlnhkgmp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtynmftcej.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtmushulqx.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtagtwhmzb.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtbrycbixu.html

Py:   isinstance(u, User)
来源：http://hz.ivvv.top/gtgdojepjn.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtfxshsycp.html

JS:   u instanceof User
来源：http://hz.guowangkeji.top/gtvbctqsog.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtpwbhkecg.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtcgryvsmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtxsrdkyds.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtkicbdktu.html

C#:   u is User
来源：http://hz.316326.xyz/gtsktaogjq.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtgtantfpa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydzc1.top/gttnncdjqc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.andypj.xyz/gtnqujsihw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtwxylcxae.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtgszjyzhg.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtqeivfchr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtmmgabzfo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtelomodkk.html


<!-- 参考信息 -->