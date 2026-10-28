代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gtnuavsjik.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtxvlwvabv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtvafdfufc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtiyymymxj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtzbnmadcn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtissjgbzg.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtrzdjcesl.html

[E17] 首字母大写
来源：http://hz.nwbrower.top/gtqsqqwqdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tian-w.cn/gtqtelapfw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtoicwkjja.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtsxrrsyri.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtmmkpmjsa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtwgkwpcds.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtftzlyutt.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtilegmbpj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtblzlotcm.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtiqaxvroj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtwytwdvhs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtyzsvxkxf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtuixyyswk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtqcobsztc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gtslucmciw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cucudq.cn/gtvihyqbmu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtffjtlwbo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gaohongyu789.top/gtyvgkzsto.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtnxhpegob.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtssvmkhjb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtdrzrwhds.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtuyfuegsq.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtaaxjjhxj.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtuajzrvhz.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtkkrgkgxk.html

Ruby: s.lines
来源：http://hz.zhaomingkeji.xyz/gtzauxijya.html

C#:   s.Split('\n')
来源：http://hz.tian-w.cn/gtutaedlno.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gtxmkbuaxn.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtsytqxjbl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtjxadftql.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tian-w.cn/gtqcehdhks.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtlsibdwyh.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258888.top/gtjmfaiknm.html

Go:   if s == "" {}
来源：http://hz.52xcode.cn/gtkdiyujws.html

Ruby: if s.empty?
来源：http://hz.yangfankeji.com/gtnrzvnvam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtnqzslstu.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtvkuxniuq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtzxigyxky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtolpmlgwb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtsqumdbye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtalznqzrg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtseuawogj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtepbgqhej.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtoxhqjkfu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtwpfwyqdf.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtkmsspqbj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.havefunace.top/gtltswpfsg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtqvofmtfq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gthfhnfdgu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtizcsyzao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtwcabbqdj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtfgcwusxk.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtdllmnsbt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.snrcjt.cn/gtmtmssyzj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmtfzaaaa.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtncrztbvf.html

================================================================================
来源：http://hz.birdmap.top/gtunvstrtg.html

[F01] 读取整个文件
来源：http://hz.zhengqikj.top/gtyusfzauz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yongpay.top/gtpfvndkgn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtnuoelkut.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.snrcjt.cn/gtobfalsvl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtnlnevaui.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtngeylxbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.andypj.xyz/gthndkergu.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtzfcwsadd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.haohaochexian.top/gtdjyjwxit.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtnqpejvdq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtzvupvnsh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ybcxt.top/gtnvwhyjjp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtggonclrh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtbrpxrggv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtyirxkjzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gthcnjqeag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.iojbl.cn/gtrjifblmf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gtecapwigj.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtjdjpfyzj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gthramkqdj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtopmbogkb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtmsfbdddw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtnmvhpcrp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gthiaihmue.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gttabrxpgj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtpmndetud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtuccvsmkk.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtjcfllbtg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtbqtkzqjl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgfzy.top/gtkolvpjzm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtkfpipabw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtmxuwnxat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtszydapib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtwvlqwufl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtwzqtvnkk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtxaewrron.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtzgsrmokb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtpdohxeja.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gtsmokkrou.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtltlbwtkw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtndgelvob.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtpfmterqk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtuiadbeku.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtjcjwrosm.html

C#:   File.Exists("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtbyqphmww.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtmgndabqf.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtdgdtpbys.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtzwmmqxuh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtfouamurg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtbonofafv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtxgygpxrz.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtkjrspvpv.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtkmbznfga.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtvcyyijab.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtgdemqrfk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtiylnopoa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fengsongda.top/gtgstlrfgd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gttpoqifsz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtrfhqahok.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtqewuqyek.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hywenlv.cn/gtqkyudjnb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hysaishi.cn/gtamsrwwfx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtootruofe.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtnxycmirb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtqparmrnv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jianghu66.top/gttlvywloq.html

JS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtieexqrit.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtovxdlfhx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtlsqpnlrg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtaokefnwo.html

Ruby: Dir.children("dir")
来源：http://hz.yueranfly.top/gtfmeloaot.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gtwnyxtjbj.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtevdzdjto.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtgdoyaays.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gtdjbtsici.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtgbpvysyr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gttsgmccpr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtbgqfhsyh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtgefuiwry.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gttkjmjhzj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtopaapxby.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtbungtilt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtlfcsgbdz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtjivcyknv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtqkacxdjq.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtsrjtgdhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj202588.top/gtukmfzjtx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nwbrower.top/gtjaqmggfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtgplqptxb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtpnyuqfpe.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtrsvtmxci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtqizadxnm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtajieikgc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtxapieqvu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gthnixazau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinghuilouyu.cn/gtjxtuvzhs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtvjgjevhw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtjyjrpvjw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtjriuhvse.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gttaogviax.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtqjaminbj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.iojbl.cn/gtijvhnmcj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gtfilrqcio.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtcblinbnh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtiylpmifz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtwvxqrauj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtrrrrofzh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nwbrower.top/gttzcxoitp.html

================================================================================
来源：http://hz.cheryme.top/gthpxtcjxu.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtiinajvec.html

================================================================================
来源：http://hz.cucudq.cn/gtfyxredfr.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtdjyufzpw.html

Py:   class User: pass
来源：http://hz.yuanzhike.top/gtgdyuhulr.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtnbhrcjzl.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtpevbricd.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtlgqsskyy.html

Java: class User {}
来源：http://hz.yj20258888.top/gtantuvocv.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtigsrqeca.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtmbcrvywr.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtsjkbnebt.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtgooeykyp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtndnkbkxb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtlpxwtzqq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtydblzktd.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtdbgyknia.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtofkyjzga.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigufen.top/gtfxqrilvj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.kuanghao11.cn/gtvfcjdkfy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtzdwtlwkp.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtcansykad.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtlrdzpcdk.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtdxhtslzv.html

JS:   this.name = "x";
来源：http://hz.haohaochexian.top/gtyoeoktwd.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtwnbtkxag.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtjzalrysm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gtbocmxouu.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtesiivvku.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtficradyg.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtdosphhpo.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gtzsxiujnx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gthpochwwf.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtqihczktu.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtduexausb.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gtutieivlw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtbzvbanml.html

Ruby: def greet; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtoyinuenl.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtwuranwfw.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtfdmxvrzc.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtqpcnlosn.html

PHP:  class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtjqbqiaca.html

JS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtcmtqickk.html

TS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtohjqjmbg.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtqtiishby.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtzbwabkjg.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtndjvutuv.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtfcbfgoqr.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtxctyqnrg.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtjnnpcniz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtwcutjytj.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtstuqmdbu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtymcdqyoh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gttxzknlkg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gttiivzmfd.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtpwfanqng.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtiegdptsl.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtdivnkejj.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtgxfyoxld.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtyvzxomkx.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtyugbqnvo.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtgjqcfwvt.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtqyeqijjg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.andypj.xyz/gtyzndhjgh.html

Ruby: super
来源：http://hz.hysaishi.cn/gtsogsohwm.html

C#:   base.Greet();
来源：http://hz.jqgfzy.top/gtakcgrxxo.html

[G08] 静态方法与属性
来源：http://hz.guannengcc.top/gtxbyarkvc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtxwzdisgi.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtorftpqhk.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtxcaieymj.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtsjdimysm.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtpanqtloi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtkmnmkjli.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtddnbqkaa.html

C#:   public static void F() {}
来源：http://hz.jinqigfzy.top/gtvchwfnip.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gttrvvlfst.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtgnzpluia.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.birdmap.top/gtepnufwfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sxryk.cn/gtzaybthyf.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gteczpfijt.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtldztwfyo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gtddtahqge.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtwdrsbxrf.html

C#:   interface IShape { double Area(); }
来源：http://hz.birdmap.top/gtkmqismte.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtnyjebbtr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtkylvhmvj.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtsnraojko.html

JS:   #private 字段；其余公开
来源：http://hz.birdmap.top/gtvqxjxvdk.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gtftesityv.html

Java: public / protected / private / 默认包级
来源：http://hz.jlsjyb.cn/gtlmfxlsae.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtpfubynvh.html

Ruby: public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtoemrcxfl.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtkqyhcgpm.html

[G11] getter / setter
来源：http://hz.hnqzz.top/gtarczugfi.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtowkwmlxw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtclxkwlnh.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtvzzckjam.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtduzldccm.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtqsfgimsi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sxryk.cn/gtbrgrqkek.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtfpbmqyqv.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtvadgcmdk.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtdjhqzrji.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtirvzfwxv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtwawylzpt.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtxztndxgf.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gthakaammf.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtkgliclcq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtahlorlpx.html

Ruby: def to_s; @name; end
来源：http://hz.jianghu66.top/gtsdjycgvc.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtisxjozzr.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtipgfujed.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtvkxnqzca.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtvbxbsxvg.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtnflmtjhd.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtndiavwxw.html

Java: u instanceof User
来源：http://hz.pycfn.com/gthufqxjfd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.vqdsnc.cn/gtwvozxbfk.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtrpzrdrjk.html

C#:   u is User
来源：http://hz.316326.xyz/gtrxsvvftz.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtxovighap.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ppjwa.cn/gtmjbcanlr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtgytpxtos.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hfpthk.cn/gtoytwwswj.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtowitsftq.html

Java: record User(String name, int age) {}
来源：http://hz.yj202588.top/gtcnbnojck.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtrgiieclc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtnnvlwhya.html


<!-- 参考信息 -->