代发 wailian999

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gthdxvlguw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gtdufwheie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.iojbl.cn/gtqfzhbfyv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtrrfqzhlg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtcfwippjy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gthiresgrn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtcdwhxddj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtyegjqwpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtjqdcxjrb.html

[E19] 多行文本按行拆分
来源：http://hz.yueranfly.top/gtzecqwdhq.html

Py:   s.splitlines()
来源：http://hz.cdnleiting.top/gtwgvbeeoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.52xcode.cn/gtbquhcyma.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtfvzczkuq.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtjjrgeagu.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtkzzvapht.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtrjvpauzc.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtidodjucs.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtqkduppoj.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtcpmlgjwc.html

Py:   if not s:
来源：http://hz.cashguo.top/gtnjyrnifq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yanxiufei.cn/gtgilbutgy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtobpvkvay.html

TS:   if (s === "") {}
来源：http://hz.xuanzx.com/gthtdaxaec.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtvpfozijh.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtnmfdmgwz.html

Ruby: if s.empty?
来源：http://hz.havefunace.top/gtbfobkyuu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtpwzlfkjb.html

[E21] 超长截断加省略号
来源：http://hz.zhengqikj.top/gteqbvbuap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daria6918.cn/gtewrvntje.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtxllfnkaq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtxoxqecne.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtwwnzzhze.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtcsziclif.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gtruwwukzj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtjqazbxka.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtirmrzoai.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtbmpdpuie.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtaphfobky.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtmtvxzjqf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtxnadlfxr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtvlkeksfv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtyiuwamec.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtirnnmtil.html

Ruby: s.bytesize;  s.length
来源：http://hz.svipenyu.cn/gtywclhick.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtqrhflnra.html

================================================================================
来源：http://hz.zdqjudy.top/gtlnobxfdt.html

F. 文件与目录
来源：http://hz.jianghu66.top/gteqxuiaoj.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtehpybjof.html

[F01] 读取整个文件
来源：http://hz.zhengqikj.top/gtfwnbimwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtslsoxvfq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtuwjcoung.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtrkhbakqk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtztszpepn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtugrsavuk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tian-w.cn/gttmbfpwsd.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtwlrgolma.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtwoutkrly.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtzhusyqwf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigfzy.top/gthxeessqc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnqzz.top/gtrqkbsxwo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtdobnhelm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtdupuwecg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtnwfrdonm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ppjwa.cn/gtezoxjjcs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtrngqewwj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtomnkmaff.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtvqqrofme.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jiagoushi.top/gtvwohmtlz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtvpmcbhfh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtzkumtzbc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtruvyrcer.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnxiangtu.top/gtklgutzls.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.bjfxy.top/gtuzqxkywy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtxndpzdyb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtbeyfqbwk.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtimeoldpj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenjidiqi.icu/gtoaknasas.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgfzy.top/gtvekbkmsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtxdlvjnpy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtlzzletam.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gttidxofjq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtryqraguu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.havefunace.top/gtpbjarnqj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtbglxyvry.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtbmqjfwrw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtiyfgspqo.html

PHP:  file_exists("a.txt");
来源：http://hz.hammf.cn/gtdlidtgla.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtrxfyupcr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtvfsghjoh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtmphovdsv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtdhxacrda.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gtisusgyre.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtywgeyxkk.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gtrhofcees.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtkmascirz.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtomkfzdoy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtjpqwuwzx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtyzxglpgn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtqlyeqpdn.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtnwxdazpe.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtiwrzbapw.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258888.top/gttpzhrcvb.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtrlkwtzng.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtmahxjibn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtvveaxeen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtqnncbkrh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtxigrvyzz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtxhnkhrzj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258.top/gtbgnkrkya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtdiearsit.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtgfobzyvt.html

[F08] 遍历目录
来源：http://hz.aizwys.cn/gtnlvepnlv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtifnxcbxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtfwwbxeba.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtnyepfote.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtlxwbokvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtxiqgbjwp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtjhobbums.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtwtttpaml.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fzhhl.top/gtyvoqqnhy.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtoyckqjqo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ybcxt.top/gtymhbtzti.html

PHP:  filesize("a.txt");
来源：http://hz.316326.xyz/gtgksoatnf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtkofrmftf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtuiryfhaj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtmacukwbl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtuvmjtswl.html

Ruby: File.size("a.txt")
来源：http://hz.tanke756.top/gtvdtsjbdt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhongyouzk.top/gtzeolkifp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gaohongyu789.top/gtnxniqmnu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtekbolqoe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gtdsapepmn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtqeiekonk.html

TS:   path.extname("a.txt")
来源：http://hz.quarkkingdee.top/gtwvdqdkmo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtoeflawrw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gthnbyptfe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtmdnrfyvc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.iojbl.cn/gtcclelzna.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtwepvlwcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtfqbwcymp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gzhubu.top/gtfywattfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtnegzwdvm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtsqobspjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtupiovyyk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtuhkctuuw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtqkesdbnv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtwurasyef.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gthgwaaqkt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtzvckvusv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtgiqxzoul.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtwlxxjzqg.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtqafqldna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj202588.top/gtnrdjdrhu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtfedrdgzy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtljsaoncm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtbcjfmoic.html

================================================================================
来源：http://hz.yangfankeji.com/gtsnondeem.html

G. 面向对象
来源：http://hz.c1oappe.top/gtcgyhesgz.html

================================================================================
来源：http://hz.svipenyu.cn/gtomnefoyz.html

[G01] 定义类
来源：http://hz.yongpay.top/gtjzxctseu.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtbbozuske.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtxufzgayd.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtwrwftcik.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxinkj.top/gtoplfvtiu.html

Java: class User {}
来源：http://hz.ydjk.org.cn/gtxcrgduyj.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtbwnoofxa.html

Ruby: class User; end
来源：http://hz.dashuyun.cn/gtudyfobcw.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtntschsuk.html

[G02] 构造函数
来源：http://hz.zhoulong.xyz/gtbwlvljon.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ybcxt.top/gtljboaslt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtscedmwkg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gttlpwgdip.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtprlxyxsy.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtwakzqjsh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gtoybwenii.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtqafcnmfm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtcpunnade.html

[G03] 实例属性
来源：http://hz.xinyue.icu/gtocgeqvja.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtrugrprkn.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtrzpqqmiz.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtdmprgkxj.html

TS:   name: string = "x";
来源：http://hz.chenjidiqi.icu/gtjymxmlbw.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtayfrroow.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sufxvd.cn/gtbemynxee.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtmlbfpwwc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtweawpjce.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtfjpunwwo.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtojdelypc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtwfbpyrir.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtzurblqoc.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtmakayser.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtosrphtev.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gttayeajmh.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtyhgyptec.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtfzhfmeuu.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtuqmwugor.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtrhqyuteq.html

PHP:  class Admin extends User {}
来源：http://hz.daxiang520.top/gtxbjymlak.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtpnbcjmlv.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtmvbjndtc.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtuivvsghm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtlyufiujc.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtdgufuetj.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtbddwtjkt.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtvglwihjt.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtmdkrdtxd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtlczqlvkh.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtalwgedyf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gthzpcqtng.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gthcnyyxwd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pycfn.com/gtwzkdqleo.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtiqmtvcjq.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtzjnsrnoz.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtitzvoulv.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtgyhiorfs.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtcaffrtmz.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gtohaqagqn.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtklnyhqkl.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtyezwrhom.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hywenlv.cn/gtwnexpzjs.html

Ruby: super
来源：http://hz.vqdsnc.cn/gtrfuorvot.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtfxidqjco.html

[G08] 静态方法与属性
来源：http://hz.yuanzhike.top/gtgsbbzaar.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtcuopauyh.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gticjpqkjd.html

JS:   static f() {}
来源：http://hz.fzhhl.top/gteyilmgab.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtnrhahoet.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtpyslnefq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtokkxeere.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtpclepjwo.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtahksfjdo.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gtljfgpohz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtbkmtdlmw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xziqi.cn/gtvurpluys.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtleovqouf.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtsyxdytog.html

Java: interface Shape { double area(); }
来源：http://hz.hysaishi.cn/gtvownqgjo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtkxyutfai.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gogol.net.cn/gtftrpewdt.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtaffxwkqn.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtbfjzzizi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtmajeymcb.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gthvdyfujw.html

JS:   #private 字段；其余公开
来源：http://hz.ydzc1.top/gtvwanuqkp.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtwzkgtlcv.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtanpifjtm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gtavpbpxxz.html

Ruby: public / protected / private
来源：http://hz.gotoacloud.top/gtahtigdup.html

C#:   public / protected / private / internal
来源：http://hz.fzhhl.top/gtpniraazg.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtmbqdrika.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtuslfesmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtafonsywk.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtobxoxpum.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtjiqtgwtu.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtgpoxzzix.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gtggjdlwmb.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtfjozfqhf.html

C#:   public string Name { get; set; }
来源：http://hz.chenzaomai.com/gtqlobhjpb.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtpusiejjp.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtnhdsmlkd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtahewtiji.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtkizzgbdn.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtpryhtbfv.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtfygfxjdq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tian-w.cn/gtujvbxlmu.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtkgzqliit.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtslajhrha.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtatvcllij.html

Py:   isinstance(u, User)
来源：http://hz.jinqigufen.top/gtlpsudnoz.html

PHP:  $u instanceof User
来源：http://hz.xuanzx.com/gtppwhsaft.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtdqxfcftl.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gtwhpfccev.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtiodydkfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtalshyyaq.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gtbbxjelan.html

C#:   u is User
来源：http://hz.redwolf501.top/gtduksndfz.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtqhgbtfke.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtkemlpbqj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gteydjcnau.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtvnwwnyib.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtlddfwbyn.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtxykiokbo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtimprpkob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxinkj.top/gtmybtoikw.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtzproqrhd.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtvjmrvpsa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gthrbseavy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtxlwhrqry.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtnrpjthhb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtpwictvzg.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gttdjbmaqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtbbqwysro.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtrocarlfw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtmssetujl.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gtloiypohc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtbatzzddj.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtzatdnuhr.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtvjnlbscr.html

TS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtgrhovcnp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj202588.top/gthvvitnwt.html


<!-- 参考信息 -->