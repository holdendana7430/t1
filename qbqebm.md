代发 wailian999

Ruby: s.lines
来源：http://hz.andypj.xyz/gtxddkfuql.html

C#:   s.Split('\n')
来源：http://hz.chenzaomai.com/gttqxlxyej.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtqqsolopt.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gtuoyeadun.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtidglyixd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangkeji.top/gtjqlsdgoa.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtmkipxlav.html

Java: if (s.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtpnbyowxp.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtoebkmrtk.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtxihafxtw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtlvdpiiij.html

[E21] 超长截断加省略号
来源：http://hz.ywan-chungtsiang.top/gtptxbzmeq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtuaidqxij.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtrccrsonj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gthiscjlqa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtoyobchbp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtszxgekgu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ehwqpu.com/gtzdaucgbj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gttetmqdgo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtrpfhisuu.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gthwdlntgh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fengsongda.top/gtifaehnyj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtwejtpxwr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtrheoczyg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtduelajvs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gtptapkwyv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtnrvdfkhh.html

Ruby: s.bytesize;  s.length
来源：http://hz.tianlin.xyz/gtumzwneno.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtwrhslhtu.html

================================================================================
来源：http://hz.nanxinkj.top/gtblsbjulw.html

F. 文件与目录
来源：http://hz.yueranfly.top/gttqywmrdt.html

================================================================================
来源：http://hz.52xcode.cn/gtizkhmido.html

[F01] 读取整个文件
来源：http://hz.xuetiantiany.cn/gtauehljzb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shuidangran.top/gtcrosdxem.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangtech.top/gtdefadfzq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ppjwa.cn/gtsrmxgxzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daria6918.cn/gtdpeluvcd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtuiilfefu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtwbjovzeo.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtxdvvgcvo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlfoynjyc.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtuxrqzoty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aizwys.cn/gtoifguydv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtrinorgnr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtvurppnjb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtytpeliee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gttqsdxjzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.meibo888.top/gtgzsjeazu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cheryme.top/gtnoktljno.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydzc1.top/gtwfetyaki.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtpawoyung.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtlnpnpirv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtqkwfxeuz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtgnuosgzr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gthtxelapl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtckvnymzg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtvolkitpt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtghwhmpoh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ivvv.top/gtjjmtzuhr.html

[F04] 追加写入文件
来源：http://hz.svipenyu.cn/gtevoapnum.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangkeji.top/gttwqavwxw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtlnnponpu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtcepgzzdw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtlwenjadu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xziqi.cn/gtlnwmbqkq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtxfplfzef.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtounpblbb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtbnpwcqwa.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtrmugbtuz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtomulyooi.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtaphpqykf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtgvuyvcvg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtrcejatgp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtrzncazfn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtnlooohgu.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtgoiooooy.html

C#:   File.Exists("a.txt")
来源：http://hz.cashguo.top/gtyoqsfhuq.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtsqvvqyka.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtpulvcuem.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtoxufnzhb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtygclnmfc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gthvfawxmc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtxebdrkro.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtdnkxdump.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtwtvakqsd.html

C#:   File.Delete("a.txt");
来源：http://hz.cucudq.cn/gtgcjxeqer.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gtswyjuaqv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtykvejrgu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtavxqdtsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtoavjmliw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtjmshxpkp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtpztwtuga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtllfklwmv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtrxhxlgyt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtwrguzvuk.html

[F08] 遍历目录
来源：http://hz.yuxming.cn/gtlzfrqrse.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhengqikj.top/gtnsugsnbi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtjqgdayeu.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtmqqcjyhu.html

TS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtbuutkppv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtlpguhwpm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gtjhzeoyxa.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtlopjxtdm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ywan-chungtsiang.top/gthbwsjpyk.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtcgsdmjkg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gtnxxrsjol.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtrpswixkk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtsxmzcdiv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtkxjytfdy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtkoaiasfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinyuanbaomall.cn/gtgfeuqynm.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtynkegpau.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtxtkyxupd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtvsulirum.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtwbsdlvkr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtzwiiznuh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtzitfhxzz.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtmtlqgdty.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtlzcrpbwf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtcsvwdxgf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtgwgobcye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.mhx1999.top/gtjnhajldt.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtybfguddc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gthdwxkrmy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtpbcifgpq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtxpchjezc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gthjrgvnkx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dashuyun.cn/gtzpkkcmvm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gthwjtnriw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtfnbppafd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhixingplan.top/gtoyjbemob.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtaqducbxw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gttkehsnmg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gtvheojrgx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtymwafimi.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtvnlugyhq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtqlrvnnpr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtiyjdmgpv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtzopxbtts.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtbsmfqgjz.html

================================================================================
来源：http://hz.tian-w.cn/gtgdnodzzm.html

G. 面向对象
来源：http://hz.tian-w.cn/gtcwrrmwae.html

================================================================================
来源：http://hz.tian-w.cn/gtfweoxxwk.html

[G01] 定义类
来源：http://hz.sxryk.cn/gtesxibnci.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtumhorgau.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gtirarwkim.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtwzozabqa.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtfqbhopbd.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtnodjpmiq.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gteahlcuza.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtafwlqyhb.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtpmnoglfo.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gthbppddya.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtfentejoj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtbmqqfbgw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtloluzhin.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtivqffriy.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtjsyhjpsz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtfrlhxlyv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gttyhtvghe.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtbszvxugg.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtvypsjzby.html

Py:   self.name = "x"
来源：http://hz.vqdsnc.cn/gtdwbdtxzy.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtehoblzwq.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtytlcllui.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gtkvcujocg.html

Java: private String name;
来源：http://hz.redwolf501.top/gtpdiwedix.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtxuxoejfy.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtnpefhdon.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.vqdsnc.cn/gtbbynhjfe.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtfgqxwmss.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtqbiuwyal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gttsafhcmb.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gtyjhnqewx.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gthesyujgu.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtchviydvw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtwlyuhuwn.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtusmwesmu.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtqdsrsqut.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtbujgpaiz.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtvfrkntsp.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtzraqjghg.html

JS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtleuqqgxg.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtczwncqrg.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtulzdnxry.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gthsgvkbeu.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtxerrmxre.html

C#:   class Admin : User {}
来源：http://hz.zycfv.cn/gtvaeftjnc.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtcvgpqcuc.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtqvsnhrva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtpuqxthky.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtdxwtpfou.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtoxknxlpf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtzmveyfob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shuidangran.top/gtcluelgzm.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgufenzy.top/gtpzxucars.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtljgygrnw.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtxtbknkpe.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtsxexcnko.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtmzbccwch.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtpinbyjkr.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtclhwocrv.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtggxktnxe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhaomingkeji.xyz/gtlvvmcmts.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtojiepkzt.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtvjdqmpfg.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtunmywclt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zdqjudy.top/gtznfxnobi.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtdzvaxaxj.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtypvocjwl.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtyqnybblr.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtajzytzku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtomjlakgc.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtuewanvww.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtjsrbeagv.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtemmnqpsw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtrewsvpnl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtuwxwnymz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtteswasmv.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtreywotne.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gteiurmaee.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtcfpecyfe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtbfnqhpcq.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtlrqiakll.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtaxlisqqd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtakxwpbyi.html

PHP:  public / protected / private
来源：http://hz.ydzc1.top/gtbjkzrlfb.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtxiopbcxd.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gtvbkdudmj.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtyeoxmcyu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dianchejie.cn/gtsqfgaiwu.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtfpujvhca.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtsketqnbf.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtyaphblqb.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtaboolzdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtujqgxvuh.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gtskpndpas.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gttbmbwmzu.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtzqmedgcd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtivnmizpz.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtechhpzml.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtaayfqnxh.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtheypyyux.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtunbwhsgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtuogpwofv.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtszjitsll.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtczidtgtl.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gtckpvmdva.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtelnpmtbc.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtmzvewqvd.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtolhybsvz.html

[G13] 判断对象类型
来源：http://hz.mhx1999.top/gthfuovgyx.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtwdsqalrk.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtvxonkcmq.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtwzpsnqpp.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtbzkyscvm.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtrsfdrfrk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gttinkwryu.html

Ruby: u.is_a?(User)
来源：http://hz.feifeiyinyue.top/gtqysrvxef.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtvnytvfyw.html

[G14] 数据类 / record
来源：http://hz.hfpthk.cn/gtyriwptih.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtvlfddjtf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtnglhxzlg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtmivcdxpq.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtcgokckyn.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtwdlnxkcp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtvqqeexpw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cdnleiting.top/gtuslkqyqs.html

C#:   record User(string Name, int Age);
来源：http://hz.hywenlv.cn/gthwqaxsuk.html

[G15] 枚举
来源：http://hz.tanke756.top/gtsqwedrlv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtuurgreoj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gtkhmwsakp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xziqi.cn/gtgfvaeiid.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtyprwwfsf.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gtmigrpolf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtnunlivwp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtbcocqpvo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtcrtjmmgg.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtjfaubkon.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtagdryrji.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtblfqjxhb.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtuaexfuhy.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtywqaqxgw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtouzcvlgs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtssbrdcwg.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtqplqkcmd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtswvyendz.html

================================================================================
来源：http://hz.sxryk.cn/gtqggrjgao.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtartyjpxr.html

================================================================================
来源：http://hz.yonumen.top/gtsjhctsgy.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtazquqypa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtmmwanpwp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtsjmbhacn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtcjsmdejo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgfzy.top/gtbvclrnmm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ehwqpu.com/gtcqofdwrn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtttndmflh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtycvknojv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtxmuubucv.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gtrxoswthk.html


<!-- 参考信息 -->