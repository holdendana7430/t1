代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtuwqmjkxx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtodeugqfs.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtppqaohjj.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtqypmikdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtlhiaxusm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtnicitbdj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtooqzbpyg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtimxljdor.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtkjamsqkk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtowzfgkrd.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtgmozyioh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtkbzxhdsu.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtlnxtpqdf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinghuilouyu.cn/gttnymaedk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtdrzixdww.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtwojlskkb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtkofmjsmu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtxkruigpt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenzaomai.com/gtaftwiivn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtaxuajbqa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtrihqzaxs.html

[E19] 多行文本按行拆分
来源：http://hz.316326.xyz/gtjttrwrdy.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtxzzsvvwl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gtfawzcpsx.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtnzrmeegl.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtaqrbhqqa.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtottqrjyk.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gthwzynqdb.html

Ruby: s.lines
来源：http://hz.shangyingyoupin.top/gtbqfggedd.html

C#:   s.Split('\n')
来源：http://hz.tanke756.top/gthixtkuyc.html

[E20] 判断字符串是否为空
来源：http://hz.iojbl.cn/gtffaeiapl.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gthqqbuouc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gttfdsearo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtxmanycea.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtsdhrldqq.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtishcpaso.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gtgkuqkjhv.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtpbtkhuhp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtetqanluv.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtwyckvvka.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtcglajkzw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtncrfbtnl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtshpjxsvj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtzetoyppm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtcpuwqbnc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtwcprbemv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtsknslwkf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gtbwareydv.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gthfndmupd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gthvpoxrqp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtddkpbtvi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtyqoumbac.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtmywczogg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtzreqewsa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtoxoigpcq.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtlolsfbvk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtbprtpgmm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtnaebqkny.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtnvyjghqo.html

================================================================================
来源：http://hz.sysykeji.top/gtdruxtquk.html

[F01] 读取整个文件
来源：http://hz.jinghuilouyu.cn/gtoefsjvyn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gttimowcex.html

PHP:  file_get_contents("a.txt");
来源：http://hz.andypj.xyz/gtpgdukyck.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gtkfnlxyfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cashguo.top/gtahrwgjoz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtthdotckb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtsxzhwfit.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtpbgqdwqu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sweek.top/gtlwmvfjes.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtwpmrkvyq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hongshengwenyu.top/gtjszwntre.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtrqiocgzq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtsxrsmbwj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtkdytxzlm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtatznokjo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtqltxiraj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinghuilouyu.cn/gtxqjuozwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtpbolxljq.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtfyyijtpd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtiodxlotk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtnbaehnac.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuetiantiany.cn/gtqjlelsug.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtptpqemzs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtuvkgacqy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtvguxcjht.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtivgsjqzw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xziqi.cn/gtqysgqpit.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtuqaxlhfl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtkkqhdspl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtgazwbilz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtgscciijs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtcupdjbav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtqdwzoiyh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtnyezkhhn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtwfgmckjo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guowangkeji.top/gtugsqtdsw.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtlwlhprfq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtgzybbpzf.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtmzcssiox.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtugspsxjz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtxhwdehjb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtxthjihls.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtpcaknjft.html

Ruby: File.exist?("a.txt")
来源：http://hz.52xcode.cn/gtkatvudfg.html

C#:   File.Exists("a.txt")
来源：http://hz.jianghu66.top/gtoomkdopy.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtiqcgpbni.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gtdoclohay.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtmdlvxqae.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtxagxkcve.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtjgvcykmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtvwerhcnq.html

Go:   os.Remove("a.txt")
来源：http://hz.zycfv.cn/gtvnjghsgt.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gtwoyvvqrf.html

C#:   File.Delete("a.txt");
来源：http://hz.daria6918.cn/gtiuwwfgsh.html

[F07] 创建目录（含多级）
来源：http://hz.xinyue.icu/gtpjavrhkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.0kj1m.cn/gtbvahkzrz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gtwptjyotx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtcjgpdctg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtvhzillss.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gttmpkiwsr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pengpengdd.cyou/gtngiqlupj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtxsrohcue.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtnnwuupcx.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gttvbhcvcf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtwjwqxmkl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtyrveuatx.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtltrngudg.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtfcbmtpas.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtaessthig.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtusubxote.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtzsuwxvwg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtbmyjgqju.html

[F09] 获取文件大小
来源：http://hz.hongshengwenyu.top/gtxtptfkuz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gttalvytnk.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtsaezboqc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtgddnypwh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtacboovwi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtpvcmgumn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtvbbzgwjp.html

Ruby: File.size("a.txt")
来源：http://hz.wangshuangyany.cn/gttjmhwzcm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxuanxn.top/gttvfbydmo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtpscofvmc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtqwoifnub.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yueranfly.top/gtpipofuip.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtazedeuhg.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtghnwsofa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xinyue.icu/gtbmcwsbkj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gtzcnekjxf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtdtbivdre.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtnseltkyi.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtbkibuvzr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtxtnwyaic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtfizaqnbd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtrdqhomyg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtiadqafdl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.quarkkingdee.top/gtqgbfaqxw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtqrbvqfzl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gteznajotn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtdxeblgrp.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtlumvakke.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guannengcc.top/gtipdkjehu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gtmhhtexmo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhongyouzk.top/gtxwoliwmx.html

TS:   // 同上
来源：http://hz.316326.xyz/gtosbwqqyx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtdrvdmlwb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gtopefwmfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tianlin.xyz/gtbatnacff.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hywenlv.cn/gtmrvcdoyr.html

================================================================================
来源：http://hz.yongpay.top/gtiwepvrmq.html

G. 面向对象
来源：http://hz.shuidangran.top/gttxwmjfbi.html

================================================================================
来源：http://hz.cdnleiting.top/gtfxjhhavy.html

[G01] 定义类
来源：http://hz.zycfv.cn/gtmrpndddo.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtrwkpxdpq.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtemlfmpoo.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtpknfvyzw.html

TS:   class User { name: string = ""; }
来源：http://hz.iojbl.cn/gtqdecwome.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtyzcroftm.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtdjuuharw.html

Ruby: class User; end
来源：http://hz.jinqigufen.top/gtixbmqghs.html

C#:   class User {}
来源：http://hz.nanxinkj.top/gtbagjzpyx.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtebkrfxbs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aizwys.cn/gtdvqmefni.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gthycwwuln.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtwldzgrhk.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gtecswtueq.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtupnzeavq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtcyewkncg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtgasqplib.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtrixoqojd.html

[G03] 实例属性
来源：http://hz.ppjwa.cn/gtypguttyk.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtkfycwhev.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtcmojmbfq.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtxxpjejxd.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtirbuqrsv.html

Java: private String name;
来源：http://hz.xuanzx.com/gtpufpyeyl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gthtwpawah.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtyiecdrnm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtktdjfzqp.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtjmkssciy.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtjgemktod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtqcgwuhix.html

JS:   greet() { return this.name; }
来源：http://hz.birdmap.top/gtszsjrgdt.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtcqonohrd.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtapdiwvlr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gthjvzucyg.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtvnrexgkm.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtyymermum.html

[G05] 继承
来源：http://hz.tian-w.cn/gtdhagktro.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtgrupfddc.html

PHP:  class Admin extends User {}
来源：http://hz.yongpay.top/gtlrzhjjlq.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtwbspemva.html

TS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtyjagkhpj.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtkbweffdo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gtlpadqxvi.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gtormmzlvs.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtqvblqvra.html

[G06] 重写方法
来源：http://hz.yanxiufei.cn/gtkuxcwcko.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtkqbsjixb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtkdbabjfi.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtnpkenlde.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtjpmxoetf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtfjvfljon.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gthgepaeuw.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtgcdvetcn.html

C#:   public override string Greet() => "admin";
来源：http://hz.zdqjudy.top/gtqqwozyyd.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtkzwcnvha.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtygibxhqo.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtrodwoiyl.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtodcaaagc.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtgmscsiva.html

Java: super.greet();
来源：http://hz.cheryme.top/gtnoocfwki.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gteleomgph.html

Ruby: super
来源：http://hz.chenjidiqi.icu/gtdjnfjhja.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtyctdxcdi.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtwagnonna.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtbujgauwh.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtpzejrzgz.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gttnlfvzfx.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtuaruyqwa.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtfokfuvwo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.kuanghao11.cn/gtxriigdfs.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtqhuwfgpo.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gtqughybhw.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtnwnbiutq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj202588.top/gtzlhpmgyk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtibsgwbos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtvauaobag.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtekhdatbz.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtvfgbvsvr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtemlnkvbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangtech.top/gtuzleczuo.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtaaicisqj.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gtiamijphc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtnjqwodoh.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtfhiuuxpn.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtngaloviz.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtqzotrcsn.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtajkkpdgm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuanzhike.top/gtcvmbippx.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtslnwmpip.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtmnnfamnt.html

[G11] getter / setter
来源：http://hz.shangyingyoupin.top/gtuilusrvq.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtvafprpvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtgctoywxh.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtwrjsnskh.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtvijnycvb.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtdsgjqvcg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtsivvkttm.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtbmmnvbkq.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gtmbujnthz.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtmyrrsmzs.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtuefervpa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtnrkqczrm.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtyxmwcnhs.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtbtwdasph.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gttihosqwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtsrtivgxm.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtzmykrjaw.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtbvvqoill.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtuvmymtin.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtezrdnyif.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtfakreiuf.html

JS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtodxwpddc.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtfflyernl.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtvqozjhuq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtdptojarl.html

Ruby: u.is_a?(User)
来源：http://hz.yuanzhike.top/gtomrqpsna.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtnmlntanw.html

[G14] 数据类 / record
来源：http://hz.aibaodan.cn/gtndrjpbwi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtwkgbqooe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtolhqqsiu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtnmkxhdbt.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gthktbsexa.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gttoxyedeo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtdlxcprqx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydzc1.top/gtoghaecyq.html

C#:   record User(string Name, int Age);
来源：http://hz.pycfn.com/gtldxlnquw.html

[G15] 枚举
来源：http://hz.316326.xyz/gtiyvsboyr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cucudq.cn/gtzsspwfnk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gttaikjert.html


<!-- 参考信息 -->