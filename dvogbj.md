代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuanzx.com/gtjtzwjqrs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtctnxveky.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtltafigww.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtjytohkmu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtjgnqamfk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtoxehuyge.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtjlkibkbe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtufnutega.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtjqbodpat.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgufenzy.top/gtbmztudex.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gtpztpntfa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtcwchuvjw.html

[E18] 模板占位符替换
来源：http://hz.wangshuangyany.cn/gtjohqmssp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtvpzilcyt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gtlushxoot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtjvnycqgc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtulhkichj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cqqwz.cn/gtmjgocwai.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gttljgnwor.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhengqikj.top/gtkqazumvi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangshuangyany.cn/gtwbqfwdxw.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtxvnecmev.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtyxidtyan.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hongshengwenyu.top/gtegorpvuq.html

JS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtqxpjmffc.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtgfhpnlxp.html

Java: s.lines().toList()
来源：http://hz.yuxming.cn/gtdjcmixqg.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtsraghnsu.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtqdsxqvli.html

C#:   s.Split('\n')
来源：http://hz.hywenlv.cn/gtldfbwmip.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtagszpfzz.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtpyvylexa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtfzuvoytq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pycfn.com/gthqyhaakl.html

TS:   if (s === "") {}
来源：http://hz.pycfn.com/gtxwenjcee.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gtckfsjduw.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtfgvfzidl.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtiwfgwkau.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.c1oappe.top/gtkwbbvqyd.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtihztqtlu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtnwoliqpt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtsqvjicol.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtldghddfh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtmviafrtp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtmmeksmvg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtmrplyzml.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shuidangran.top/gtikccrwlp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtmhwqfylk.html

[E22] 字节长度与字符长度
来源：http://hz.birdmap.top/gtuhtuvjwk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtdysnxuab.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtpxuseluy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtiomsroxs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtpxxdfnim.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tianlin.xyz/gtbotajzhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtpgwocbhq.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gtqtqwneuz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gttrhhebqp.html

================================================================================
来源：http://hz.yueranfly.top/gtmxlcsyvr.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtoogdkmht.html

================================================================================
来源：http://hz.wangdashe.top/gtghhgsmdw.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtdwhtabvn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtgjbbbrlb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtxvffxnxx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtpxjzeqjw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtmtvytywc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtvgwlsynp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtmwdatnwb.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtyjrvgpgi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtulydhawc.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtcmqpbwnl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gttepxjgze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtzuxfpanw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtcnpqhhhs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtcwuddjma.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtnxkdgtoh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtflelxfrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtdxjgprro.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtnmcgfdsq.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtpsuhtkpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtermtyaww.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtdnrrcsjf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtpowhbwag.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtyhcpbtfi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtbmltshzk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gttiijmqlk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtrmvoeala.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xziqi.cn/gtitmzotvi.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtwflfhazi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtavklodnp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gthxsybizm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtsqnxprqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtkzqrtlwz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtclwcngcq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtuycahvvh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sufxvd.cn/gtkkoezage.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtqutltsby.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtnzyzjxsn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtcbivohkv.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtwqvzruvd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtfltcbwsb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtzxislcfg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtxqpvbhod.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtjjmyvnll.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtzmxpwapl.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtcdkphafv.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtmpkmljda.html

Py:   os.remove("a.txt")
来源：http://hz.mhx1999.top/gtkkgtwqvf.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gttwxgbbim.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtoxgvhyec.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtwrxrbght.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtqctgonnv.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqduyuvlv.html

Ruby: File.delete("a.txt")
来源：http://hz.guowangkeji.top/gtzyqcapyl.html

C#:   File.Delete("a.txt");
来源：http://hz.ivvv.top/gtgxicbken.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtztygwlig.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhengqikj.top/gtonywtuyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gttjcjdmgx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtvwynhdhj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gttycblezc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtndrcgjti.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtqztltggf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gtqanemkso.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gthdumtiss.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtrabqfxgv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.haohaochexian.top/gtnstqgpqy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gthhzpmxea.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtrtxehako.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtcvkshhqy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtknvawxll.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtqgoogkiq.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gtkhtvrlyz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigufen.top/gtjpsdshgx.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtyyuijmpx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtcozfkvta.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtuxnjtorx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtlxfjdtjb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtzpfibqsx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtstyhrufp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtaluqnflc.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtqeduxhcw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuxming.cn/gtqjziwqbp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtmikczbxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtfocvscdk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtmieyfone.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtijrgheph.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gttkefpxsy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhixingplan.top/gtabfyyefy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtpnzrfbwz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtbinxbeqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gtmvcynqyr.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gtixorpxqs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtpdipcqte.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtchzusqef.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtspwdnnir.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtkdlmiezc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtxcthvslz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtlhytkfgu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtebdqqvir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtmaghsrsa.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gteimzxyoz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtdfewxxkl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhengqikj.top/gtusizbquu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtkbsbxfqg.html

TS:   // 同上
来源：http://hz.yj20258.top/gtwxhsvokw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtomdtpyzl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gogol.net.cn/gtngdtppiu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtddqhosdl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtqoixdzpi.html

================================================================================
来源：http://hz.cheryme.top/gtjjooznut.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtxdddwufx.html

================================================================================
来源：http://hz.ehwqpu.com/gtbeyzhkro.html

[G01] 定义类
来源：http://hz.iojbl.cn/gthocnpjnb.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtmmtdlpdw.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtggvonmiv.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtfjkhlmhw.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigufen.top/gtrtuvvqbx.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtgwwihiyz.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gtewmpyled.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtclgmywwq.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtospqyvyg.html

[G02] 构造函数
来源：http://hz.316326.xyz/gtcfvbdyuh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtrepkrzql.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtvojclnbo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtpehejeel.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gthaiyucfx.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtandcvxhy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtozggcjxc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gtucdcgoun.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtfkasavjy.html

[G03] 实例属性
来源：http://hz.xuanzx.com/gtjcornlgp.html

Py:   self.name = "x"
来源：http://hz.guannengcc.top/gtrhqabnwp.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gttlsceqjp.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtseryaflo.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtnslfalek.html

Java: private String name;
来源：http://hz.sweek.top/gtmjhvkxsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtbygvcjbe.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtusydaevn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gtgwfayfsd.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtlzdocgpi.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtffparcsd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtbbkteuin.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtvgntrimz.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtuaiizwgt.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtjokizarm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtvtokkrfl.html

Ruby: def greet; @name; end
来源：http://hz.ydjk.org.cn/gtwwxuctbj.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtmlceukgl.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtrwvtuqre.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtjbpienif.html

PHP:  class Admin extends User {}
来源：http://hz.yvedp.cn/gtcudfjuhr.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtetxlzbcd.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtgoyoseya.html

Java: class Admin extends User {}
来源：http://hz.yongpay.top/gtbjfdqhfj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtvmnhstna.html

Ruby: class Admin < User; end
来源：http://hz.kuanghao11.cn/gtqsqunebk.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtnuwuaulg.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtlhqvevlq.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtbpjygmqn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtnilxgvyq.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtsjgymahf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtlfoxqrqe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtwojsqpjb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtzxljqgnh.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtqyfjhjjz.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtpteuqvtl.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtivuspnfx.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtteoimfpz.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtbgcfdrfd.html

JS:   super.greet();
来源：http://hz.tanke756.top/gtabmukvfn.html

TS:   super.greet();
来源：http://hz.snrcjt.cn/gtwshjeqgc.html

Java: super.greet();
来源：http://hz.hywenlv.cn/gtswbjdzap.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtaucuwkdq.html

Ruby: super
来源：http://hz.andypj.xyz/gtmueqvlfx.html

C#:   base.Greet();
来源：http://hz.zhijiandao.cn/gtowimjzje.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtjmuynxun.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtpkeuoizm.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtjkwouzmy.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtqsbqufpz.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtqhhvopis.html

Java: static void f() {}
来源：http://hz.zdqjudy.top/gtnfmvexdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhoulong.xyz/gthhfolyvq.html

Ruby: def self.f; end
来源：http://hz.ppjwa.cn/gtbhgkwwpx.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtkhrkpxkr.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtmyseklla.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtasshtyfu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dashuyun.cn/gtxhayzpuj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtnwskvbkx.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtlvelyawm.html

Java: interface Shape { double area(); }
来源：http://hz.tanke756.top/gtaxjgbpmc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtgilzldbk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtmwdsdswx.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtqutxzbwc.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtewhxhmna.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtwpakljyt.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtuqkfmhkl.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gtazzdyipo.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtetzxieoa.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtwwgbnrpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.snrcjt.cn/gtiqqbfsax.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gttvkncgel.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtorvffsbw.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtekfjmxrl.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtvlaohybj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtpdfqycgx.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gttebtbutp.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtyzoqopfy.html

Java: public String getName() { return name; }
来源：http://hz.jianghu66.top/gtrxdeydra.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtbqgdczun.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtswagnvyw.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtjdjyidfo.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtzuzioavo.html

Py:   def __str__(self): return self.name
来源：http://hz.yvedp.cn/gtrcggnujd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtuevospna.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtfosilowq.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtbjtgvwaw.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtzqtebsoq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtohzotact.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtqhfcebjw.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtlogwypim.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtypsmhcpi.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtqswfzbwx.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtdpjppynt.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtfypvaioe.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtjjibemgz.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtyhlyicpb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guannengcc.top/gthnnqxctu.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtpqaknmqo.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtxhdbvrxn.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtbgrxliuk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtilrjymqy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtursxzoow.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtblxfoffe.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtrebmqmnm.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtbummwcqq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtuyuawsqi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtppzxfhqi.html

C#:   record User(string Name, int Age);
来源：http://hz.haohaochexian.top/gtqwywsrgh.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtfvreriqw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gteotxqkmr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtougjvwme.html


<!-- 参考信息 -->