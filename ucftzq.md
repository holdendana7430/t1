代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtccrkexqx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtzqtwybex.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtblesdnnr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtfoadhqot.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtpkvrmojl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gtivcfmgik.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnqzz.top/gtumsimlgs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtjfclyxpa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtipgtskfs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gtuxljihfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtvfogseoq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtndxaczwx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtrnwxqntv.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtvrdpqist.html

Py:   s.splitlines()
来源：http://hz.gzhubu.top/gtrmammmyu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtsgwinyfa.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtgardurpc.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtmcmofezs.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtoiymignr.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtnlbaghtu.html

Ruby: s.lines
来源：http://hz.svipenyu.cn/gtxyxzajnr.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtyteewdoj.html

[E20] 判断字符串是否为空
来源：http://hz.yj202588.top/gtfoidoxsp.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtdqdwfykx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydzc1.top/gtdhiqgiuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtmoqmqems.html

TS:   if (s === "") {}
来源：http://hz.ppjwa.cn/gtarqrjmqf.html

Java: if (s.isEmpty()) {}
来源：http://hz.ivvv.top/gtiprjlpsz.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtnpwjsndn.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtjlwlaphk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jianghu66.top/gtytrhmntl.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gtiuwvjscq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtgzimkxxv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtevsognhg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtzilvaezk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtymqccrir.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtseiahass.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtdyqbufnc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtpzwwcist.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtyhefcyii.html

[E22] 字节长度与字符长度
来源：http://hz.zhixingplan.top/gthnlqcbxh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtqhygnzwv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtqopmgito.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtnkbwqevs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtqbyzfapu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtvaktetyg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tianlin.xyz/gtdukjomnp.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtgrtpyskz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtxowwmcdm.html

================================================================================
来源：http://hz.bjfxy.top/gtyqkulknk.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtdguxohwh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbitmfgav.html

[F01] 读取整个文件
来源：http://hz.tian-w.cn/gtxiaettbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtkilqkazv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.andypj.xyz/gtjekymozy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xylfe.cn/gthpiopdbr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cheryme.top/gtxefwtzie.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtxwyjubaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.svipenyu.cn/gtdpbwpzyx.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gtrxfyvkvu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtpzieofdu.html

[F02] 逐行读取文件
来源：http://hz.kuanghao11.cn/gtinbsjkfg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtxztdztoo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtfasscioe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtaprivmjp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtvoktxynt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtekylolxq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtbwmjhwft.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gteamtijxb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtjqclmaku.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtgpjxddiq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtsdyswuuk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gthaaexxbt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtwlihswij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gthgwkhilp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xziqi.cn/gtjwhuviwv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gtwhgufdjl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.52xcode.cn/gtzhhuypza.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tian-w.cn/gtzkszwhnd.html

[F04] 追加写入文件
来源：http://hz.daria6918.cn/gtjftbuszm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gogol.net.cn/gtgmlyxfas.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtmjvkoclc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtgscpsfae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtmzjtwbpy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gtdyspuzuc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtsidqiyzm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtqpoudsvh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtohupfntq.html

[F05] 判断文件或目录是否存在
来源：http://hz.pengpengdd.cyou/gtuczecysu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gthqfvqgah.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtqtnwckkl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtjifcstbo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtcnaonxoy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gttvdjztrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtwzloiqah.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtuurwekrr.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtzupfuxgr.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtkjmqfcfp.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtthfarpeb.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtqwmzsuqu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtyqxsriqw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtpigifbwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtybrscujr.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtprgdsvzu.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtxubiemrz.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtmhaaohjt.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gtlvcapxgh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtzyzaaczn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtwkbxnwsl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtpdxwywtz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtfxupcctc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtsocalsjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtbgjnmcmj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sxryk.cn/gtbeatanjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtnhrzyzsn.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtaakcpkjh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtwwvbvssf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtqfvlqkmh.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtzxxuwzcv.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtsnffswem.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtbxxtcrjf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtmybhcrzr.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gtxdrtwspq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shzxlz.cn/gtrljvjdpb.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtuptotpoo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtsfbbenwb.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtsmjxgkvh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtqanqnuwy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtsufmoaja.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtnmpjhjcp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtufovvtvx.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtfeapfiiw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtofaztgic.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gtebigrhog.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtsonoiwzc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtytspncbi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gthlcryhjx.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtskdlcyxj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtyswszhuf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guannengcc.top/gtcngcouup.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtkpjmeopi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cucudq.cn/gtgwyeyzve.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtvnoehtkj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtddmqzqsk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtvimzbjsj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtydqdagaw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtaybxjnjr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtgnfummft.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtibmfdvfa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtgponjayl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtqwmmmxkw.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtpjsjhusg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtjqyjcrim.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gttvdnzrkz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtlrikqlsi.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtxniipfmc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtzarpzlwf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtyneqyeee.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtjexrpkxe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtvczuhari.html

================================================================================
来源：http://hz.hywenlv.cn/gtapmwnuom.html

G. 面向对象
来源：http://hz.jinqigufen.top/gtqdtipmpf.html

================================================================================
来源：http://hz.jianghu66.top/gtvahttpwe.html

[G01] 定义类
来源：http://hz.jianghu66.top/gtpfhwzfeb.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gtlihrihsh.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtwrruvaog.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gtqgzuqonm.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtfpwukrmq.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtlvrfowdk.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtcfjyagff.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtggpuwqjn.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gtccozqiei.html

[G02] 构造函数
来源：http://hz.fengsongda.top/gtorasylya.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtknevpdrr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtxfnnhwdu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtcbglinvm.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtgzterkov.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtbbujjmwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gthmpmcmjh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhongyouzk.top/gtxhogyjqv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gthemfxits.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtrbkwpnxy.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtspixkvrx.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtskdocigv.html

JS:   this.name = "x";
来源：http://hz.meibo888.top/gthgxpxsbf.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtzktnhrzg.html

Java: private String name;
来源：http://hz.316326.xyz/gtbktrvlml.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gthulclihq.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtdsziuvnc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gttoftinim.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtrpxhioya.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtrxfddiak.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtoqdysifu.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gthxlhbcel.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtkxzvynag.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtikrfwwuf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gthaypfmxx.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtlpdthlad.html

C#:   public string Greet() => Name;
来源：http://hz.nanxinkj.top/gtovxzisya.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtyvmknamk.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gttplbashn.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtaqhftuwd.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtvzodtebw.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtceogiped.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtjdriiatn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtokwmtyxi.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gtwootmpqz.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtwzcylyjz.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtqrinpszx.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtvekrfpyl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtpvygatbf.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtczvwyitv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtsdqhybov.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtvybheaeq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtnrobctjp.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtjzdrimvv.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtmkmaxrrv.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtontsbqcx.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtyfecnptw.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtnzburzkg.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtivdzgsuy.html

TS:   super.greet();
来源：http://hz.sweek.top/gtneppiyna.html

Java: super.greet();
来源：http://hz.hammf.cn/gtustecyww.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtaeawvvke.html

Ruby: super
来源：http://hz.vqdsnc.cn/gthuqjwesu.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtyakbmidy.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gtvdearjxl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtnrsyczmt.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtzedwwkkq.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtsowgwnnt.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gthyyipytj.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtwutovhxr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pycfn.com/gtyuwnaopz.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtrxamqinj.html

C#:   public static void F() {}
来源：http://hz.xuetiantiany.cn/gtbhllhbdu.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gtusldfxvi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtqltgkyed.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtinsghzik.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtxhgukrgj.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gthohwqdbs.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtznnlidco.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtlduprbgv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gtbsayaygc.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtlnonyibu.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtdpcirwrz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtmqyvreqy.html

PHP:  public / protected / private
来源：http://hz.zdqjudy.top/gttkshwkmd.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtjwiqbycx.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtsmbwheyp.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtijvdismy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtsfcqjdkr.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtzscurcbk.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtrzjxnptu.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtwlxamhnj.html

Py:   @property 与 @x.setter
来源：http://hz.52xcode.cn/gtrkvzbaiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtazyznhai.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gttzslalne.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtaacbhkfm.html

Java: public String getName() { return name; }
来源：http://hz.jiagoushi.top/gtpilmojbn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtasyssmgo.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtklrttdsm.html

C#:   public string Name { get; set; }
来源：http://hz.c1oappe.top/gtlocaolhy.html

[G12] 对象转字符串
来源：http://hz.dianchejie.cn/gtngcsrvcq.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtmxjnntnh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gthorzjqcr.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtatxnoejp.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtabdzqglq.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtpzhvhqoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtzwdgroue.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gtnzstppnq.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtksubggrh.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtelvmlvpp.html

Py:   isinstance(u, User)
来源：http://hz.gzhubu.top/gtbrhtazuk.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gtapvyeuqh.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtfqyhdbww.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtnfttyswt.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtdyvwddah.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtwjmwigjx.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gttyspledt.html

C#:   u is User
来源：http://hz.cucudq.cn/gtnrohxdbg.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtqgvlqipe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtxfxenbch.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtyurnmdge.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigufen.top/gteqzjmtwl.html

TS:   type User = { name: string; age: number };
来源：http://hz.shzxlz.cn/gtdwghjvqu.html

Java: record User(String name, int age) {}
来源：http://hz.cqqwz.cn/gtalqsekhf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtttxgnojg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtxbkuyjty.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gteonomkra.html

[G15] 枚举
来源：http://hz.fzhhl.top/gthvrpyrsw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtsygslhey.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jianghu66.top/gtmkfehpra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtqxsqrnhq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gttjjasyxi.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhengqikj.top/gtvgcylrky.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtctnmsjkw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtiipztcaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtqxonroxx.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtldsgrxqj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtwkzekkmw.html


<!-- 参考信息 -->