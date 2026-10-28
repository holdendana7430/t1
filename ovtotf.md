代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtnynsqjui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtfdvjvhyl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtdxycelho.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtchbhdhnk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtbvsemqde.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtilcwpcye.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtobwkwikt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtqlpghizz.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gtulwydfkr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtgiortzyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtmfmmzgnf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtumavibgk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtqxttasyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtheueumcp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gthvtfjtwt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtiklbypwu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gthphfbbiq.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtolgyusum.html

Py:   s.splitlines()
来源：http://hz.daxiang520.top/gtscnzzqgy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtrmpcmfwd.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtfqkynorm.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtbumqzfav.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtldvfvoce.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gteduvicgk.html

Ruby: s.lines
来源：http://hz.ybcxt.top/gtyntxctio.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtnorsoiro.html

[E20] 判断字符串是否为空
来源：http://hz.jqgufenzy.top/gtpgplepyy.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtejwloggj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtmarysjfy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtvpfomctq.html

TS:   if (s === "") {}
来源：http://hz.dashuyun.cn/gtqsogzqec.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtipceiiwi.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtfbnfejxa.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtalaxxnvr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtgnkyspyt.html

[E21] 超长截断加省略号
来源：http://hz.yueranfly.top/gtpnpsxrca.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtdwbbypkz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shzxlz.cn/gtobnaaxbp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtjbxuvrsd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gttaboykjg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtuoqhkfwe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xingfuxueyuan.xyz/gtlgzyjisk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtpqnuzxbx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zdqjudy.top/gtzurdhwtv.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gttjxnwvaw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtynhdxsfq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtihvfswou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtpkmysffh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtthescbps.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gtqzueaobt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtkrrhurfx.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gtdbjoziln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtnunlfffg.html

================================================================================
来源：http://hz.hfpthk.cn/gtfirmgxbf.html

F. 文件与目录
来源：http://hz.tanke756.top/gtaqcdttcu.html

================================================================================
来源：http://hz.yuxming.cn/gteechjclx.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtpvietocp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtzxifaqwo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtqnbwefas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gthvljmncc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtxzmvznsd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtwxbcsgcd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtqhugwzwm.html

Ruby: File.read("a.txt")
来源：http://hz.jianghu66.top/gtvmiljzsr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtlkydugdc.html

[F02] 逐行读取文件
来源：http://hz.yvedp.cn/gtjqhbhcib.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhoulong.xyz/gtipwccxtc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gtelkyjbsb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pycfn.com/gtbqyojbue.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtkykyhjsv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtncocmzdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtkxxnrxxl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtenjyzsvb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtkjsgzyfi.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtissnirbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gteinjbkyp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sysykeji.top/gtnqthemwp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtzefkpdyk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gteubdrqcs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtevwntzjj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gttispjvdi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gtuihyiykr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtrfelalvc.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtnzgmwisn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtvcebbybk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shzxlz.cn/gtnhkspakn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtpobvcfcd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtfqkmevps.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtgqgxrwen.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtfjizohky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtajbsmmkn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gthyghfrfl.html

[F05] 判断文件或目录是否存在
来源：http://hz.snrcjt.cn/gtiszmklhv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtkcrqhvrm.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtwvnbxkcb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtzgdqeqio.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtxuycgwlt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtvmehbfqy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtlfhdcduq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gtmspxblkp.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtebxigpgj.html

[F06] 删除文件
来源：http://hz.xinyue.icu/gtqhlmlzzm.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtlhdrljzq.html

PHP:  unlink("a.txt");
来源：http://hz.zycfv.cn/gtrhpyqpbh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtkuqvjstq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gttoopuzsb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtcsvcgzym.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtlqaqlwbz.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gttqaxdbor.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtahwbilwy.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtxcdhufta.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sufxvd.cn/gtnpnhqvls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258888.top/gtqvulqylt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtkuagkjtj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtdvlcoihr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtrypkndyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtxxdqkobe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtmzqqbjpq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gticdxynii.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtdpwounfg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtmzygpnbh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtjzofvurv.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtwvyzcpev.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gttwahswdi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtboojqahg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xinyue.icu/gtsbyfddlj.html

Ruby: Dir.children("dir")
来源：http://hz.chenjidiqi.icu/gtglultjge.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gtfodvgdkz.html

[F09] 获取文件大小
来源：http://hz.xinyue.icu/gtuucbsdah.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gotoacloud.top/gtguerwzwg.html

PHP:  filesize("a.txt");
来源：http://hz.sxryk.cn/gtywwiikkt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtdokiitnz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtbnnzcpbl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtqbqgiyek.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtrqkqzzpu.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtwjeidyai.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtlmhqkkfu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtqjjhyiqc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtxjmscdmn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtsrxbvhbe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtaieiywdv.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtrlasbvzd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258.top/gtmaexauph.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhengqikj.top/gtsgcwkbeb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtwettbmah.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtopntcoht.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangkeji.top/gtgclfstbh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtlzbravkf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.mhx1999.top/gtxbpgzmmj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtiitjelci.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gttcybdjdv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.havefunace.top/gtmvdbllpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtloskflaq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtpwubnesb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.vqdsnc.cn/gtxgemtscr.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gtfdxhasyo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gteiomwpeg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cdnleiting.top/gtlelxnjfv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtutpcfggn.html

TS:   // 同上
来源：http://hz.xylfe.cn/gteltfczqb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtqvmelprj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtyftjgglt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtjchteqxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtxosioecy.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjkfmebyw.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtvzarxnpw.html

================================================================================
来源：http://hz.yj20258888.top/gtvlbtgudq.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtunzowfml.html

Py:   class User: pass
来源：http://hz.xuanzx.com/gthilhkhbx.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gthdknkhzr.html

JS:   class User {}
来源：http://hz.cheryme.top/gtgnnvknlm.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtihsjcplc.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtwntxfqmj.html

Go:   type User struct { Name string }
来源：http://hz.zhongyouzk.top/gtwyhdswub.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtmsfaeraq.html

C#:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtynjnkqeu.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtmazuqngn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtwoycoqfi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gtwbjqcclh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtmfvfxrfu.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtkhwkgfin.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtkonodcca.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtbuhajhsy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtquwabpzb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtuopryjza.html

[G03] 实例属性
来源：http://hz.dianchejie.cn/gtfktifgkm.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtbyiandbe.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtbmsvxbqh.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtolvmmcpc.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtfwnysmod.html

Java: private String name;
来源：http://hz.yj20258.top/gtoccahpqf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtldepnixd.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gtaoinjnkr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tian-w.cn/gtqrxfghfu.html

[G04] 定义方法
来源：http://hz.sweek.top/gtbzyhcgax.html

Py:   def greet(self): return self.name
来源：http://hz.jianghu66.top/gtuokuuhlq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtobxzhgzy.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtthislaje.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtapkejarl.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtvnzwvykd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtgusvcejq.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gttpfuolpi.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtyswegmgi.html

[G05] 继承
来源：http://hz.andypj.xyz/gtrdydzzwg.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtqxzfruof.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtplwbtpvb.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtxmovrsnn.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gthxamxpwg.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtrxusmrgc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xingfuxueyuan.xyz/gtmrarzrji.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtzzcailaf.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtrjvlrrxm.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtjhdrondy.html

Py:   def greet(self): return "admin"
来源：http://hz.zhiwuduotai.top/gtlofhbxrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtezxztuio.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtcvwckeis.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gttnqwvsuk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtdajuqkuv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtkgbpgjvl.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtvseujswg.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtnzpchnks.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtznmdosqi.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtphfnpybb.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtzqnispse.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtzzarslyt.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtjqgaidwp.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtkfsmzwfz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtgifigigf.html

Ruby: super
来源：http://hz.ydzc1.top/gtuzqdoreu.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gthvhgzynx.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtoajdvhwx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gttegklgqr.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtnuttlcio.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtynjfrtkf.html

TS:   static f(): void {}
来源：http://hz.bjfxy.top/gtuurvjhdc.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtslijnnzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guowangkeji.top/gtnzxijyjb.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtgescvutx.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtgffxvjwl.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gtlircjmhm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtlvfivmqs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtuicsuuil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtdpcejcam.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtkolfatzf.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtljdmgltq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtkwtuefno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtrbpkdaak.html

C#:   interface IShape { double Area(); }
来源：http://hz.nanxinkj.top/gtahknacqg.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtvmccdtul.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gthpynsskn.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtwntmbfwy.html

JS:   #private 字段；其余公开
来源：http://hz.chenjidiqi.icu/gtpodvtpew.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gttoirlyez.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtcyrjyybe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenjidiqi.icu/gthtewfeml.html

Ruby: public / protected / private
来源：http://hz.ybcxt.top/gtepqtwpnm.html

C#:   public / protected / private / internal
来源：http://hz.snrcjt.cn/gtngvojkcu.html

[G11] getter / setter
来源：http://hz.yangfankeji.com/gtgxxeuytr.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtnbiqbcji.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gttijsliox.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gthtnphccd.html

TS:   get name(): string { return this._name; }
来源：http://hz.hysaishi.cn/gtoxlosono.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtnpxwwehh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtofofyjui.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtptmowicf.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtbnodrnog.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtfdxgfspp.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtgqazbgwd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtvyfcshfa.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtvofdyaju.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gthworuane.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtjjibhcwn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.9152youxi.cn/gtcvqqqkiq.html

Ruby: def to_s; @name; end
来源：http://hz.tian-w.cn/gtfhcdqqwc.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtqqdlyhjl.html

[G13] 判断对象类型
来源：http://hz.feifeiyinyue.top/gthmdhzstu.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtdwodzamp.html

PHP:  $u instanceof User
来源：http://hz.0kj1m.cn/gtfbitybol.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtftljcwbq.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtrynoerhx.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtmxppdlmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtysarusag.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtaonhftdl.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtpqjpvrny.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtozrgxcls.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hywenlv.cn/gtwtdgecuk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtzxbzhnhm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtxuaixvow.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtgvjyxdxb.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtqsksixly.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtymyngpbm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtcjarlkmi.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtjqpegiib.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtznrakvfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtpbembmlr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenzaomai.com/gtbcsqxiim.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtdflhlezy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtewsdpfks.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtubknhovx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtcdltpprz.html


<!-- 参考信息 -->