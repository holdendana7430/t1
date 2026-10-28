代发 wailian999

[E18] 模板占位符替换
来源：http://hz.tianlin.xyz/gthxhwsmrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gtpcayfllp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtrgalhloo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtwhyghchm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtcfkmsrmo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtrnywhhjr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtiabcwfcs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtdgrwnvzf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.feifeiyinyue.top/gtwmjuwkxq.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtoslchdwy.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gtizjtaqrs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtucddlenm.html

JS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtzpmhiaeb.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtrenhgcdh.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtnfyhmxdt.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtnuvezkvc.html

Ruby: s.lines
来源：http://hz.ydjk.org.cn/gtymctjujb.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtkhnjktuv.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtyyytbljo.html

Py:   if not s:
来源：http://hz.9152youxi.cn/gtpwyeovmc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gthblbrtnx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtprxdcxyl.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtdofbalkk.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtcrqggcve.html

Go:   if s == "" {}
来源：http://hz.hywenlv.cn/gtwhttrhsd.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtcteltgle.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zdqjudy.top/gtjuqirqdq.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtwlgatgxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtiyowyvtc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tanke756.top/gtggastokx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtozvgiumb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtegbdbylv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtsbxfxxaa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.snrcjt.cn/gtbiisvmcf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtbnevlhyk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtqleppvjm.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtrktozaaf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtkikeqdrn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtkcfvebzg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtdzwztuxp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtjvcfjfjf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtmwkmmioh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtljirnywo.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtygeskabd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnqzz.top/gtgoonvrcs.html

================================================================================
来源：http://hz.yj202588.top/gtkyhproud.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gtdarnlova.html

================================================================================
来源：http://hz.nwbrower.top/gtrelyxqwb.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtzcakpfxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtafrozlpp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gttattsqff.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenjidiqi.icu/gtxnlztmfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtsyznkpfz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtgsifonug.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtxlwjuumc.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtozbuyhql.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtclpamdwc.html

[F02] 逐行读取文件
来源：http://hz.jqgufenzy.top/gtsaeplgnp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtyphwfoxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtxmbdkrkw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtmvqrvtdp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtuyyprcci.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtibygcpbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtliftnslj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtfysyzpvz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aizwys.cn/gtrsagchtj.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtwlybmewf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtlgkgtzhx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuxming.cn/gtgwpefrwa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtypjottpm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtypgyxxun.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtcmsfhmpw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtmsphsjti.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gtfxauhgwl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtnzwwukyf.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtpryrecgv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangkeji.top/gtrwkacwje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtxagahkii.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtxopunezd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtumkjwhry.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zycfv.cn/gtlgceealf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtojxixtra.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtraeqnuwr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtvsokqxjz.html

[F05] 判断文件或目录是否存在
来源：http://hz.birdmap.top/gthsjcshht.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtddhrbmxe.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtfozeudth.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtxqdousqj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtinggibku.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtaotewbfx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtqxkrnnik.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtslutqhbo.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtiouumpxw.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtogdagvgy.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtzexrzfya.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gthpvxoamc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtmlyubfur.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtpiltczzt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtpqgaqzyd.html

Go:   os.Remove("a.txt")
来源：http://hz.xylfe.cn/gtjbuvarkk.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtmvgvrntq.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gthlftctrh.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtzkrkjsva.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.andypj.xyz/gtyfrwpiap.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gtwjnvuifd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtkuorkmnb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtepaajpmy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.9152youxi.cn/gtdqduajij.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ivvv.top/gthrzsvwib.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtasyjajiz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhoulong.xyz/gtsdidbtoc.html

[F08] 遍历目录
来源：http://hz.wangshuangyany.cn/gtiddgdzhm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtzhkzjrqt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtrtjyyksh.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtwpfylodu.html

TS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtxslbpsjg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtteopxbhb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtrdrccxiw.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtaaopahcf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gtfdqorffg.html

[F09] 获取文件大小
来源：http://hz.mhx1999.top/gtpfwadhro.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gtrnhllqij.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gthfzcdzid.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtertqdqxp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtbulkyvqx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtfeybukiv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtrhyzvqcf.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gtcfykcghg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtxklovark.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtyevzgyev.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtpyedcqwx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shangyingyoupin.top/gtpeldvvvc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtzjbpxgjp.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtekllpzzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gthknzrdru.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtlhvdbhbi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtlnyiftku.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gzhubu.top/gtaknpxahz.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtfuebesgf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtkkqimsyf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gtcgxsavpj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtvzvzitby.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtgczbkagw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhaomingkeji.xyz/gtrqmzerul.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gtpoctdipb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtjvgghxhc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gtvekzweie.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtlcakayuq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hywenlv.cn/gtqiyxxixd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnxiangtu.top/gtjsitrpox.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtgowtfzab.html

TS:   // 同上
来源：http://hz.xylfe.cn/gtpnhozrvf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtqmdtfvqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtthoqlbws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gttboybkjc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtzicejcjy.html

================================================================================
来源：http://hz.316326.xyz/gtzqzfojeg.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtjxgeawxh.html

================================================================================
来源：http://hz.yangfankeji.com/gtjepixxly.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtruguaorz.html

Py:   class User: pass
来源：http://hz.zhixingplan.top/gtwlirvzkx.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtepkidncq.html

JS:   class User {}
来源：http://hz.xziqi.cn/gtmdojkfyc.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtrhpsdkmf.html

Java: class User {}
来源：http://hz.fzhhl.top/gtbzaxseua.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtoypyeghm.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtvtrybzic.html

C#:   class User {}
来源：http://hz.cucudq.cn/gtbesvxttv.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gteehpjsoc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtpihrlpyt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtwyhfuxzo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtnbsogzkh.html

TS:   constructor(public name: string) {}
来源：http://hz.jyoumei.cn/gtcpxjjsrx.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gtkgnwcpnv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtjdepueic.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtaftppupu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtqalfzddl.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtrbcprvso.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtrxrcenud.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtjlaauoto.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtpjirzqsu.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtepbvctyt.html

Java: private String name;
来源：http://hz.316326.xyz/gtqlgrudqq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtnkcyzqje.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtejvbzoxk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gtddlziuiz.html

[G04] 定义方法
来源：http://hz.tianlin.xyz/gtmaobndab.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtktorchez.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtvghizccz.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gtxhnhgnlt.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtcluqgrej.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtxlyapmrd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtrvnrsiux.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtvhepaqwg.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gtbmvuqxqd.html

[G05] 继承
来源：http://hz.tanke756.top/gtaickoute.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtfgabtgkb.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtuvdlonaq.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtlqguwbpg.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtitwqqetq.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtwhbcnsmk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtvixkdaop.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtrbfqwaeo.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtbbpssmag.html

[G06] 重写方法
来源：http://hz.zycfv.cn/gtkgxwwnug.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtkbmiueps.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtxpfzqmby.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtxjqqlbig.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtbjjhwkvh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtkhrgtydx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtdcnzreyh.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtpeiitppx.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtvmynbucd.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gtemqkrxcs.html

Py:   super().greet()
来源：http://hz.wangshuangyany.cn/gtgyeawqlm.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtkhbycxno.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtfdgmwuzw.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtylzwwnse.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtqueygqjt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ybcxt.top/gtivqikdun.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtdrrfpktr.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtnrzskwgf.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gtdqejrnjj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtdteyncrm.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtyqwfrndl.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtelziewyj.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtiirakezn.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtivarvhgx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtbmprazmz.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtsnznypfy.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtzitdizhy.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gtouuerhsj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtshsgtpmu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtzmqdlomd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtenkygmwu.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtvtwjqosn.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtoctdqeaf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtvoeotlis.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gthamvbjdr.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtbgevfoum.html

[G10] 访问控制
来源：http://hz.tian-w.cn/gtmwpyzagz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtnmlxrsgt.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gtpapznzft.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtqjxpmajc.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtirhjdzmu.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtgobeigof.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtfazpqgoz.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtksspnimx.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtjzwmgvvq.html

[G11] getter / setter
来源：http://hz.pycfn.com/gtsbpenqsi.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtjhprmojt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtinvbzljb.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtpwmyfdsv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtqaevlpca.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtwytqlwpl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtynyvclvr.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtnrhlejxh.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtagwdnzzo.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtsddvaxvz.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtkwxwfahc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtcqffcpnp.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtmmawlysb.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtfzelzpdz.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtnutfkjac.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sweek.top/gtgmirriwr.html

Ruby: def to_s; @name; end
来源：http://hz.tianlin.xyz/gtilpjqlwp.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgfzy.top/gtwvykufsg.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtdgjsiwnz.html

Py:   isinstance(u, User)
来源：http://hz.jiagoushi.top/gtyulpbfut.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtdyhwzwun.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtoqipjqey.html

TS:   u instanceof User
来源：http://hz.cdnleiting.top/gtfpnnnmjl.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtnqeboztn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtyfacmcpk.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtgdddmdgp.html

C#:   u is User
来源：http://hz.xuanzx.com/gtjxzhvbuz.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gtytzwnclq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtuedpgemx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtmaejbkln.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtqycnpeqq.html

TS:   type User = { name: string; age: number };
来源：http://hz.gaohongyu789.top/gtbtiiwnhg.html

Java: record User(String name, int age) {}
来源：http://hz.fengsongda.top/gtrsvlcvhw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtzmjblmjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtwslythqa.html

C#:   record User(string Name, int Age);
来源：http://hz.9152youxi.cn/gtzcmyusam.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtxrtdmznb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtjtjeviop.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cdnleiting.top/gtchhievsh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtqdhvbvjm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtrucaiuxn.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtbmibdbyy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtrutwlpli.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtkcpsdzjs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtpmjkqimr.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtnfyaabcd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtlomvyvbr.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtveihxemg.html

JS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtbkmwddvm.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtdekkmfkj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtbkohogjt.html


<!-- 参考信息 -->