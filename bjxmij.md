代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtzxqpzune.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhaomingkeji.xyz/gtmqxekijh.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtwiakuazx.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtoyjlbnam.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtyojcbegf.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gttstnmpdh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangshuangyany.cn/gtykfomvhh.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtuniimbib.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xziqi.cn/gtkwoosycp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj202588.top/gtsvilcmep.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtexsuxupz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtcyxrxpkd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gttgnpyfrx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gthygrmdni.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtwwmcgegn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cdnleiting.top/gtmqhyxrof.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtzdvdhqyp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhoulong.xyz/gtsufzpoeu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtogsqmptu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtgixpafpp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtphnglfxe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtwancejlt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtrqqbftci.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhixingplan.top/gtnigpcpqm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daria6918.cn/gteymxcdjg.html

================================================================================
来源：http://hz.redwolf501.top/gtauevswzv.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtsqissowe.html

================================================================================
来源：http://hz.jqgfzy.top/gthagnobkc.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtbmxuhsvl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtkvirqejw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gtgwurymqg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtaogxwxpe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtwqmrhsah.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtyvmyuvtd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtowcteljo.html

Ruby: File.read("a.txt")
来源：http://hz.cucudq.cn/gtzjwoosfj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtsqjibuau.html

[F02] 逐行读取文件
来源：http://hz.xylfe.cn/gtghlrxmne.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtfnacgxhl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtizmlijvy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pycfn.com/gtetnyfmjd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtabyzkzij.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtdutjyvzl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtxykwwsbd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhijiandao.cn/gtrcurvyrb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dianchejie.cn/gtyyfppcvd.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtmlyxebpz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtmqrofowj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtaltxxoet.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gthenhnrib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtnnsngemo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.smart0.xyz/gtlgltqdtj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gttujyucuz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xinyue.icu/gthvbqelmt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtcqebstzc.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtcwxojvaz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtrchjjbvs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gtvxyjdweq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtdtbfonzu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtemdtunji.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtpkjwjebr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtwpaqzell.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtmrkfyntg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gterkpkrpa.html

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtjnvldtpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yangfankeji.com/gtjrzboxmi.html

PHP:  file_exists("a.txt");
来源：http://hz.jianghu66.top/gtgfowqiac.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtfjbxcila.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtovubfuiv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtqkvmtyns.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shzxlz.cn/gtqkslmhks.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtoiovkpwe.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtjueucztk.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtxiglpikn.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtqoxxibfs.html

PHP:  unlink("a.txt");
来源：http://hz.meibo888.top/gtsownbdkj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtbhuwxvjy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtqllpikgg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtftyvyosf.html

Go:   os.Remove("a.txt")
来源：http://hz.quarkkingdee.top/gtvndalhjq.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtlegsfccs.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtydcvxxaz.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtfxmjbvly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtmuidydgy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gthkjxotpn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtpymefqis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtpmvejtud.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gtbqaueeuu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gthbfjhvkq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gthhnvojmx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtygeenmgc.html

[F08] 遍历目录
来源：http://hz.aibaodan.cn/gtwwppuqft.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangtech.top/gtijoznfct.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtfcpsidzz.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtzmymjoum.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtwhtfleaz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtedrfqxin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtepbborim.html

Ruby: Dir.children("dir")
来源：http://hz.yongpay.top/gtcdjlsjww.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ppjwa.cn/gtqbhszzwb.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtozcimetw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtiedkijgg.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtwceovvse.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtfpjgfbwy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtnouvdoae.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtnzotpjnu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtgqbqerbr.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtfnohvtwc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtdpcqrvhh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtvbehhhfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gthsjjpyei.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtoaftwdfq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtevaaeptx.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtyepmymtg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtowwymyaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtxeffbhva.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtvhgjxzbe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtdhowmlrl.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtzkxulcmb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtwuairlap.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtphnhsqaw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtrkqgvsmf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtemjeqgfp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtpbklcjim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gtznmzixcm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtgycldnxx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtrosbmdjr.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gthkawdohn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtgwnkfkpx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtrzijfebu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.0kj1m.cn/gtoydchidc.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtzoqcaqpm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtjzgxuvul.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtixkryukp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtniztfspd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtlcftkned.html

================================================================================
来源：http://hz.yj20258.top/gtoyhrbyvl.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtiizdjdys.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtauzcqazt.html

[G01] 定义类
来源：http://hz.ivvv.top/gtnghpzskm.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtuqngvlwm.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtouropzcp.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtdhwmwidg.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtbafzhejo.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtrgwylsbo.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtzfgkbeya.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtdwnwnmyt.html

C#:   class User {}
来源：http://hz.dianchejie.cn/gtyexulvnh.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtepypzceu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gthyerusgz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtkddsunsp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.redwolf501.top/gtrdkyfygv.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtrlpoiefc.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtaydzdtnw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.quarkkingdee.top/gtpcaepbda.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtexlcugsz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtpcisptge.html

[G03] 实例属性
来源：http://hz.yuanzhike.top/gtyorsnzsn.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtrirqavnl.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtnlxiyqwt.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtcegnsnmg.html

TS:   name: string = "x";
来源：http://hz.yj202588.top/gtozirveoz.html

Java: private String name;
来源：http://hz.xinyue.icu/gtducssamr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cdnleiting.top/gthylhvfgh.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtevnrchxd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtvbpbgsmk.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gttjmsoamn.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtqoqgimpt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtrvkljiwd.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtxvovzsln.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtxfuqdsgp.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtmoomuega.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gttntbxlpx.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtddkswcxy.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtijehaxfn.html

[G05] 继承
来源：http://hz.aizwys.cn/gtpcldqrlg.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtuymocevp.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtwxsghztw.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtougopbom.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtlwsnbjti.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtfeklhhqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtvoiypsxc.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtrpfowfqu.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtczihmjch.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gttakwehka.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gtfsjnprif.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtgvzrpptw.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtwjagikcq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtebvuhkuf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtloclelti.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtankjxmca.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gtovrctbah.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtnffvlhnx.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gtlxfwoied.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtltjtflur.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtzeqgyodp.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtqyqtqfyb.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtrglufumn.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtkvgpylma.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtuwymvbut.html

Ruby: super
来源：http://hz.shzxlz.cn/gtmeuzlhgm.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtpxxwtatt.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtcexrqxil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtcacozwwo.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtzzmrclbt.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtiygwsmfb.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtphqjvtnr.html

Java: static void f() {}
来源：http://hz.jyoumei.cn/gtzikemean.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtpxwioyvh.html

Ruby: def self.f; end
来源：http://hz.xuetiantiany.cn/gteemgytio.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtnfazcqla.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtmhzovftw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtvgxjbpqr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sufxvd.cn/gtormlwjaz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtbinzfgrf.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtuaindhdp.html

Java: interface Shape { double area(); }
来源：http://hz.vqdsnc.cn/gtxfmmyneu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xylfe.cn/gtlpqgnwtm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gttynydgeo.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtlbwvlxve.html

[G10] 访问控制
来源：http://hz.havefunace.top/gtmufgnjda.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtdoxfnift.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtgdnzxagi.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtmjyehowz.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtdibrxkmd.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gteoenwoiv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xylfe.cn/gtueairiic.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtgicjmujy.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtrdgiixas.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtekszlrzr.html

Py:   @property 与 @x.setter
来源：http://hz.snrcjt.cn/gtxdivugzf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtouewmgxq.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtfufxrmik.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtckrnixvl.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtbvnyaiwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtoowwvpml.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtqnigcrej.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtkydzblwa.html

[G12] 对象转字符串
来源：http://hz.c1oappe.top/gtkgaxtwbh.html

Py:   def __str__(self): return self.name
来源：http://hz.daria6918.cn/gteyierija.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gthpswhkfs.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtnvmjvexe.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtqaakybmz.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtvercaaye.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gteukyoqut.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtvfzpffoe.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtyotrdfse.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtafmhgyed.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtfyplhxhu.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtoicllrse.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtjttpqaih.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtvdhuxhkl.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtmpmhaxkp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnxiangtu.top/gthknzavtw.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtzcwvrvdf.html

C#:   u is User
来源：http://hz.ybcxt.top/gtyjpwtrvv.html

[G14] 数据类 / record
来源：http://hz.cdnleiting.top/gtfcoemrmh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtfnzetpul.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtstgurzxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtaytsjfye.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtfsbndibi.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtjvkrkzvk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtavofesrb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxinkj.top/gtcfmztmjd.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gtepqhoipw.html

[G15] 枚举
来源：http://hz.meibo888.top/gtfcyfvyfm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.haohaochexian.top/gtwrftzfvj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtordwfmpt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtajtjgvlf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtzwyheatn.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtersowulo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtmjhvrdxf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gttkrylynu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gthjnwvfkn.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtbklxjmcy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gteqbhosvg.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtguomeojf.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtloeyhoma.html

TS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtwqhtsurg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gteykdvtfi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtdzaawkng.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gtfgraqxyt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gttdxrpooh.html

================================================================================
来源：http://hz.tianlin.xyz/gtarmyujom.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtmpoqebcd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gteawlctmf.html

[H01] try / catch 基础
来源：http://hz.ivvv.top/gtdfurkyss.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtabirrthe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtvitvpgwo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtwhzyrbqo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gthbdsdqeu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gtnwwygsna.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxuanxn.top/gtvswjfqio.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gtiiyvemfv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtxglmcvjg.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtifrtqujs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtjkhsibow.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtpwwmygwd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtybumdhbc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtxltsrxaf.html


<!-- 参考信息 -->