代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.vqdsnc.cn/gtgjijnzqe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhijiandao.cn/gttljafgjp.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gtfmpnuplm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sxryk.cn/gtkrsbcjxj.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtweluxlmr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtgjoyesto.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gthabmhtgx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtkioyxylt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtbqierbmd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hfpthk.cn/gttrpowcnz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hongshengwenyu.top/gtexelofyi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtvnwrojps.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtufxfezzg.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtouwrvmyp.html

Py:   s.splitlines()
来源：http://hz.havefunace.top/gtyrfgtdxs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yangfankeji.com/gtbuyufwvh.html

JS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtqnpjmpjs.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtwwjwptcb.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtyaaugfpq.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtovqbkryc.html

Ruby: s.lines
来源：http://hz.jinqigfzy.top/gtppmajtxz.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtrcvmqjyl.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gtsoabomzj.html

Py:   if not s:
来源：http://hz.ydjk.org.cn/gtknukxuqo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtpzenujmj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258.top/gtdwstydzn.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gttjqujvqg.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtshztjklv.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtzoouxblq.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtfwntdbva.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtwxpstcjj.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gtisirheio.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtjjhqbxih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtrohwrmqv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtnfmnghao.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gttxglkxtt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtywmjoeqh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pycfn.com/gtfhekuhia.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtctjygzto.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtjvgduqrs.html

[E22] 字节长度与字符长度
来源：http://hz.cheryme.top/gtyycbsxfb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtbutyyuas.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtbzdqgvmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtqzkkaafa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtijzgzuea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtzltkryuw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtzuxyvfaz.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtjssavqgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtprjvdkgf.html

================================================================================
来源：http://hz.sweek.top/gtbzdkrnda.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtpngcsazt.html

================================================================================
来源：http://hz.yj20258888.top/gtvqfnvbnj.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtdokttpcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtindydyuz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtncesbzbx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pycfn.com/gttoedcjkq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dianchejie.cn/gtzmjrbkiz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtflmesdkt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtldxzozkz.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigufen.top/gtydbhheyr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtcpzeahjq.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtjjqknhuf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtrwpejqxi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtqeyixwsw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtjwlccqcp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtnqvlyyxe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtsgfqwlsi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gttsoqkluv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtwktvlyil.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtorgvepcu.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtfixhysen.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gtmpfqctqa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gtelbdanis.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtbpxrsvdx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtspuqqodh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhengqikj.top/gtbcyvhsbl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtwxatslhl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtsgdmgcfa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtfjivbfgp.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gtrntrzzpw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtixrtcgsa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guowangkeji.top/gtaafglkry.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtmxshbrog.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtkkaomysy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtreerbbrr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtrykdsqrz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenjidiqi.icu/gtcglwdffd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gttmaxlspa.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtnapntucy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtyfxybaul.html

PHP:  file_exists("a.txt");
来源：http://hz.shzxlz.cn/gtveqxvqga.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtqisnqmwr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtomqvbxik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtsmqpmghx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtqgpjbzbc.html

Ruby: File.exist?("a.txt")
来源：http://hz.redwolf501.top/gtmqpdbbjh.html

C#:   File.Exists("a.txt")
来源：http://hz.aibaodan.cn/gtoqehjhod.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtnekoidrk.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtavwafhxy.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtdjrocnhx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtffopvbsi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtetfixypo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtgdibijjn.html

Go:   os.Remove("a.txt")
来源：http://hz.9152youxi.cn/gtmgotkglm.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gttscseukt.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtieiqbcvu.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtzuunsimk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtcrljafvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daria6918.cn/gtjqrapuhg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtkeaejcyp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtedutbgnu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhengqikj.top/gtlifjqbsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtsikotbst.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtnpntotee.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtosycsxfi.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtgfpgcjgc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtguaysiks.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtbjcgthse.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtrakhbuam.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtvgdtdazs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtaoptxcko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtemsqswku.html

Ruby: Dir.children("dir")
来源：http://hz.sxryk.cn/gtlsaaznwf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gtvgqmfugg.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtcwgqswoz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangshuangyany.cn/gthpzuhzxu.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtpjwbxqke.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtrlqfombc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtagamekma.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtfavxrmhd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtjxgxvkug.html

Ruby: File.size("a.txt")
来源：http://hz.gotoacloud.top/gttvafphsc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtvgrimnwd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtisbwfigi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtdcqwqnaz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtuksghdgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtmeqfckkx.html

TS:   path.extname("a.txt")
来源：http://hz.fzhhl.top/gtupcofurc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtwtfuejtx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtiakgskvp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtcxjxiacl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gthawoctdk.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtgcazguwu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtjsezbpmv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gthvcjhnjj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtvujeztsb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gttdrbxgwf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gttmxiddtj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtvpqwwvme.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gttauxldvx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtkpefvxib.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtylvxersx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtprgbouxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gthftsenqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtjnkklbjt.html

TS:   // 同上
来源：http://hz.sweek.top/gtwiaerxqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtziwhmbiv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.quarkkingdee.top/gtjxnwzrns.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gtnpmtqqku.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.kuanghao11.cn/gtggolhtoy.html

================================================================================
来源：http://hz.xuanzx.com/gtdyudrekg.html

G. 面向对象
来源：http://hz.mhx1999.top/gtgduyvyqz.html

================================================================================
来源：http://hz.bjfxy.top/gtsvcvrfip.html

[G01] 定义类
来源：http://hz.tianlin.xyz/gtuwjlbgor.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gttshwipdu.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtwiatyfrj.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtdxsetqzr.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtyoyomlvb.html

Java: class User {}
来源：http://hz.cashguo.top/gtqyhiguqz.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtdnwiqbpg.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtuhsvfudu.html

C#:   class User {}
来源：http://hz.shanyushiyangtech.top/gtfhqknlye.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtrfpfwyfd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hywenlv.cn/gtkdnlzuay.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtjismmict.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuanzx.com/gtbxdgfmlr.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtowmzisfz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtjjsixiop.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtdaztwgvw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sweek.top/gtspwygckg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ehwqpu.com/gtymlxxemp.html

[G03] 实例属性
来源：http://hz.nwbrower.top/gtbqpnsyjk.html

Py:   self.name = "x"
来源：http://hz.yueranfly.top/gtknuswtld.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtzqypzywu.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtiwswcmyh.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtttpztdvr.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtdneagphy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tian-w.cn/gtwporbfxc.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtgpsxkegy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtfgodipmd.html

[G04] 定义方法
来源：http://hz.cashguo.top/gthsexcwmp.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtfwcgapri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtimixcwmg.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtrzdtokth.html

TS:   greet(): string { return this.name; }
来源：http://hz.aizwys.cn/gtjqnytfii.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtmganlvws.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtarcycyys.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtxfyryffs.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtuefbxttn.html

[G05] 继承
来源：http://hz.yuanzhike.top/gtgwplxvud.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtavzvckyj.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtiylecyol.html

JS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtpiarczxe.html

TS:   class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtelgmnkvu.html

Java: class Admin extends User {}
来源：http://hz.shuidangran.top/gtufigcxtu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtmizczpui.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtpvxppzww.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gthmehkclm.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtmtjlownx.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gthpgrwecm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtkkszwdox.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtcerzzknx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gttkvbmrfo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtuzteivdu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuetiantiany.cn/gthcvcbmbo.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtyygztgha.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtwukzcuzg.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtodudytvt.html

Py:   super().greet()
来源：http://hz.zhixingplan.top/gtcwdvyjrp.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtbkzncryu.html

JS:   super.greet();
来源：http://hz.yanxiufei.cn/gtcgyisfwh.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtbroezhwz.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtzlstcnfa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtxdzbcgif.html

Ruby: super
来源：http://hz.jinqigfzy.top/gteqlwvdxk.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtruvbuhrw.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtnlpnmbnw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gttijfgmyw.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gtqyglgrbd.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtpyuskiud.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtlvechxfh.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gtgudjbxps.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtdgrxqktg.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtwbdrbvar.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtsdwwnyru.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gtavlfkwbd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yvedp.cn/gtferivxsh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258888.top/gtlzcpeinx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gteclgkdgx.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtdqxlbywe.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gttzrjmpsk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gttzstewfg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtqtuismwp.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtexjztusg.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtxpeerkgi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtieinbjju.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtxuphdaom.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtokbayhcu.html

TS:   public / protected / private
来源：http://hz.yonumen.top/gtfxvulvye.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtlbzsbuzy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenlongwang.top/gttjzsqdvc.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtwikzntbo.html

C#:   public / protected / private / internal
来源：http://hz.zhengqikj.top/gtczyagfmq.html

[G11] getter / setter
来源：http://hz.sweek.top/gtcwhvgrvd.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtaayxdbfx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtnpshnoeu.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258.top/gtodiowlno.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhongyouzk.top/gtuvwjdoeg.html

Java: public String getName() { return name; }
来源：http://hz.hongshengwenyu.top/gtqrjocdmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuanzx.com/gtkchrucye.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtlxdimtws.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtixatuafw.html

[G12] 对象转字符串
来源：http://hz.kuanghao11.cn/gtjbsjgumu.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gttfhmuiao.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gthbaoncqf.html

JS:   toString() { return this.name; }
来源：http://hz.haohaochexian.top/gtohcqjunq.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtzvoqsfky.html

Java: @Override public String toString() { return name; }
来源：http://hz.cqqwz.cn/gtjhrycvcv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtsktdmcme.html

Ruby: def to_s; @name; end
来源：http://hz.yanxiufei.cn/gtzscgixtm.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtbkbccija.html

[G13] 判断对象类型
来源：http://hz.dashuyun.cn/gtiupuxtif.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtewdcfucy.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtyxezoonp.html

JS:   u instanceof User
来源：http://hz.yj202588.top/gtkyhuxxks.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gtvgjtptls.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtkdyazeua.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtkediepys.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtxrvcuots.html

C#:   u is User
来源：http://hz.dashuyun.cn/gtxrmxfprx.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtsxcjxfcr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtfljbsssr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtwrqroddw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hfpthk.cn/gtripjxqyi.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtgwicktik.html

Java: record User(String name, int age) {}
来源：http://hz.sufxvd.cn/gtuolgkyhw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtqctuwxev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtrrwpkkdo.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtczjtixkd.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtvywempjk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtkfmwbvpl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtpdshbqip.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gthfltulpg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtrxsxtvon.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtqvjtnvoe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtrfjobjyd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gteyeveioe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtrdesrlmr.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gtfkrnyqcb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtxmdnsgjh.html


<!-- 参考信息 -->