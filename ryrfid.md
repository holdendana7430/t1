代发 wailian999

Go:   if s == "" {}
来源：http://hz.andypj.xyz/gtpuzoywqy.html

Ruby: if s.empty?
来源：http://hz.jyoumei.cn/gtmbbyyxom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zdqjudy.top/gtjaakribd.html

[E21] 超长截断加省略号
来源：http://hz.cheryme.top/gtbzxrislj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtywqroqja.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.mhx1999.top/gtliiudjmn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtrzhkkfjp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtuvbnwlmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtqkpshbuw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtxkqwfdny.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daxiang520.top/gtzpckpgqn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydzc1.top/gtctdvyzsu.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtnlcqupxy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtqxvnsyhx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtdhoaaeca.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtpzqdqmah.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtxfolowsu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtgabxbiup.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.svipenyu.cn/gtiruspfbj.html

Ruby: s.bytesize;  s.length
来源：http://hz.cqqwz.cn/gtcxrqqtxx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cheryme.top/gtdlrymvtc.html

================================================================================
来源：http://hz.smart0.xyz/gteqqydecz.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtmicxgtxz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmaoefspi.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtzrzjznby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtccbosktm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtfhjlqtag.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtzylypltc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangtech.top/gtennpsbwo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtdaxlqtxi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hammf.cn/gtwjytmwpr.html

Ruby: File.read("a.txt")
来源：http://hz.cqqwz.cn/gtdohgcyrb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtubtvssuj.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtqefhkkte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtxunfnhrp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtruzshabs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gthzcujmok.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtzuqldqjm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtohacgmhz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtpusbutcy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtyejwkfov.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtawuxwvza.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtulrmxlao.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhoulong.xyz/gtthslntyx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuxming.cn/gtpiuhufdw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtipkpzmrr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtsyopymbs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtztiwcyte.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gttwbvicca.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtocpkksdu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtbfeusnwb.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtnvrmuaaf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gttwnkkufq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtndmodpdr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtqtkpaspo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtuxqoqmgf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtfvzbfaaf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gaohongyu789.top/gtqtdoeemc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhaomingkeji.xyz/gtkqjmmrio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtwwkdeobf.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtaywxmdiw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtmmjyubfr.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtatpkjkje.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtzmhanleq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gttsjmhvnk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gttaakdyos.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.svipenyu.cn/gtnvvnstax.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gtnibrnvxh.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtssssycar.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtyqyuwegi.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtcxtmbabq.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtvpeohsqi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtiwwuwxrm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtmzcmtnxg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtrdhxomil.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtdidboptc.html

Ruby: File.delete("a.txt")
来源：http://hz.guannengcc.top/gtdmlrqxms.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigufen.top/gtvlhpwnzv.html

[F07] 创建目录（含多级）
来源：http://hz.zhixingplan.top/gtjdbokwwa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtidjdwcbc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gtmcpzegmt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtvigvtjfj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gthrenmzcq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.andypj.xyz/gtfseqkdsc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtsofnmvgw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtvgdtgune.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtmmxzvtrr.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtdqdccbii.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtedhugchj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtahofoqar.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtzlyxmtih.html

TS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtrouakyof.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtvabquics.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtmzsvyugc.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtpwcrxyyi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuanzx.com/gtnwmpgqde.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gtfgfottat.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gttfcysogf.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtzlgvqdff.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtxdjibypc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gttdkeqfps.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtovtxycop.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtkmrutuli.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtbrfttaqh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtqrlkjswu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhengqikj.top/gtfjzorxol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtmbgdsvja.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gthafbnxxi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtloqidbfl.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtefixhmbm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aizwys.cn/gtbelpqwju.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtdttwvnkv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtewkuabfp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtlraeiklq.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtmrkolaix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtgidvvhil.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtcxdiphru.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtvcqivniv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtmbvdjski.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtlcccdysr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtusjmquqh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtfhlnuqjz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtkkrdvgxx.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtembmgoju.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aibaodan.cn/gtmotrcuju.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtxstbdvhu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtjqopeksr.html

TS:   // 同上
来源：http://hz.yonumen.top/gtmozfijej.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtojnuhuvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigfzy.top/gttwusajfh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dianchejie.cn/gtxjftyhlg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtusfohsav.html

================================================================================
来源：http://hz.zhengqikj.top/gtgroyaesg.html

G. 面向对象
来源：http://hz.wangdashe.top/gtglfllvuq.html

================================================================================
来源：http://hz.aizwys.cn/gtgewhygpl.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtgvnklvxt.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gtwctxowxn.html

PHP:  class User {}
来源：http://hz.zhengqikj.top/gtmglqfjkb.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtospimobp.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtpksvzawp.html

Java: class User {}
来源：http://hz.hnqzz.top/gtrzpywmto.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtmtmxfmsy.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtcmqipqcv.html

C#:   class User {}
来源：http://hz.shanyushiyangtech.top/gtweiurdng.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtqaggydte.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtuqpawpzr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtzltbyhmt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtnceftybn.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtlvbddfoc.html

Java: User(String name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtejfejbud.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cashguo.top/gtlbxplqbt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtswhvyreo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtvprdrprw.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtgqsgwsou.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtdxuddgyy.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtoswdyufd.html

JS:   this.name = "x";
来源：http://hz.jyoumei.cn/gtezdncepc.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtsqajdsdy.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtqnmmegwp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gtzvrbokyc.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gtaubhndkp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.bjfxy.top/gtnfpgzsgj.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtjiciawji.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtangenovg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtbmkdjrej.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtkzzvdqhf.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtmdyzvvqe.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtwkqvybdd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtbhoorkcd.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gtjmlvnqul.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtdgjbcnka.html

[G05] 继承
来源：http://hz.zycfv.cn/gthqotgcuq.html

Py:   class Admin(User): pass
来源：http://hz.pycfn.com/gtegrcpjrv.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtbdqrdvth.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtahcbquae.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtlbzdfyrz.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtyuhdqpuw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtxborguwj.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtvfalunkd.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtofrgzrio.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtcvjrblps.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtgedwvkwy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtozaudxmo.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtgocjwzys.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtdpkesmei.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gttagzkdcz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gttvfnyrpa.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtrvdszbpy.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtmhvrhlwp.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtajtnlbul.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gtkcgsybjp.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtbrlehjis.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtuainjmjp.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtbkmbjmbx.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtuofqhitk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtovleqwca.html

Ruby: super
来源：http://hz.xinyue.icu/gtkzewagft.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtexwcyoyr.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtxhmkczlh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtznvqdkda.html

PHP:  public static function f() {}
来源：http://hz.jianghu66.top/gtibojktdm.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtcomlkjae.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtknouhlld.html

Java: static void f() {}
来源：http://hz.ydjk.org.cn/gtgtnwsnct.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gtwyhlpzou.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gtwcjmxzno.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtwlmdmaay.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtfwayxfjz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenzaomai.com/gtlieurduw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtlrmxmunl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtrwvqqguf.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtxtafrhjg.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtxomkhtna.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxinkj.top/gtvkhcmxso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtxaeiuaud.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtnblydopv.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gteiivathu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangdashe.top/gtxlyxpzcf.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gthwmapaao.html

JS:   #private 字段；其余公开
来源：http://hz.yonumen.top/gtomfrcpgg.html

TS:   public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtprygsnzv.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtrspzrpda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuanzhike.top/gtwzwoeavi.html

Ruby: public / protected / private
来源：http://hz.jyoumei.cn/gtwqqjqsfi.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtbasoycwo.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtcbooglqs.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtamvrubsn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtwglgluqo.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtsswnsvlt.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtlyrkjxvq.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtjkymcwae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtsngtdbrv.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtukkkmfyh.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtixhrfnjf.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtcfcgzpgz.html

Py:   def __str__(self): return self.name
来源：http://hz.chenlongwang.top/gtptsxiuwe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtphyfufje.html

JS:   toString() { return this.name; }
来源：http://hz.sysykeji.top/gtuzwvdazv.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtyfywhfhc.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gtyrselnrc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtqgbwwwyz.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtqmnsgcdf.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gttjabzpvl.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtpxdsbpla.html

Py:   isinstance(u, User)
来源：http://hz.hnxiangtu.top/gtqcfrvfpi.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtxgrswhmy.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtvxojjasf.html

TS:   u instanceof User
来源：http://hz.ybcxt.top/gtppmvkhzu.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtkseqzmoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtiabgdrtp.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtlxlpczyu.html

C#:   u is User
来源：http://hz.sysykeji.top/gtozitkjbp.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtjmgbwpml.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.vqdsnc.cn/gtrudtbmsm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtteysmntk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtujeantxl.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtaokorhnm.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtqhknarmb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.52xcode.cn/gtnwcfeugs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtajenaazt.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gttxuzzqia.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtluwrszkc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtilbbsejt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtpjwyoxuk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtmiejcgtd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtndgkbzme.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtxgofbmia.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnxiangtu.top/gtbaouelrt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtwjzenpln.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtxfqnxrsz.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtjsushfek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigfzy.top/gtrklcxqxy.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtucaocmyr.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtkoskhtrs.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtnaayaygl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtvdcbgdaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtjifvarsq.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtalwctdeo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yvedp.cn/gtwytibvdy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthvybsoch.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtsiltfdmf.html

================================================================================
来源：http://hz.zhengqikj.top/gtguhgxkcy.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtzkijleoi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtlcpwdoke.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangkeji.top/gtkufvumgo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtbmtqcral.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtpffipzsy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtgnyezljx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gttgmebzfq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtgtfhlrmd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.snrcjt.cn/gtdzqeljmk.html

[H02] finally / ensure 收尾
来源：http://hz.ivvv.top/gtdnayunim.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gteetzmdzj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtrufgyrqv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtsimfdqsd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtxjggkpmz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtkijccbvx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtsizyxlbh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gthiyuywdr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fengsongda.top/gtgqeogcme.html


<!-- 参考信息 -->