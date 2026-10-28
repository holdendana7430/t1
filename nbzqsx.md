代发 wailian999

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtsrwoeayy.html

C#:   s.Split('\n')
来源：http://hz.haohaochexian.top/gtqunkwgmr.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gtmjlzbuvg.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtigewycis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtukwivsid.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhongyouzk.top/gtgfbxplqb.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtbripyess.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtbjslxbes.html

Go:   if s == "" {}
来源：http://hz.hywenlv.cn/gtdgkbefmm.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtaizermeh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gtzgfeyvgy.html

[E21] 超长截断加省略号
来源：http://hz.xingfuxueyuan.xyz/gtbfyhxcna.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtudbfogxb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yongpay.top/gtedkrzuvw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtbgjqmtoc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtaixzsfxp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtzwgbakll.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sysykeji.top/gtjfeomofy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtlnayqyej.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtqqcyuuyp.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtamwhmwnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtkvpfvema.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtcecqycyl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtuvtdvsfq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtrykytctb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gticiefnnd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aizwys.cn/gtwwodggev.html

Ruby: s.bytesize;  s.length
来源：http://hz.hfpthk.cn/gtcoljfhby.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtguvasfxe.html

================================================================================
来源：http://hz.yj20258888.top/gtzwzovyvr.html

F. 文件与目录
来源：http://hz.daxiang520.top/gtrrvcdvjv.html

================================================================================
来源：http://hz.52xcode.cn/gtlhkuuizj.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtyjdxzcvb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gtwrapynzr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtesmabfbk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtpbhstrtb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gterqqtvjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtofyafnry.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtnncvxbgs.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtqypkortc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtdeolsaqk.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtksmyswph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtxbgqsopx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtxcfqizqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtiuqotqxk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtkeungopv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtcnntyaml.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtuzxcqznh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtghuxptjl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtelbrdoyb.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtzwbapftq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtzcxaijlp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtvnhljnai.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtwsxncelr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtywmxiyho.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtpjzphjva.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gtbxmyncem.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtmlgjuhwt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtaomtiunb.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gtqzfijdal.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtoegjbcoz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gttyswetre.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtgjtrdwke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtksdfzzoi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtozxafrly.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtgxkgcaeb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtwzgfpnji.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtqznsyryc.html

[F05] 判断文件或目录是否存在
来源：http://hz.shzxlz.cn/gthpbrakkb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtemkjnwje.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gtrrourhus.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtpcgpzcfg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.bjfxy.top/gtxbgwmmyu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtnxerxezd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtkkchfeeq.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtppzyuwrw.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtebaosvwo.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gtyxzkfsdk.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtkablhbuz.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtrgncaube.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtggixscod.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtvucwamoe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtdqdqhviw.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gteuwlximp.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtjcjjnzoi.html

C#:   File.Delete("a.txt");
来源：http://hz.meibo888.top/gtxmdchtna.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtqqfyolfm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenlongwang.top/gtspwqfxgb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fengsongda.top/gthumejzwv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtoqebbsrd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtuiqfmuoc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gtzbsdbhbd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhixingplan.top/gtqpvlabok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtklgdbwcb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtgoykkryj.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtuomuroqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gthrfusqbg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtigewvmki.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtspnlkpbw.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gtaertnstj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtvwzrntia.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtyxufaisy.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtujlypjwg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtrcfsydkv.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtzgeetlhj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtdahcgxux.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtomvslbhr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtptlgbopv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtrdplighl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtasgnnijx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pycfn.com/gteluyruhn.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gttvoitriw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gthlvdeecn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.mhx1999.top/gtxxswbizm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtgftqyicq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtlejiawbc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gthtjjwfnh.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtaajyudvr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtspmpfrjl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtgyelypgd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gttryxjczu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.316326.xyz/gtcqgjflgq.html

[F11] 复制与移动文件
来源：http://hz.chenlongwang.top/gtxenkrzan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtiuqpwjpx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtnlwntykc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtipmilirg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtszcqhdus.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtvbragtie.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtbyvxaoiv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtyzhhkith.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtcmeaetmb.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtcmoqxssi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtwmfwbzdn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtpudubnii.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtfrqojpgt.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtrvkbiari.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuanzhike.top/gtddnlcjdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigufen.top/gtzokjkwrm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jiagoushi.top/gtencjvyfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gttmubixks.html

================================================================================
来源：http://hz.yj202588.top/gtcylgcvlj.html

G. 面向对象
来源：http://hz.sweek.top/gtncvsnzfd.html

================================================================================
来源：http://hz.jiagoushi.top/gtnacociip.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtrollntbv.html

Py:   class User: pass
来源：http://hz.sxryk.cn/gtifgsohzd.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtlhrhghzz.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gtbzchaiqr.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtazjjbfun.html

Java: class User {}
来源：http://hz.jlsjyb.cn/gtktzwxtme.html

Go:   type User struct { Name string }
来源：http://hz.yangfankeji.com/gtnfbkrxue.html

Ruby: class User; end
来源：http://hz.cucudq.cn/gtnujbgqsg.html

C#:   class User {}
来源：http://hz.cashguo.top/gtgeweykwy.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtngbfanxq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtwvbnhviu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtmbbibrac.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtmskxhbau.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtfnrslgjn.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtmujsyqbi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtvlawnpkf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtdulypwjd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gthjmibras.html

[G03] 实例属性
来源：http://hz.gotoacloud.top/gtjklskxxj.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtpxmivkow.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtvudclfbo.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gttwiodvuw.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtbgnervyr.html

Java: private String name;
来源：http://hz.xylfe.cn/gtgyxdxmwf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtlnykaqmg.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtlmtiqwsl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtzixbdoqw.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtspyuptya.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtpduuwdms.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtzysnmull.html

JS:   greet() { return this.name; }
来源：http://hz.tian-w.cn/gtbxcflysm.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtycpwzudg.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtzwrsnnjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtoeedwwdi.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtxtflalda.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtvqxkahdc.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtltpbyyya.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtupgnmlrz.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gtmxjliyvm.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gteqnbxouq.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gttfhnseqg.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtepwvnqhe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtplijkfug.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gttdizvvyr.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtjhgsyfpq.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtntvejrcl.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gtzabhqswi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtjryvbiuj.html

JS:   greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtasebrgrv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtlekimpzk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtjuovzpid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gtcgxutjcq.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtwutoyttd.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtiqmchjqc.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtjawueqjg.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtbeyokkan.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtrviwvygu.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtphuvxllx.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtoiaflxwv.html

Java: super.greet();
来源：http://hz.hammf.cn/gtnckwpjok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jianghu66.top/gttgbrbxxy.html

Ruby: super
来源：http://hz.mhx1999.top/gtvcdfioig.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtchiauokt.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtpfbyrhen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtkgyaksue.html

PHP:  public static function f() {}
来源：http://hz.sufxvd.cn/gtgbnrytbp.html

JS:   static f() {}
来源：http://hz.ywan-chungtsiang.top/gtgqnxsfdy.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtikvtxsfc.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtrwnbhaix.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtiraymerb.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtzfpplikb.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtegulhgme.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtmbzafspf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gttjprqezw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenjidiqi.icu/gtxuatkslg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtqvanilni.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtzcyxyslu.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtkzcqsnoi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtyiauovhs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtffkylmpx.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenjidiqi.icu/gtxzrgksbh.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtzgfjlcdw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtvmcrclhk.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtawneapzu.html

JS:   #private 字段；其余公开
来源：http://hz.sysykeji.top/gtwmlbrzlg.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtnnugwuji.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtluzrfsnz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtmwbinfzw.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtjklbizex.html

C#:   public / protected / private / internal
来源：http://hz.zhongyouzk.top/gtcalxkgdl.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtfhorhrft.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gtmmvwnmnc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hammf.cn/gtojwsajeg.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtgsftqcrp.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gthruvndoz.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtlnuxuplv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtmqysybzi.html

Ruby: attr_accessor :name
来源：http://hz.gotoacloud.top/gtfyehsbqh.html

C#:   public string Name { get; set; }
来源：http://hz.hywenlv.cn/gtkzkumyhb.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtybkvldib.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gtjnrzndqy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtawowllot.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gttcpbrkyd.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtzkcmjntd.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtlxdbagmf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtdxfoywyn.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtywfpwwqy.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtfknzzqwa.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtzhfeuvrw.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gtwdyuapjd.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtynziqgkn.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtyryiaclg.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtidwuxuvn.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtqyqiohxz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtsgfzxejq.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtioptsrxx.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtswsfgrnw.html

[G14] 数据类 / record
来源：http://hz.yj20258888.top/gtxqpdrvkx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtrufhnpqb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtljnotioz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtthlmdrjb.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtxgzsoucc.html

Java: record User(String name, int age) {}
来源：http://hz.gaohongyu789.top/gtvmwaqfej.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gtpdwzxhqi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gttoemlpuu.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtlssrzxey.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtqeqtjbkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtxwzylnli.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtcykqvqme.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtdstkftkf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtpxsushll.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtcmfqbnve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gtcrlrvcfs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtzhkpopvu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gteoubuqsg.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtrjafuebd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydjk.org.cn/gtbtwiqqta.html

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtoykijcsq.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gttdatekmd.html

TS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtdkftgoxn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gthxyejxon.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtzfgctkei.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtxhbeikpa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtyypberbi.html

================================================================================
来源：http://hz.fengsongda.top/gtbugocyzm.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtusjfugvk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuvexqive.html

[H01] try / catch 基础
来源：http://hz.ydzc1.top/gtslmgluia.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gthomkahri.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtyujatase.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gthxavihdt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtsugkpucd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gthpszhsnk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtznexsuvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gthlbknbmf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtnyumntjj.html

[H02] finally / ensure 收尾
来源：http://hz.ivvv.top/gthjyrhndk.html


<!-- 参考信息 -->