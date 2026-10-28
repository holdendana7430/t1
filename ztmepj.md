代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtpzcpirju.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gthleinzfz.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtdyyabsrz.html

Go:   strings.Split(s, "\n")
来源：http://hz.hammf.cn/gtbamqicwj.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtztljgzfb.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtlntygcjd.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtvpooienw.html

Py:   if not s:
来源：http://hz.svipenyu.cn/gtyixmlhrw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtztesmzsa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtniqkalrl.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtcqzxkaqf.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtdtemmtgv.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtkssiiglx.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtbfbwqejj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtqqbcpfwg.html

[E21] 超长截断加省略号
来源：http://hz.hnqzz.top/gtgubnjkso.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gthosnsvba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtdkwgdlpj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtilegvxwr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtjfctbnvm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtdkqsmobc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtxzdckkhz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtxukdhhah.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtzbvhuxen.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtjadosqwp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtvaiesnko.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtjgldkecu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtbonhbwcf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtcejjkgpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gthtbhfhbh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtpclsiqit.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnqzz.top/gtbifqzzgp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtmxalqhby.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjuwosgtd.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtbiffjsbz.html

================================================================================
来源：http://hz.cucudq.cn/gtfpkxdefa.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gttufxjzss.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gzhubu.top/gtqingqkan.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtguqrymgc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtwsljbtsg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtxraulyiz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gteddhsjug.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtrdnmxoad.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtwfnjkdzi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gtkwmywcmx.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtnuarokse.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtweqdwvhd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtnecrvyyw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtnvqnrbib.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtycduexlw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtbsmidsxo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gtfjvgxdoo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtrylimznv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuxming.cn/gtuqcnkwuk.html

[F03] 写入文件（覆盖）
来源：http://hz.316326.xyz/gtixqgaart.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtjwfacdrw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gtodqpgfhv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtvuvtlbqy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtaravsazc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtfreogmop.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtscvgwxkk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gtspjhvuin.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtghgqehoq.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtjkhotbch.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtidkymshe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtoonhhxcf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtcupxuegk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtwscgeacc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gtknylzdbr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtywsfnwhb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ybcxt.top/gtnsavnlug.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtwazedysn.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gtxiihlzty.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtyrquvham.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtihmjuepm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtzurfzxzn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtwbcswhmz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtxdnwcopw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtmbktclso.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gthewbgofz.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gttfnlkcci.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtruakkbtd.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtyiljwcpx.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gteixjsgxq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gttlwzulmf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtpjqxctfe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtgbtlzroe.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gthrwltunl.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtxqubzozr.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtywrbprsh.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtvtaqphys.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtcelpevqf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.c1oappe.top/gtjselhjaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtctpwuszg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtftnatajk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtqhinodca.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtagtbjkyh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gtkoqrnutr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtwuezgwhl.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtkmaxghrf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtxogladzg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtslokeibm.html

JS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtaeiijmuj.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtvkrmflqf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtiyseixhn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtkqzgzbom.html

Ruby: Dir.children("dir")
来源：http://hz.aibaodan.cn/gtuhduhtow.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtdhkuoumg.html

[F09] 获取文件大小
来源：http://hz.feifeiyinyue.top/gtjtojobbr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtxfxugfgc.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtgdjmczir.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtsrfglfgg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtumkqkhpw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtirndmkta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtkcullumd.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtelewvapi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhoulong.xyz/gtpreslzyg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtdptigunr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gthhmuvpon.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtymmtoojn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtuwmowebi.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtfbtfsapz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtiegjbbes.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtjihmwyyu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gttvshrxaw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtlzguadas.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtmvbmlben.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtasfmnyud.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtrbzjrvey.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtnbjxbjeb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtcvsokukl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxuanxn.top/gtylirtbtw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhiwuduotai.top/gtlfyyjvlq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtsrcddpxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.meibo888.top/gtujejsppn.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtvhjygtqy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtekyzncot.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gthtgcwxcz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtzypufwnt.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtyzeenatg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fengsongda.top/gtbvylcotl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.svipenyu.cn/gtkwuefhbb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gtsfogqgqh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dianchejie.cn/gtdakowvfl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtybfvoujn.html

G. 面向对象
来源：http://hz.nwbrower.top/gthurolmrn.html

================================================================================
来源：http://hz.chenzaomai.com/gtgrpexltd.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtcknlvwck.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtbcrylapk.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtzbngxzdq.html

JS:   class User {}
来源：http://hz.sxryk.cn/gtiwdolofa.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtvtksnjzp.html

Java: class User {}
来源：http://hz.yonumen.top/gtmmtejydn.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtvtbgtomc.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtavfkbtjl.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtnmthhlzx.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtshthvjdo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guannengcc.top/gtsetxueay.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtscbowzbb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtidrrumed.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtgxiryebo.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtdccntffr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtyipczgbj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhiwuduotai.top/gtodvnblsl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigufen.top/gtmoacbvul.html

[G03] 实例属性
来源：http://hz.pengpengdd.cyou/gtibyhlysm.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gthxwozedn.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtceuyxkqa.html

JS:   this.name = "x";
来源：http://hz.zhoulong.xyz/gtxbadzqlt.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gtptnwjezz.html

Java: private String name;
来源：http://hz.yj202588.top/gttsbnhvqz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtyqgpbxpu.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtgigyjffq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtwmxpwnrp.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtcgngsghf.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangtech.top/gthqrkdgdd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtaiqwacbp.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtxvegdipv.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtzsfrflhb.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtayujfrsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258888.top/gtprybfnlz.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtuqskklfi.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtmmiuxybi.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtbehaqqwm.html

Py:   class Admin(User): pass
来源：http://hz.haohaochexian.top/gtxvxqxfyr.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtjnrqpqsl.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtnhxzopzq.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gthzxkihfq.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtybfdgmdg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtfydpnuec.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtvhpogair.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtgzgvfrei.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gteikxdufg.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigfzy.top/gtqhzetebk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtvajzgdnj.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtheuajuin.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtlyeufnpe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtvkhapywa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtemrxdfbu.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtrwpkhzzv.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtrxmlsiri.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtyyakqfxu.html

Py:   super().greet()
来源：http://hz.yvedp.cn/gtqqkkxmos.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtadeoyxjm.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtdtpcwlwf.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtlyvescyh.html

Java: super.greet();
来源：http://hz.pycfn.com/gtbmfdstve.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtijtwkqkq.html

Ruby: super
来源：http://hz.mhx1999.top/gtkeuxgoni.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtlamvbnhg.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtuflgqqcz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtrmwvthwc.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtbzikbkkh.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtoatyzsmh.html

TS:   static f(): void {}
来源：http://hz.ydzc1.top/gturfumhdp.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gtrlmsyiik.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtqqnrmxnb.html

Ruby: def self.f; end
来源：http://hz.zhijiandao.cn/gtojnilhst.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtqjobolel.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtvkiqxoqc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtnahmxhvr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenjidiqi.icu/gtxydljaja.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtfumnecec.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gthkathqnb.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtyqrpgbiw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtlldupwts.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtyszraidx.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtmzgbunwg.html

[G10] 访问控制
来源：http://hz.sweek.top/gtqxlvioty.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtcharhhis.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gttxhodzoz.html

JS:   #private 字段；其余公开
来源：http://hz.aizwys.cn/gtvulfncab.html

TS:   public / protected / private
来源：http://hz.yvedp.cn/gtvmhousia.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtamnzmrva.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtggimkicb.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtvqwkocvh.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtncsavjfv.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtpxkcztng.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gteajimcml.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtrgtksuze.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtsqkgfokc.html

TS:   get name(): string { return this._name; }
来源：http://hz.jiagoushi.top/gttprfocib.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gtblddlroc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtxrcfwhue.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtdzkjqnds.html

C#:   public string Name { get; set; }
来源：http://hz.hywenlv.cn/gttbphmemt.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtmwflxqgu.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtqzlznvzm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtxqyowihv.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtsfygojqt.html

TS:   toString(): string { return this.name; }
来源：http://hz.shuidangran.top/gtbcdngoqy.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gtotrewbrr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gthiimfxle.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtmvvcvavj.html

C#:   public override string ToString() => Name;
来源：http://hz.sufxvd.cn/gtqvzmxfqa.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtsgseliar.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtniubprdt.html

PHP:  $u instanceof User
来源：http://hz.dashuyun.cn/gteeuhhsbd.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gteewamwll.html

TS:   u instanceof User
来源：http://hz.daria6918.cn/gtpubccccw.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtmhguwlzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gttpaxzmiz.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtsmlawlmv.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtcfglxfbs.html

[G14] 数据类 / record
来源：http://hz.zhixingplan.top/gtbutlvlzg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtrwizfbny.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtlsizzoth.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtiprvshuv.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtjliyfiak.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtduhogzol.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtvcddppfx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gthxewikqe.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtfxahkavw.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtsawnxxkp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtduownkye.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangtech.top/gtnlthmcpf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gtbqxmfwoi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gteuiieked.html

Java: enum Color { RED, GREEN }
来源：http://hz.aizwys.cn/gtojldrxfq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtxdesfvxt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtksqzfwnu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtamdmtwys.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtuthkcgpu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtslqpakzp.html

PHP:  get_object_vars($obj);
来源：http://hz.yanxiufei.cn/gtobxybpyh.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtouklhdew.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtfuaosjpr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtzilwuzjd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gtxpqopdtf.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtjymqxukj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gttfieyqoh.html

================================================================================
来源：http://hz.birdmap.top/gtvwzlzfmi.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtbzygiqne.html

================================================================================
来源：http://hz.sweek.top/gthqcrzwix.html

[H01] try / catch 基础
来源：http://hz.wangdashe.top/gtdwlndfpc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuanzx.com/gtqiltpkao.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fengsongda.top/gtruaxtjwk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtsejosonc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xziqi.cn/gtnpmlgjzw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guannengcc.top/gtefaivwfg.html


<!-- 参考信息 -->