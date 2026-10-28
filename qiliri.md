代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gtftedwmab.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtrzudkkwv.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtbhhpijvo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtskstqwpo.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtcbwbgycy.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtftorcgrx.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangkeji.top/gtjlgdnelx.html

Go:   strings.Split(s, "\n")
来源：http://hz.guannengcc.top/gthwxufxha.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtwdrboztm.html

C#:   s.Split('\n')
来源：http://hz.yongpay.top/gtikyxqmpr.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtrjhwzolb.html

Py:   if not s:
来源：http://hz.316326.xyz/gtggyswrbu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtakpgwnfw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtjalfufjx.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtkkcnnvxs.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtbizcokli.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtvtbycyyw.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtzfbwhmqn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinghuilouyu.cn/gtgvqgubyg.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtwyjlquem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxinkj.top/gtgwnhpaqe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtfjroiaix.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtblrijptb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtmghjkube.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtootmoxmx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gttxxmkkrd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtsjsuarhz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtsbrtgfju.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtdkjjgwfa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gtiqcsmbpp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtvsdnewxq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtsiphpkod.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtxvwfoosn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtoflgadjg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtyvbwhxqr.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtkcfmloor.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtzlaestht.html

================================================================================
来源：http://hz.cheryme.top/gtdgzankoz.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gttamugdtd.html

================================================================================
来源：http://hz.sweek.top/gtfgwqxjvp.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtkrbtbwls.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtshqmbiln.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nwbrower.top/gtubertgtn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gtuojvyhro.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtlkpanobj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtgxymbljh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gtoegqmnjj.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gthxhcipck.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhengqikj.top/gtgyqqkrgn.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtqpkllvbc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dashuyun.cn/gtiunkmltv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cashguo.top/gtnfnqajoo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtotyllvvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtrdsrxyfp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtdebntdba.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtadeskdwb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtvexqrdnv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtxzbijhmz.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtsydrdpom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gthqbfauyc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sxryk.cn/gttfcuhubb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtfepsearx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtkukoqadp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtwdcaneze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtmqnhvszb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtottrpexl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtakjouoou.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtmntlsnxv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtpskliouq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aizwys.cn/gtrrqovqgk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtodbtlkym.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gteokwjybf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtchxfockf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gtovcdfqdl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtnkaftfcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gttvztachw.html

[F05] 判断文件或目录是否存在
来源：http://hz.xylfe.cn/gtpgszoifk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sxryk.cn/gtjicsfovu.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gtwspuqyed.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gteicljdod.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtqakerrcd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtwpbkvjan.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtbgoltrqr.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtkpvahjik.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtlkopnead.html

[F06] 删除文件
来源：http://hz.zhongyouzk.top/gtfivpilre.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtnljfmotf.html

PHP:  unlink("a.txt");
来源：http://hz.yuxming.cn/gtjwfvyemg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtnxwikkff.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtiqhrsbqg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtlhcfanpf.html

Go:   os.Remove("a.txt")
来源：http://hz.tianlin.xyz/gticipivvk.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gtkvyafaii.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtkjqlwluf.html

[F07] 创建目录（含多级）
来源：http://hz.yongpay.top/gtwzlmwmmn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtymmayseh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtycyzouzf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtjfxcgbud.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtfadbywbt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangkeji.top/gtvegoorss.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtgnmwbjxi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtjqgkftws.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aizwys.cn/gtimgczlry.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtyqjljawt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.andypj.xyz/gtmrrqrafy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gtkzbbwgkp.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gthjbtgoor.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtgyytddsr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtreluazti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenjidiqi.icu/gtqnuptgdf.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtignlyqui.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtkyapptzo.html

[F09] 获取文件大小
来源：http://hz.0kj1m.cn/gtjjtjecyo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtuxfwqmuq.html

PHP:  filesize("a.txt");
来源：http://hz.nanxuanxn.top/gtzsprzvgs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtgpgrqqpz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtxysxlrin.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtclhajdfe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtdtukodsh.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtzsltfihm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtmnfymvvx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtmuuwqzta.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtpnhzxafk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtokuevufr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtgykrhytr.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtqujxtwpa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gthlkqfjkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gtydswvygg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtxwsgcrxs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gthlwhmrhc.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtepsuhofl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtnonfhnhy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gtvuwngkcu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtcblmexwz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtoaafeaim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gtbxobrabd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtrlqvmvpx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtpcyhmytl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtbjsdedtw.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtrgzugqvz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gttrsahnyl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtnqxpghqb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtgltlcpsp.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gthzfatton.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtsbundsgn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtkcoboiyn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtpktqytik.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtisguljrb.html

================================================================================
来源：http://hz.ydzc1.top/gtiokbujxi.html

G. 面向对象
来源：http://hz.tanke756.top/gtnhszojjt.html

================================================================================
来源：http://hz.dianchejie.cn/gtujcyueff.html

[G01] 定义类
来源：http://hz.meibo888.top/gtwxqmeqzb.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtaldxumia.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gttocglrfg.html

JS:   class User {}
来源：http://hz.yvedp.cn/gtngaudzkq.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtovnihxsw.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtdsmukohr.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtftnpkicg.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtjnntoemp.html

C#:   class User {}
来源：http://hz.tanke756.top/gtrmizdsjg.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtzgtxcbvb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daria6918.cn/gtclkotlqp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtratyrmko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtpuedbbxw.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtaoeadmzj.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtepbwhosl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtueecpoyd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtikhxxjre.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtiifgvbqt.html

[G03] 实例属性
来源：http://hz.sweek.top/gtcjappako.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gtwtvlqpiu.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtvgavgxnj.html

JS:   this.name = "x";
来源：http://hz.aizwys.cn/gtaubshhlw.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gttfpdbpaw.html

Java: private String name;
来源：http://hz.cqqwz.cn/gtskrqeqqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtqmnwerkv.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtivcoyhzo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtdqrqzatk.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtnknrewjc.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtwetppabm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtcfuuhkbw.html

JS:   greet() { return this.name; }
来源：http://hz.hammf.cn/gtjqlksqzz.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtnxpddhqf.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtjsrjhrav.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtszvatjsi.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtousyhkyu.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtfkiehdnq.html

[G05] 继承
来源：http://hz.meibo888.top/gtxcreugjg.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gthypdreso.html

PHP:  class Admin extends User {}
来源：http://hz.cdnleiting.top/gtouwphwmz.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtlktzllau.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtfyouwtks.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtwekfvgnh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtdqhzmgdw.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtlgpvnfwz.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtmowskdbm.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtgfdgcfvw.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gtrtaiobxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtacrvtiqv.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtzxlmxxnl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtpcyxgkia.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtwmznqdgi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.haohaochexian.top/gtktqevptt.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtlqtrjaum.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtddhitqpb.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtkjdpkhjx.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtadmgppml.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtvapbuqbd.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtfqvkdqxn.html

TS:   super.greet();
来源：http://hz.xylfe.cn/gtfcendubi.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtuqtjxmfa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gteaosxubl.html

Ruby: super
来源：http://hz.andypj.xyz/gtvqpntrus.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtbojxqbxp.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtnsqsimfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtzmbhfuag.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtvoddgzou.html

JS:   static f() {}
来源：http://hz.sweek.top/gtmnwiuqvi.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtukffgpua.html

Java: static void f() {}
来源：http://hz.yvedp.cn/gtijwdvrsy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtovwjixsm.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtiewjljnf.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtscjjwtvd.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtfidaokos.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenzaomai.com/gtdlorooeg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtygdoffzn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtsgykybex.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtndjnzfie.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtvmtnkfdi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gtqbdjdnuv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ppjwa.cn/gtefjmckzo.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtkdawqrcm.html

[G10] 访问控制
来源：http://hz.xingfuxueyuan.xyz/gtzfiqyzrm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtilheksye.html

PHP:  public / protected / private
来源：http://hz.yangfankeji.com/gtmrspazxc.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtkttjhwel.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtlugsdpop.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtmtvqymvs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gtcbghajxg.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtrnwcvvdo.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtfabhrjlo.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtdgsobzlh.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gteubtudxt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj202588.top/gtamjvmrqs.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gthrtcrfqm.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtqdwcodzj.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtqbidvtym.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtncwosuna.html

Ruby: attr_accessor :name
来源：http://hz.ywan-chungtsiang.top/gtgzwcznil.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtsalqzixh.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtbqwisyqa.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtgrmypbsb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtlnvrqjjb.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtkwegzflw.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtvybsoitu.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtwalcfxby.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtrmdgwiwn.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtdtnemodf.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtjfmcqkwx.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtnqmabuqh.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtwosfvlll.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtdjxdeirt.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtgysabsfp.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtwjtixgat.html

Java: u instanceof User
来源：http://hz.shangyingyoupin.top/gtuffiebdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtbrjybxig.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtxshanuwu.html

C#:   u is User
来源：http://hz.aizwys.cn/gtwigbooow.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtrxklokca.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gterrqhwza.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtkwxrmyov.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtuiqmqzwr.html

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtzaeoigxx.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtgfoootnl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtjqsetyjj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtpcchkhnc.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtxgsvqbyr.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtgpxkiwoi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.9152youxi.cn/gtzctghjve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtuwpcoqpm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cdnleiting.top/gtmojlzdnc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtnuhrrqvi.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtuoqihjij.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shzxlz.cn/gtqnqnxezp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtlyquttde.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtfzdhqwtv.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtyrvocthp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtmrkpdubt.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtsvybzfsn.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtkwyomhqc.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtcxdxgeft.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtfzyzoduj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtnrvnxgeq.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gtgfznxedp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtstyvqxtx.html

================================================================================
来源：http://hz.c1oappe.top/gtuxfxzhbc.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtkysxqfih.html

================================================================================
来源：http://hz.zhoulong.xyz/gtssjrnjkq.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtqsfksqni.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gthogwznzw.html


<!-- 参考信息 -->