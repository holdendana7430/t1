代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhaomingkeji.xyz/gtwpnschap.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtpvikolad.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gthtcnrppz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ywan-chungtsiang.top/gtuoeiwoog.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gttfrqvmop.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtngjafbuh.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtlryklctn.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtclpynxbr.html

Ruby: s.lines
来源：http://hz.nwbrower.top/gthaqicgis.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtqfvjfiaz.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gtoyvcomvr.html

Py:   if not s:
来源：http://hz.zhiwuduotai.top/gtfjaqrarx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cheryme.top/gtgptjllvs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shuidangran.top/gtyonktvoy.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtzrvoqkmp.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtwrorvqhx.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtnkkwggud.html

Ruby: if s.empty?
来源：http://hz.kuanghao11.cn/gtkpxntehv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtmonzamoa.html

[E21] 超长截断加省略号
来源：http://hz.redwolf501.top/gtazlkdofz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtaujywlwu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtgnurguay.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtrvsooryr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtxvjzgnqe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtbprnboru.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtkueotjvl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ybcxt.top/gtataultcx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtnauyoymo.html

[E22] 字节长度与字符长度
来源：http://hz.zhixingplan.top/gtudglijlg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gttdxoxmtf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtzmdvebya.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtwqzituxa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtimgcmdks.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dashuyun.cn/gtfduodxdd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gttbkcuzxt.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtsxgqhuyh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtkkvmvgvq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtydzoapzg.html

F. 文件与目录
来源：http://hz.tanke756.top/gtiywmuerd.html

================================================================================
来源：http://hz.yueranfly.top/gtoyucqwdd.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtdgvazige.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtolhjirju.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtnwxkfomz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gteitfbktv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shuidangran.top/gtyphzkqsb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtoqwgfxgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtlujibfew.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtjmmzmjop.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtereskvzv.html

[F02] 逐行读取文件
来源：http://hz.tianlin.xyz/gtolvltzmx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.havefunace.top/gtztevunlh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhengqikj.top/gtwkvzoets.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtjxvsmfwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtnjewnofs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtibdxgpyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fengsongda.top/gtosehaabc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gtjpeqwboc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtawppnprj.html

[F03] 写入文件（覆盖）
来源：http://hz.guowangkeji.top/gtmgkaeimx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fengsongda.top/gtngkejkwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtnclgrtka.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtrezkxsxn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtyduekpcc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtcrjmkzoz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtrzdkyjhx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shzxlz.cn/gttmlrfdck.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtcesdctfa.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtbvojwhts.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gzhubu.top/gtiheksmvd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gaohongyu789.top/gtocevurzx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtlvikxbad.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guowangkeji.top/gtijvrgaig.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtfrarnwfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtbzykygwb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtapbyqkyj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gtnxpvltpx.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtwhzpltdy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tanke756.top/gtwznchcqe.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtacybrbyx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gttuaxalga.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtzvbexobl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gttixfcvqh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxuanxn.top/gtlpjjsapg.html

Ruby: File.exist?("a.txt")
来源：http://hz.andypj.xyz/gthgceozxx.html

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtparyceun.html

[F06] 删除文件
来源：http://hz.sweek.top/gteitccsfx.html

Py:   os.remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtjtwcsmsr.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtjxablndx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtpafthjbw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtsskjjjjc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtgecfyall.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtxknmfejf.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gtpzrqoisa.html

C#:   File.Delete("a.txt");
来源：http://hz.chenlongwang.top/gtuinmbqup.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtdjdwoeqc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtlajmfdhp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtfwlzfafb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtplipwzxa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtzhyfcosn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtkxiyunlc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtdtmfugil.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtqnlqdppd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtfycjzgna.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtrwnkrgli.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtahdqyixn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtqavczlqs.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtyqlsoxwz.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtpiiepmvg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtenrafvgw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aibaodan.cn/gtjugyrvxf.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gthfitcqak.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xinyue.icu/gtljumdxaz.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtmbshnryc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangshuangyany.cn/gtclmjzmau.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtrewxyign.html

JS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtpzyanhai.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtmvxehgwx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gthuevcmdw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtzolvdhav.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtbklmksuk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtzqpshbvc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtdnqufvkd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtadgrkiym.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gtasevvxsk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtcgmxdlak.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtikmuppil.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtislogquz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gtfuplhyak.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtvjzjrcob.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtwxozyqlf.html

[F11] 复制与移动文件
来源：http://hz.wangdashe.top/gtjncdxqdq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtawjpmuxo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtvrpvzdrd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtqcajmfpq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtrmosixxo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtaobvqwap.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtfcleagdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtnkemxgav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtnitaglkk.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtkkcwbnbi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gteocouani.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtdcarbyer.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtfhjyptzk.html

TS:   // 同上
来源：http://hz.cucudq.cn/gtayagoeru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gotoacloud.top/gtliawdvdh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtttwiyica.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtsnhslwtz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhixingplan.top/gtrhsmniwd.html

================================================================================
来源：http://hz.wangdashe.top/gtmauzfhqn.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtshpxnlrx.html

================================================================================
来源：http://hz.guannengcc.top/gtfbqffxfz.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gtcihrqyzu.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtiqporrqf.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtzwsmmzgb.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtukxotdde.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtjzhhhqrw.html

Java: class User {}
来源：http://hz.meibo888.top/gtjrooekzk.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtadwbmnyv.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtxfsllhnc.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gtqadgwawd.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtacjjebjj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtwgbuunwu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pengpengdd.cyou/gtfjzomyif.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtlflllzev.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtflbpmdsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtedeudlnj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gotoacloud.top/gtcbphjria.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtnsgbgjkv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hammf.cn/gtfibbagay.html

[G03] 实例属性
来源：http://hz.yuxming.cn/gtobwkqgbh.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtmlegawci.html

PHP:  public string $name = "x";
来源：http://hz.snrcjt.cn/gtcfzlhwdo.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtxkhxncrr.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtmzvskyjd.html

Java: private String name;
来源：http://hz.cqqwz.cn/gtkovsnpew.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtslzxflag.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gthaugrpur.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtxlpmnvnk.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtihisviis.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtazartdkh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtkxpjgwga.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gtqepaohdt.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtlukowkka.html

Java: String greet() { return name; }
来源：http://hz.yj20258888.top/gtrsmvytrc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtktcpdphx.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtuleqzzgt.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtgqltyrlz.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtspnvuuyy.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtmonkpudi.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtaygifvga.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gthttvavre.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtldxrhivg.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtsqmmybak.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtwjmanktp.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gtfxgehzui.html

C#:   class Admin : User {}
来源：http://hz.hammf.cn/gtkpmtojxt.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtjruzwxci.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtdmdembyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtdpxfwpym.html

JS:   greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtolslajki.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtqrxqvleu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtsbewyugm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtwbmhonou.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtuiohlaht.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtlsrttyyq.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtpcprxixy.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtqpfmqjoq.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtbnbkzovx.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtfthuzrqe.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gttjaehpzc.html

Java: super.greet();
来源：http://hz.yongpay.top/gtyjhidhvj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hammf.cn/gtflrmtzcm.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtauqvevgq.html

C#:   base.Greet();
来源：http://hz.iojbl.cn/gtcwvtxxef.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtgdtxqxsv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinyuanbaomall.cn/gthjqzxwcp.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtzxbhdjcm.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtgekxdnur.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtwuoteeze.html

Java: static void f() {}
来源：http://hz.9152youxi.cn/gtizkusmgg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gtmhhufgak.html

Ruby: def self.f; end
来源：http://hz.yueranfly.top/gtvtzcnaaw.html

C#:   public static void F() {}
来源：http://hz.yj20258.top/gtlpekhkmc.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gtceumsbqm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtjguqgdxm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtqjddaejr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtgcrwtcxy.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtisriixcy.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtxwhblvse.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtsgoqldmi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtklyegfld.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gttgdjfsxq.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtmkospapu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gtpbdnwsbv.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtmegcqgcq.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtndnzqedq.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtcaiiraqx.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gthovmxoaf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtfqgrrqkc.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtedrqemln.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtpxddorea.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtnzmsjheg.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gttqzjqqdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtvcnzijys.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtzwuuetrq.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gteooskzvg.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtkgbpljvk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cdnleiting.top/gtkfzjlkfg.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gthgyrpzmh.html

C#:   public string Name { get; set; }
来源：http://hz.zycfv.cn/gtxbclqojx.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtzuhjoyzz.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtuqpeeyft.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtddghyddr.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtiallbpmp.html

TS:   toString(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtihghdihe.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtinyplkzb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtvsegoxbf.html

Ruby: def to_s; @name; end
来源：http://hz.tian-w.cn/gttntjeacg.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtottcdzzv.html

[G13] 判断对象类型
来源：http://hz.jinyuanbaomall.cn/gtaddfcgjf.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtsjullbzs.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtrhygjfpb.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gtixijisqq.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtbkyofepd.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtiaucqbys.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtvuutcpgg.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtqiuefnsn.html

C#:   u is User
来源：http://hz.ybcxt.top/gtflyjqzin.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtftrcaynq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtklyspphl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtpqippkvl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gttnhyraiq.html

TS:   type User = { name: string; age: number };
来源：http://hz.bjfxy.top/gtzawaczmi.html

Java: record User(String name, int age) {}
来源：http://hz.zdqjudy.top/gtjyljrcfz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtncjxhuqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtwfyldsqm.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtcgacfmue.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtokovooza.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.birdmap.top/gtijlgttay.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtvkpvkhsd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xziqi.cn/gtagyxexnd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtkddrgfez.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtnljarbcm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtjuxqhzzv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtjxjsijjs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtzgylqckj.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtuvlqafgo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gtluqzqpbd.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtpzhstyed.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtnvqafdtk.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtadjhufiq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sysykeji.top/gtoktfydgw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtsfhnskyz.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gtbryxbnhj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtdbbzmnvh.html

================================================================================
来源：http://hz.tanke756.top/gttfkdtaxg.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtlckagxdf.html

================================================================================
来源：http://hz.yangfankeji.com/gtambvvbgv.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtfvgdqdxd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gttpcymhsj.html


<!-- 参考信息 -->