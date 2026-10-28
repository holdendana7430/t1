代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtkoshsold.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtclknlqjc.html

Ruby: s.capitalize
来源：http://hz.c1oappe.top/gtrpcuszll.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.andypj.xyz/gtmydfshhv.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtpyxqlrgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtuhvwmrei.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtedqlhnbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtrwhdsbeo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gthpufuotl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhoulong.xyz/gtwsyjtnbu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtridarrfp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtdjyksoui.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gtqimtuaap.html

[E19] 多行文本按行拆分
来源：http://hz.xuetiantiany.cn/gttyizndrl.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtqlytmhan.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daria6918.cn/gtslarvpqf.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtxwafltjv.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtzjbfxyzu.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtvxutlumo.html

Go:   strings.Split(s, "\n")
来源：http://hz.gotoacloud.top/gtdrvdwwoc.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtxnjqqfyw.html

C#:   s.Split('\n')
来源：http://hz.yongpay.top/gtrqjxobpt.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtsdqhlbeq.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtetegizwc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.smart0.xyz/gtaojqiasu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtxyirprvu.html

TS:   if (s === "") {}
来源：http://hz.aizwys.cn/gtaxuobqdt.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtqyrksyws.html

Go:   if s == "" {}
来源：http://hz.hongshengwenyu.top/gtsshusnpn.html

Ruby: if s.empty?
来源：http://hz.chenjidiqi.icu/gtaqkfhcmd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtwhfqnmcz.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtjxypkjij.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtxrtsuodf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtlvveuzap.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtbxsluste.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtxwrubrcs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtmddlxcuo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gttoycgrjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shzxlz.cn/gtzvktxdyq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtgreoyphv.html

[E22] 字节长度与字符长度
来源：http://hz.xingfuxueyuan.xyz/gtrelttqrs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtkwgspdpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtkjuowins.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gthgugqhar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtxsklcfuu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtxsehhveh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gteagtypuk.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258888.top/gtlrogwpqu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tian-w.cn/gttvvepgaz.html

================================================================================
来源：http://hz.haohaochexian.top/gtkyzrkeef.html

F. 文件与目录
来源：http://hz.sysykeji.top/gtzvmzqguo.html

================================================================================
来源：http://hz.fengsongda.top/gtsmxeuvnj.html

[F01] 读取整个文件
来源：http://hz.yvedp.cn/gtghareylb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gttytybhbq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtxirosvcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtnzvoauph.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtlzxjmfli.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtnrutdxei.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tian-w.cn/gthfohejzj.html

Ruby: File.read("a.txt")
来源：http://hz.xylfe.cn/gtsfboxbth.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtyhggnjoz.html

[F02] 逐行读取文件
来源：http://hz.xuetiantiany.cn/gtzsnamwkx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gthveqtqet.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtwneamgpg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtnrchwsum.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtiflmwuhh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtzawcskxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtmpkqmpdw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtjdzfxsei.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhaomingkeji.xyz/gtaezgcjbm.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gtlkbuzksr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.redwolf501.top/gtpmswwbdw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtjaijdufc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtlxicelax.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtfswtyocf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gttkbwmmpn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nwbrower.top/gtkpfzhwxx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtfivvcfhb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtxhpzdxqh.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gtmqamiesc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gtukapelvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtxyztiszt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtrrnkllso.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtghtdudpv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtrxamlcof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtuxqiphag.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jiagoushi.top/gthgiuteio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtkajgabik.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtfvprxcya.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtuywqdjzt.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtavnjdwnk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtylqqwqsw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtjpqsivne.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtsllbzuik.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtvcztfspn.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtbtgnxwan.html

C#:   File.Exists("a.txt")
来源：http://hz.yangfankeji.com/gtdwbmwovj.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gtshdftold.html

Py:   os.remove("a.txt")
来源：http://hz.dashuyun.cn/gttoebstdh.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtrdxbsnsj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtoruufkep.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtpkpcbqkf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtuheozfqt.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtewohrses.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtihdjmcsk.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtrtfexqgc.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtizqixues.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtkfackusu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.c1oappe.top/gtxxpzlgqh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtehuultac.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtulpguzcu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.svipenyu.cn/gtiigpdxzw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtvsxmwpic.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxuanxn.top/gtuqjetdzb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtiqiucluv.html

[F08] 遍历目录
来源：http://hz.sweek.top/gtcswhwjzy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtutnhnxpr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtvdhzxlrk.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtoiqfvkju.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtxalhwapx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gthkllndxf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtwkvaefwe.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtvwiqpphj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cucudq.cn/gtnigjsolq.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtsiwpctcm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtsinsulnh.html

PHP:  filesize("a.txt");
来源：http://hz.yuxming.cn/gtxhgharqp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtfhzrlqvu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtzpympbsx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtswxjayhz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtkaejaces.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtlrtjofvd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jianghu66.top/gteetbslwk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtrbpljoku.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtftibqgzs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtbdjefhln.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtmtkznecn.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gttylzdwgm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtkrafruiw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gtkvhaxzoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtyaluexjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtxpdyslmn.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gtuyekzxng.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gthllwhzgh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gtyvxpqqqf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtqcfuiqkq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtlqgrtitf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtfvagnbnd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtqadnpizy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtltcitwwt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtlwphpcvl.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gthgugbtat.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtlqknkbsz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daxiang520.top/gttlvfmjnq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtgbqpaoee.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtrowkattb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangshuangyany.cn/gtptqcuije.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtmmjhuruj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guowangkeji.top/gtksydvkbz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sweek.top/gtwoyoolph.html

================================================================================
来源：http://hz.c1oappe.top/gtqxyxizll.html

G. 面向对象
来源：http://hz.nwbrower.top/gtyicshmid.html

================================================================================
来源：http://hz.sysykeji.top/gtqsujymtz.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtzrydbkrn.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtkbxjkcut.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gtabsebatv.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtnqbrtvsx.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gtzsklbxxn.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtttujfxxs.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtqxvvpbvr.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtrovpktau.html

C#:   class User {}
来源：http://hz.tanke756.top/gtqglahfmh.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtsvfjfycr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtsbrizwgy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtprsmunpz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtrmlwydkv.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtwhitucps.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtaszeeyki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtyfijbkub.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtmhkvfeei.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtbbdwoxma.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtwzxntdwx.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gtfsdxwtjv.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gttxodbxnz.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gtrawlkfoa.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gttamsqery.html

Java: private String name;
来源：http://hz.cashguo.top/gtyyoapghq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtgsbytntb.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtjdopgvfy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtjspwnjrp.html

[G04] 定义方法
来源：http://hz.zycfv.cn/gtpolwohdq.html

Py:   def greet(self): return self.name
来源：http://hz.iojbl.cn/gtuutusqgo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtumtvnzrd.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtdmubcsjc.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtqzjvuijf.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtbzjiurgf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtbpkepcfu.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtenrysfgj.html

C#:   public string Greet() => Name;
来源：http://hz.birdmap.top/gtvehkgzyz.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtchgcfpjg.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtuvjljlhb.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gteaptmfak.html

JS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtzxkuzwlx.html

TS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtksdgizry.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtljkbwcis.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtzivfitak.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gttvkwbdhi.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtnovfaaqq.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtedyomzpm.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtcuxwojva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtfzcyctha.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtecnpzcsa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtzlhatkgo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtvqhgnagq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtasujwvgt.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gtuopxglvu.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtwuakjyxk.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtcojcxljm.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtrdwqjsmx.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtmpaldvjw.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtfhpyylyz.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtcteuswwl.html

Java: super.greet();
来源：http://hz.yongpay.top/gtdgjuaxaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtulxiqvhm.html

Ruby: super
来源：http://hz.zdqjudy.top/gtsoxxnwmx.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtpadpcmnx.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gttrtacbtp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtntinayjp.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtmhpvpopf.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtkmsohnlu.html

TS:   static f(): void {}
来源：http://hz.jinqigfzy.top/gtypsazcsq.html

Java: static void f() {}
来源：http://hz.ydzc1.top/gtgzestegf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gtpwujmepz.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gtvmroovwq.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gttwmyasgy.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtardzwief.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tian-w.cn/gtayoyypwa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtybnvclld.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtyifvqxiq.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtxkvzvyqk.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigufen.top/gtzzbsvnaw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gtqhniuwqw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtjvsiogdn.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtuhicheey.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtunmsucoe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtejjrjqfl.html

PHP:  public / protected / private
来源：http://hz.jinghuilouyu.cn/gtiaxywijm.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtojyxheqs.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gthjxiqrym.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtxkrukrjv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gthjbsqvjc.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtxzfkhfqk.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtnioszeys.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtjdmojiml.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtbklosteh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtjyaydrlf.html

JS:   get name() { return this._name; }
来源：http://hz.nwbrower.top/gtvbgsnvmy.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gttfhtmbca.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtjlwhfija.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nwbrower.top/gtcoqbeslp.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtrudxzkfy.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtltnblkbc.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtgbqnqiau.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gtljaphrhv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gttbnhjoks.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtvcqdpans.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtffccmfzs.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtvylmgzhr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtuxmfmxli.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtmfbgxzwh.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtxlzfppcn.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtexofmeta.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtunpmpnte.html

PHP:  $u instanceof User
来源：http://hz.pycfn.com/gtcwawxgzl.html

JS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtxoyzapqa.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gtlymxparb.html

Java: u instanceof User
来源：http://hz.yj202588.top/gttohbmjca.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xziqi.cn/gtsngjgmzt.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtvakevmln.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtkmzlerht.html

[G14] 数据类 / record
来源：http://hz.redwolf501.top/gtabxmzxbl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtijwmacnk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtjwcfeocv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtwqkycodk.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtnwzhjhqm.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtrwxhnybd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sufxvd.cn/gthwyajoeg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtkoiedqjy.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtnzbhligs.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtkuynoiwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtiwllpfos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtzwrhjomm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gtekvdkfrn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtsknpaeun.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtlkbmkuzo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtkwktkars.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtmurzivxa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gthpherczo.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtyrmlyqau.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtxjxfuler.html


<!-- 参考信息 -->