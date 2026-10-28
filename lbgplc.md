代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtjmdmpsna.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtipldxsmj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtaojkqdnj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jianghu66.top/gtklpjvqsr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gthbeuurym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gthpvzzxhe.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxuanxn.top/gtfncemins.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtmejgqdwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgfzy.top/gtdnuzbycs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.mhx1999.top/gtvspuzecl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtxwhegxlw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtgukotmre.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtlzpnouxk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtcsiwebxe.html

Ruby: s.capitalize
来源：http://hz.jinqigfzy.top/gtomqbzyxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtydaphtib.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtrgrignay.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtzpudvhth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gthnpkooof.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtmsigvtgw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtyrtepwqd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ivvv.top/gtcrqbmnud.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtymabgcju.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtgvkfvsvs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gtgkwmdmzd.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtxviqrcia.html

Py:   s.splitlines()
来源：http://hz.daxiang520.top/gtectgsiaq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtwcsxcout.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtnzhdvkex.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtooaefmjm.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtncginyec.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtahfnhdcf.html

Ruby: s.lines
来源：http://hz.tian-w.cn/gtrecepyzb.html

C#:   s.Split('\n')
来源：http://hz.sxryk.cn/gtykkonpit.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtjoywlujy.html

Py:   if not s:
来源：http://hz.daria6918.cn/gtkrkdywzi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenjidiqi.icu/gtczgywzte.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258888.top/gtnhdsjkma.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtrmkreuey.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtpwxvreou.html

Go:   if s == "" {}
来源：http://hz.zdqjudy.top/gtpgzkomaa.html

Ruby: if s.empty?
来源：http://hz.haohaochexian.top/gtyeiwvcle.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhongyouzk.top/gtygpkyfnm.html

[E21] 超长截断加省略号
来源：http://hz.jinqigfzy.top/gtssvqynum.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtfrvlshnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtsupywdkz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtyyqepvbl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtlgrrnnla.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtduiuveuq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtlbiixubb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtzjkvftoc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtylmrpanr.html

[E22] 字节长度与字符长度
来源：http://hz.316326.xyz/gtaykvgqak.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtzzogxdxq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtnbmzzefi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtublmjhwl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtfdfyehrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zycfv.cn/gtkfjxsclb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gogol.net.cn/gtdvbwybvu.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtqlkajgrz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtwstoqyvy.html

================================================================================
来源：http://hz.yanxiufei.cn/gtwhbbsukv.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtcfwtsssv.html

================================================================================
来源：http://hz.daxiang520.top/gtlulrtuet.html

[F01] 读取整个文件
来源：http://hz.sweek.top/gtsnprfsip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtfishsfoe.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dashuyun.cn/gtpdcopjpu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.52xcode.cn/gthxihgvkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daria6918.cn/gtegsjkfth.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtocdojydi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtdlkugdyk.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtrbsapmty.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gthcqyhhcd.html

[F02] 逐行读取文件
来源：http://hz.yj20258.top/gtoyxbztil.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtkdlqrsvx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtwaabgwpm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtdnnborqi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtgyrnnjic.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtunjpdtbd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtttrjwicf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtnaihheqp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gtmszjgsfj.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gtvcsamohk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtlubwrssg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtobkqbbzz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtwctbvmzi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtvoremtum.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtzxkxwwfj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtyveijvws.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtwudiochx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtespgpffy.html

[F04] 追加写入文件
来源：http://hz.jqgufenzy.top/gtqlvfmvtt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtllikwayl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtnivadcbn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtgusqyigl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtakygrauo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hfpthk.cn/gthmmgkxez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtujjxehya.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtystzihuq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guowangkeji.top/gtrxeokhye.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtpodphvqf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gttpfalfdb.html

PHP:  file_exists("a.txt");
来源：http://hz.tian-w.cn/gtumajgwre.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtiwgjzcfi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtaegriufs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtgaeuqmco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hongshengwenyu.top/gtlynrgxur.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtbxbyiwzr.html

C#:   File.Exists("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtinwescdb.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtplerfisi.html

Py:   os.remove("a.txt")
来源：http://hz.xylfe.cn/gtlcbexfxu.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtmmhweotd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtvtvomeck.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtrbujyxxa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtyjujlqlf.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtdwdnclpf.html

Ruby: File.delete("a.txt")
来源：http://hz.ydzc1.top/gtymsnulkz.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtjbsmmffs.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtxxgbfnhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangdashe.top/gtkhpsilcj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtcztmwnzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gttadoqlux.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtzwpncfpp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gthbhhluxh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtraeysyvj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenzaomai.com/gtuvbxnqdq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtebvkxwka.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtddkczycw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtveqxutwq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shzxlz.cn/gtcwlftelp.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtamzaarms.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtjlqzfabt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtbejuimsb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xinyue.icu/gttohfnbxb.html

Ruby: Dir.children("dir")
来源：http://hz.yangfankeji.com/gtesqqaeew.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtzirkjhbr.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtzuesygar.html

Py:   os.path.getsize("a.txt")
来源：http://hz.mhx1999.top/gttnndovnp.html

PHP:  filesize("a.txt");
来源：http://hz.zhengqikj.top/gtpedyyjyi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtogctuejk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtaazxxtol.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtwuvzmwkb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtbxvujjyh.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtuyyplmma.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtoiqznbax.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtnkpbwndf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtennsblty.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtdbulsotb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtdessfnnk.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtuckqqmhk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yangfankeji.com/gtgfrkrhsn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtjztyylhw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtshifinaz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtqtcgqfku.html

[F11] 复制与移动文件
来源：http://hz.jinghuilouyu.cn/gtfucxdenb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtoqjdavdv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtfhwvidmg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtwgjghetp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtxljnunxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtpeiupmdu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtxacszlqm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gthzuznxbg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtezhzvnhh.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtzjjhzjat.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtmlcduzzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhiwuduotai.top/gtqispubcv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtvammjarc.html

TS:   // 同上
来源：http://hz.zhiwuduotai.top/gtietpczmk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtjrqtahnc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtamddcdpx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtndfdigik.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zycfv.cn/gtuzsponjg.html

================================================================================
来源：http://hz.cdnleiting.top/gtxixiqiyy.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtypmdhsch.html

================================================================================
来源：http://hz.cqqwz.cn/gttfewvirl.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gtbdtttwzg.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gtrgdznbqb.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtiihlcxah.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gthlkixzds.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gttqporglu.html

Java: class User {}
来源：http://hz.nwbrower.top/gtpibmhnjb.html

Go:   type User struct { Name string }
来源：http://hz.hongshengwenyu.top/gtfqplxjje.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtpggchqzr.html

C#:   class User {}
来源：http://hz.aibaodan.cn/gtjdlvtono.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gthmewrrbv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtpnguirtu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtpgohjxrg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gthwhoeycg.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtmytfxyxi.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtxoltsdah.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xziqi.cn/gtahmngaqz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gttkokddvg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sxryk.cn/gtwhoflvjq.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtocvqkqqt.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtoimcyfqn.html

PHP:  public string $name = "x";
来源：http://hz.haohaochexian.top/gtrdialpgu.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gtxyqpspul.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gtyeorszta.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtwieokeyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtqsgidezk.html

Ruby: @name = "x"
来源：http://hz.iojbl.cn/gtyiolyqrn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtqbfeqyot.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtlcmllwde.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtuhqpgyim.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtqbbovtyh.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtfrneczri.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtqqxksjdo.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtcstpuywd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtsjsovyad.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtlidsxncb.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtgnthnmmy.html

[G05] 继承
来源：http://hz.smart0.xyz/gtwzdydwbx.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtdpjlwskm.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtnjslogdo.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtgtnbfuen.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtboezybrt.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtnyiclygd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtpseqnkcg.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtjeelluwh.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtsnpgazpx.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gttphcwiqi.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtklahuqcz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtxsrxoncn.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtvyisggwd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtrqjbwrym.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtwunkhqlt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinghuilouyu.cn/gtpfimrplh.html

Ruby: def greet; "admin"; end
来源：http://hz.jianghu66.top/gtpquuobqw.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangshuangyany.cn/gtmhpcybwi.html

[G07] 调用父类方法
来源：http://hz.wangdashe.top/gtjjnzbcji.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtjofofkem.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtrndbdokf.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtomiwqdxu.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gtwmmgckzr.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtslwwoydd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtfmferkbd.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtzeqhjdlw.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gthycinzjq.html

[G08] 静态方法与属性
来源：http://hz.yj20258.top/gtaxqpnpqt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtckoasudt.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtnasdhdbu.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtpgimdifh.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtmjbmdswl.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtcdgasxta.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gtlfuebelq.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtyhngxnbm.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtehhaombh.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtddfamlwd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.vqdsnc.cn/gtofcitwwc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtywavuege.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuxming.cn/gtejxaryny.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtyyxxxrmj.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtecxbkkiz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xziqi.cn/gtczudjdgp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.feifeiyinyue.top/gtooqcipna.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtkcncccez.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gtbkzdyykb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtalqndgjq.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtvbfnjhlv.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtrxjtjuro.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtnbwyxjcy.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangkeji.top/gtnasgjnet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sxryk.cn/gtildrtkks.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtunzvnxqy.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtzzjfwdil.html

[G11] getter / setter
来源：http://hz.sufxvd.cn/gtbhhhelxa.html

Py:   @property 与 @x.setter
来源：http://hz.zhoulong.xyz/gtwlywcysm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtofxheurs.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtzherxlyd.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtcxswermq.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtonhgipfe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtsdtlyjgn.html

Ruby: attr_accessor :name
来源：http://hz.fengsongda.top/gtikpyqzyy.html

C#:   public string Name { get; set; }
来源：http://hz.dianchejie.cn/gtwemcimlu.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtuhgbhhxg.html

Py:   def __str__(self): return self.name
来源：http://hz.wangdashe.top/gtfuceuplu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtnrxnyiek.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtsrnhyybo.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtrfrubsir.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gttrcklvcm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtcmpyxbct.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtiwvweszm.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gttznpiyvr.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtqjzqchnz.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtvjfoossc.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gtfrygnrct.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtiyeyentc.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtnreyntfi.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtmfsolyux.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gtzjfcvryj.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtsugppaav.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtwrcfepei.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtmbpqdreh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jianghu66.top/gtguxyatsx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258888.top/gtrgcusiih.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtddmqbbsu.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtgogqebuw.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtmfwscfwh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtlxeprpzx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtepsqhhpx.html


<!-- 参考信息 -->