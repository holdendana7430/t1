代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtqymsjopy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gtdjcrjanx.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258.top/gtgccouuop.html

[E17] 首字母大写
来源：http://hz.jinghuilouyu.cn/gtextsokwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtwizrhknz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtgclztjbr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtkvbrskkv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtwzysvsqw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtznlerpgw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj202588.top/gtowfrgxmy.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gthfrwmcdh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtpsmeayua.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gtnnswkcci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtryiclysc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtmleaispn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtqjynpvdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtfsulaida.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cheryme.top/gtcyapnoow.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtihqlascn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cqqwz.cn/gtitnrunsp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.redwolf501.top/gtytekihfn.html

[E19] 多行文本按行拆分
来源：http://hz.hnqzz.top/gtqpyrrcvd.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtropjvtzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gttwzftewo.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtazuirtow.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtrrcvmofn.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtqusjsjup.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtlimktkla.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gttamluuie.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtztcxjkqs.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtjhhadhmz.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtxhpaphzc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtagvafvzn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtkcrhzfpo.html

TS:   if (s === "") {}
来源：http://hz.ppjwa.cn/gtuoutnkra.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtmzwulany.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gttpnamnvw.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtgtzustma.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtrpneirhc.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtdkuxbfjp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtiyeofnrc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtxbdaagbw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtfphgrcgv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtfddhwiyb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtnyvnshtk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtiatckjnc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gthuzjmgke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtsnsikkqt.html

[E22] 字节长度与字符长度
来源：http://hz.xuetiantiany.cn/gtwiiimgbh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtjpguntdv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gthearwcfs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtifnykafv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtyamccbrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gttsvqbomt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtgtkkgpqq.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtjvakawny.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtikrpawbg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfyouzxxk.html

F. 文件与目录
来源：http://hz.tian-w.cn/gttdkzhsdk.html

================================================================================
来源：http://hz.chenlongwang.top/gtuujikcrn.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtapayjzog.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtgrrmoajs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigufen.top/gtamdtojbh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtykrzjvwp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gtwfdndntl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtuipatydq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtyqgutbjg.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtrljqwsvy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhiwuduotai.top/gtwgoamknd.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gthptgyiuq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.kuanghao11.cn/gtclrsfydz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtyxtmxqtu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtxwzzhmvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gthxxmtlhu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtyrwnqaac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gtrdrxqsao.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtsulzybfg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtsdcrabcq.html

[F03] 写入文件（覆盖）
来源：http://hz.shuidangran.top/gtquudkjsi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtamqudzvi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtjzoulbil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtvtifitbe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtxooxpxht.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yonumen.top/gtbgwuoeml.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtshwuonmz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtoyfqkufy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtoponribw.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gthbwwwgly.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtwberpejz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtnwyxjtgn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtctsyptid.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtoeimhshn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtiiohusdo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtuvwceyxw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtbbefdcfu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtlkykitnb.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gtvuckwnfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtaelkygua.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtyraakerg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtcbklprap.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtohptktjr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gthqalwcmw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gaohongyu789.top/gtrddlwxxl.html

Ruby: File.exist?("a.txt")
来源：http://hz.zycfv.cn/gtuquskztm.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gthhdwirub.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtguzbnjhv.html

Py:   os.remove("a.txt")
来源：http://hz.yangfankeji.com/gtxzvnvynh.html

PHP:  unlink("a.txt");
来源：http://hz.meibo888.top/gtszylicud.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gttiravzyy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtqdximjom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtyvvqxajy.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtgjtlcpol.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtecmmgnlg.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtjravrrke.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtbddlrixm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gthqsgjxdz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtkdauqfao.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtryveeyvi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtylpoizby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtbkolrkla.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtdnfbogxl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nwbrower.top/gtymfniksk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gtzgnvlmvz.html

[F08] 遍历目录
来源：http://hz.zycfv.cn/gtewnjifnm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtokrufmyp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtkmuywzan.html

JS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtcamvzqzr.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gttugpzpjz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtmkafxnjo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtzfelqwvy.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtemplhqsb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gtlcwoviez.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtknhudehn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtosczyycm.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtxdpjwyol.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtirywdsdl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtsvfkdijn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtbrveafpp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gttgymjddl.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtpgjqvoai.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.haohaochexian.top/gtnvhylwhp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtqmmjoljv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gterkeqegh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gtuzwlqwky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtdkvdvvfz.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gtokkodwmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtmrkexcvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtqgpvjees.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtibrmlvpu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtcgkjwidz.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gtobrbpzwj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtutmnrumg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtbzvbgjuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtuwtuzdka.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtjlyvfvxu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtgwyegozs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtlhhjnagz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtkrtmouac.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtflubopyw.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtqobjrbxf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtkqsfdker.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtsbasvryf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtegryadke.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtyxrsdjfa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnqzz.top/gtaqwhzyhv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtnedmpdih.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtriumlpke.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gtlocidtzv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtowwrbkcr.html

G. 面向对象
来源：http://hz.aizwys.cn/gtxxfpgqig.html

================================================================================
来源：http://hz.fzhhl.top/gtjwikehpt.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtockhdszz.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtfvtgqmdq.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtixviropx.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtizmohepa.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtteybvqia.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtehusbwwz.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtovzrjeww.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtmhwxidrv.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtyoaqdzcq.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtuxyjjjkf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtjlzjjprx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gtebygvhzs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gtlgklkjbc.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtywisxrqd.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtgxbnwicu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtqkasnufk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shuidangran.top/gtxeqwagnt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtkttbxsrl.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtqzasqyqb.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtatwqhwub.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtulkhlndv.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtivxsrxjb.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtwlyekibp.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtswbnctfk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnqzz.top/gtyekrigzn.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtxflfsfxw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtiipevkwm.html

[G04] 定义方法
来源：http://hz.pengpengdd.cyou/gtsdjqrwfm.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtjljfedtz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtpfwzpyki.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtwrzntvjl.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtswcdldjo.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtbvrpnbgy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtnqwcmggm.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtvizvzqjs.html

C#:   public string Greet() => Name;
来源：http://hz.dashuyun.cn/gtwgiobplc.html

[G05] 继承
来源：http://hz.daria6918.cn/gtabmmgxvo.html

Py:   class Admin(User): pass
来源：http://hz.yonumen.top/gtevdjkulr.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtvwawymzf.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtxewwpkdi.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtcsuwvtxy.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtpwcedrse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtaouujltg.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtyyflmphr.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtscbpiotd.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gthdtvaekb.html

Py:   def greet(self): return "admin"
来源：http://hz.guannengcc.top/gtrjyjuwiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtjcrqqiwj.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtrhddkutz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtkzbyewlf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gthdrdwwyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtbhuztkis.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtuphtromp.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtemdbqvty.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtrvszgpxt.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtgrteskqp.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtsxqmcnkz.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gttouyhnnx.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtfytxgkji.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtanznqtnd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtbiarzffh.html

Ruby: super
来源：http://hz.shuidangran.top/gtebwjjtuw.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtyisexkic.html

[G08] 静态方法与属性
来源：http://hz.shangyingyoupin.top/gtlvvcirdm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cheryme.top/gtgvawpucz.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtpzgrasth.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtkcqhjpsz.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtezcpzhrj.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtrjrahzjq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtfemjwmsk.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtyeolxoop.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtpzycdwvh.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtzupdaqxl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydjk.org.cn/gtchdjgwdp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtyeklwefe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuxming.cn/gtcljtqsxa.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtqyqgnode.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtcsuxplmi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gttlainujh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtusxxtxbh.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gthpcuowaq.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtfpieupmp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtlfuqizga.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtcgsxhivb.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gthuehrpyd.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtlezowwll.html

Java: public / protected / private / 默认包级
来源：http://hz.yuanzhike.top/gtbubexfdh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtljubldux.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gthjmoqxoh.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtmthuaxkv.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtytznnjsm.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtnoruratm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gttzqevwrs.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gttqykteey.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtaiubrmgb.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gtoklljvbf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtgdfuqnxw.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gtgrqdzvuv.html

C#:   public string Name { get; set; }
来源：http://hz.wangdashe.top/gtxhakngvf.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtcwbmqeyr.html

Py:   def __str__(self): return self.name
来源：http://hz.yvedp.cn/gtmezmwqrq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtexxqkyxl.html

JS:   toString() { return this.name; }
来源：http://hz.yanxiufei.cn/gtnrkmhafw.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtswoervhx.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtesmvwdzw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtqntxgbvx.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtormtsikm.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtwbdtntjw.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtobkkdckp.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gthfugrlxb.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtsibfzmgf.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtgxstigtm.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gtttiztwew.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtvzafeobw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtvugxksmq.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtdbdyoilg.html

C#:   u is User
来源：http://hz.nwbrower.top/gtivdpjspn.html

[G14] 数据类 / record
来源：http://hz.smart0.xyz/gtdiezdcql.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtcbcgrgwp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jianghu66.top/gtrvjakvow.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guowangkeji.top/gtjdvroedn.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gthwtuwnoa.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtpkfsmpkt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gtwwxhegxp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtkknguyoi.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtpnvabfnp.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gtrpjmszfm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xziqi.cn/gtpcmrbooy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtbbczvzgz.html


<!-- 参考信息 -->