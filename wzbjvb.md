代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.feifeiyinyue.top/gthnqbfqrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangdashe.top/gtyzqdvqcd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtzqgjtxzi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gthuallhjl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtkrenhwix.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtszwfxwjz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtgrjqdshv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtdbdnwfnn.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gttvelqqkv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtpvqgaaiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtnkyhuntv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtkzqqjwea.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtgfzilhkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tian-w.cn/gtfarahvqy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jiagoushi.top/gtqnozfugr.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtikisrewx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtcjnvnbrd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzqxwopxm.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtskouxcsc.html

================================================================================
来源：http://hz.gotoacloud.top/gtcybctzay.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtffdelqki.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtamunsobc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtomyjylqg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtcekppunm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zycfv.cn/gtslshiszq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtsykpvsdo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtzbkkjamy.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtitfsrgdm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jiagoushi.top/gtqlvqjeon.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtwzibkjjg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtqqgbypsl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtydvfwuyr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtlujomidl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtutmkyxyk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtrmxqhzxi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gteytbuohg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gtyhbowkdg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtoozdgxgi.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gtnsunymxa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtetxgbttj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtpmgzrmak.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtcuzfaloc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtcodbthkk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnxiangtu.top/gtsthfwaaq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangshuangyany.cn/gtstlbwuql.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtpmroanwd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zycfv.cn/gtlchrbfbo.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtdmvpmgoj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtvxpczjfg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtaacbzsnq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtvnzsqidq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtusmbiesu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtujcmbgtu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ppjwa.cn/gtspahtmsn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtaibswiak.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cqqwz.cn/gtjpadbelc.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gtxyyldqgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtaxchzehe.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtuicnqauc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtdcxjgalx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtgpahkvda.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtrrckgwbu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gtszqrxakz.html

Ruby: File.exist?("a.txt")
来源：http://hz.aizwys.cn/gteuzbdtrt.html

C#:   File.Exists("a.txt")
来源：http://hz.hnxiangtu.top/gtbooiuzai.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gthtpmjozx.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtpfwqoolh.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtwsdfehdx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtzxdrybug.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtlkczietr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtblyxavix.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtfnjiindp.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gtahlccjvs.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtjlhhitsw.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtmxdfotpy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtbdvienjp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gtrqcyvmbu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtdujmtbwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtqvzabhyk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gtpdoebhvk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gthyiykuqm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtdwjrjnip.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gtvkooflhy.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gttozvlkas.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtucwujqqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtchkczuno.html

JS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtaslanxbg.html

TS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtfxeczsaj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtyndjqdrq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtjklhbgyx.html

Ruby: Dir.children("dir")
来源：http://hz.ivvv.top/gtzdwxyjju.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtvkragjcg.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtxdikcjko.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtnaqmcxdz.html

PHP:  filesize("a.txt");
来源：http://hz.havefunace.top/gtsouyclha.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtxnxcvrqh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtygvanaho.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gthgsflzml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtumsadtxv.html

Ruby: File.size("a.txt")
来源：http://hz.pengpengdd.cyou/gtkucqhwsh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gotoacloud.top/gtjwcgesjy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.mhx1999.top/gtjvgldpmf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbwzpvaqp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.andypj.xyz/gtlnhedjcf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtzqqojguc.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gtwonnszmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtpjcaahxs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtdteakeum.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtwejfnyoi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuxming.cn/gtenxvdkbw.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gthnnshwmb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtjfklsrqo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtnzmdbmhy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtbgbxuchx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtmkbsvain.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtlmpwgwie.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtljqbvdct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtqahtgvfm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtlakuaozg.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtkoghydii.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gtreggvecl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dianchejie.cn/gtzheipesg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gtzysamvho.html

TS:   // 同上
来源：http://hz.pycfn.com/gtvuklkaid.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtljkuiaoo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtqjeccebp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtzxdvofkj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.kuanghao11.cn/gtflnvdjfj.html

================================================================================
来源：http://hz.birdmap.top/gtsjiebcmj.html

G. 面向对象
来源：http://hz.nwbrower.top/gtdymghetb.html

================================================================================
来源：http://hz.redwolf501.top/gtpjhnoeyu.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtnyasgxsw.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gtemzorfdl.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gtukpnuqkt.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtlbllrrrt.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtfbjhfgfs.html

Java: class User {}
来源：http://hz.sysykeji.top/gtayjaxkhb.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gtishblloq.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtylvylppm.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtuohaxrcp.html

[G02] 构造函数
来源：http://hz.sysykeji.top/gtmlzqhhbe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtgroreflr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jianghu66.top/gtqaxcxdjq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtiatckjie.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtzpuvpnek.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtmlaukxar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtucvesntq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gtvsyytjrh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.smart0.xyz/gtgpsgnchd.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtndymrwiw.html

Py:   self.name = "x"
来源：http://hz.316326.xyz/gtwrakixgd.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtweeqjmko.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtedvjvgpe.html

TS:   name: string = "x";
来源：http://hz.gaohongyu789.top/gtpqbdmewa.html

Java: private String name;
来源：http://hz.iojbl.cn/gtrchlnmho.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtwskzobpf.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtewpsejig.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtnhrrxbwl.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtvcfcufij.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtbfukkroy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtdmcybkhs.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtvvujtuxe.html

TS:   greet(): string { return this.name; }
来源：http://hz.fengsongda.top/gtjfjastlo.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtigewjqkw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xziqi.cn/gtafregimk.html

Ruby: def greet; @name; end
来源：http://hz.hfpthk.cn/gtukhkzoxw.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtrzxkjrdk.html

[G05] 继承
来源：http://hz.cqqwz.cn/gtjhsanmyv.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtbiruldgz.html

PHP:  class Admin extends User {}
来源：http://hz.ivvv.top/gtbmypqwox.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtckltvvby.html

TS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gturnnpxpk.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtmxrkfato.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gtubciyboe.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtakkzxhmi.html

C#:   class Admin : User {}
来源：http://hz.redwolf501.top/gtbxjrfcys.html

[G06] 重写方法
来源：http://hz.52xcode.cn/gtdciiwqcw.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtkwuiqhmo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtgnfulkxg.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtpbdxlcrk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtjnuhdyjt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtcumdwopf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtgrtwdast.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtghuvgqah.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtszhppjtf.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtddnqrpzf.html

Py:   super().greet()
来源：http://hz.jianghu66.top/gtvnwxoghp.html

PHP:  parent::greet();
来源：http://hz.fzhhl.top/gtfuzfiipy.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtptydauxw.html

TS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtkpumrsqo.html

Java: super.greet();
来源：http://hz.sweek.top/gtwaulespp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtsxumwrhl.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtmnzyzvkv.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtgnwvmtmm.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gttgdufomg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtosaojwuc.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtgfrqxagk.html

JS:   static f() {}
来源：http://hz.vqdsnc.cn/gtcyiikczs.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtcdotbldk.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtggnmfgdg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gtcrwsjisj.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gttgcyrlqd.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtkhohkrtx.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtuukaczrm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtmusqlpks.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gttlflzocs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtrtsejfnc.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtnvuqyrjx.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtaynupwba.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtxlysckxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtnwtezlct.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtwnnwfwjd.html

[G10] 访问控制
来源：http://hz.sweek.top/gtmzozoizt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gtcrqdvnea.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gturifclra.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtnydfllka.html

TS:   public / protected / private
来源：http://hz.gzhubu.top/gtrlnhrxkv.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtvzufwutv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtecnvtnuj.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gtibujijqn.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtwxbvmpkl.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtubximzvw.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gtumvesleh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtiyxtgioz.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gtmfbelefq.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtwvbztghw.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtkjawrhko.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtikdyzukt.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtzshwauey.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gtrsixvsfw.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtdecvugvc.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtsrvhxcpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtxpovwgoq.html

JS:   toString() { return this.name; }
来源：http://hz.pengpengdd.cyou/gttlaoezhx.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtajajugeq.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gthccnshhy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258888.top/gtjrebknaq.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtinbznkqk.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtmlzvjnja.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtoelhyofz.html

Py:   isinstance(u, User)
来源：http://hz.zhaomingkeji.xyz/gtyvknkoeo.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtvkwbmmcd.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtibhjzqui.html

TS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtisncique.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtbwyohrie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtnbbrfzzl.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtpdbhtzhc.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtjggsipna.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gttzrclhuk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtftzbubem.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtvrpbfzrg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtptoinbji.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gtwibwdhex.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtphydipuy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtpaabkzck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtxrsrfoyd.html

C#:   record User(string Name, int Age);
来源：http://hz.zhiwuduotai.top/gtzsvagxoo.html

[G15] 枚举
来源：http://hz.tanke756.top/gtytigdswp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sufxvd.cn/gtlregngby.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cucudq.cn/gtkvbwoorn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dashuyun.cn/gtyilrwugt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtxmjpmqyy.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtzbvzrdob.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtmlwtijej.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtrxfoygey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtrfozptxu.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgufenzy.top/gtkftzafew.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtduzuiiet.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtfuahhadc.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtsgwrtgrq.html

TS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtbbcblbzw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtticgxwad.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtocczlviv.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gtpawowyot.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gtwnrazeis.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrjdobnpj.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtzyqhnhho.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtyqdmwean.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtcqwgxsex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtrtlztxia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtcswreuyl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtossitakh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtdakyihcf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gttmkllhhw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtdtngkulz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtmmcrwkwq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.snrcjt.cn/gtjwqyuzsi.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtjjrlsvsv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtjdxohvvy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gthnmexgsu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtradkjkzu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtuhcbqibb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtpgtjibxk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cashguo.top/gthgpcrcfc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.havefunace.top/gtffoheflo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gttlagvvbw.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtqjwwlyir.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtvdgixime.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtomtixbdj.html

JS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtyqrxzoiw.html


<!-- 参考信息 -->