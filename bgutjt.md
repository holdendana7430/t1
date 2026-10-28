代发 wailian999

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtcghjhirw.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtteaojies.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxuanxn.top/gtrqrqajte.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtrzpfkqob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtaepzddim.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtovkmmgft.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtjbxbwgzz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtrjxcbyla.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gttpfmhjnx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtvhyujnca.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zdqjudy.top/gtroxxprlv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gtfgldvlcs.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gthrlzxvei.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gtergcopjr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtzxpoyffx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtmslzqmma.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtxogkbvqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtybkxuvff.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtxkoqwcnw.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtxojwxjrz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtvkxpqvjk.html

================================================================================
来源：http://hz.fengsongda.top/gtvyyaaami.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtsjzwvzbb.html

================================================================================
来源：http://hz.yueranfly.top/gtvydgoaih.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtltuapjsq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtmtubtagg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtgjkbvzfe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtfhzmnrew.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tian-w.cn/gtfftupbas.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtueqpkcje.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.svipenyu.cn/gtpkwynzml.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtdaijfmrf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtleubacvn.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtpvtdouwn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aizwys.cn/gtsrlvpojx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtcmjiqhhq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtwsjaiunm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtyghmpovq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtvfrohsmy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtjbkhexks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sweek.top/gtxbzbslei.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtxnpiutas.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtnyjzcycd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtwnhfqkun.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtjoappajt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtpidedyxr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtnsxhnucy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtxqwdqxej.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtmckhxmgp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtpzrdmpzg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtmciogren.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtnhpuezzr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gttfveatfq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtzbxppndg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gteejgwwoo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtzihpejpt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hammf.cn/gtngvovenq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtkxtshzpl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtkzgdvbis.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtwbqmsiwn.html

[F05] 判断文件或目录是否存在
来源：http://hz.gaohongyu789.top/gtfwsjcyxx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gtuiqssenl.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtcqgnzqgm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtrjkxjbzs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtxaprhojl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtirmyjszh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtlxcxutda.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtenlwbzuo.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtxnvkhloe.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtclcqngxf.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtrkxfopbl.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtqamsufoo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtfowimlcp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtyiixzhes.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtctblvfsr.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtkpdtqvvp.html

Ruby: File.delete("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtfhiylwsz.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtodtnmkzw.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtftutolxr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtkjzraozk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtvpsmvxvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtrxsygmbs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtxwvjtckj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dianchejie.cn/gtznbeqakm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtvgganxcf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj202588.top/gtkhvmtpwn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gteejbjutz.html

[F08] 遍历目录
来源：http://hz.gogol.net.cn/gtawjhidyq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtxfjlqpyd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtauaibpng.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtxfwaxjbi.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtsemxutxf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtmqfjlzzc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtdiqfzmlx.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigufen.top/gtuqwjwhqx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gttnfjdzrf.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtledmjzqi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtysvnedze.html

PHP:  filesize("a.txt");
来源：http://hz.yanxiufei.cn/gtfgmiwjqt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtjgbdjras.html

TS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtatdworqk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtkzmnkvds.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtznwpddbz.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtconoyips.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtsmfuhutq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtnfvasjfx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtvpytaakr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gtkxrblelo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtflhtljpj.html

TS:   path.extname("a.txt")
来源：http://hz.hysaishi.cn/gtxeabdwwl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtjmpgksys.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtrlhigtlk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtvevheaty.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtncozosqz.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtyyaamfdt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtlxnghtvj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gttudqpdfs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtcovaxvya.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtxefxcppa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jianghu66.top/gtpkanwsyj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtmarymcxv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtcgbfbgzw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aizwys.cn/gtmydtmrwi.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gttlqybkbn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtjwaojdsn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sweek.top/gtlvaotari.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtdglxmgje.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtxbbrmdah.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtwembsxos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtupuauaeg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gttkjzqxbv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hammf.cn/gtmkyftpyf.html

================================================================================
来源：http://hz.jqgfzy.top/gtmuxnnabq.html

G. 面向对象
来源：http://hz.gzhubu.top/gtgumjwoei.html

================================================================================
来源：http://hz.hnxiangtu.top/gtootvmqtd.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtvzjtggpt.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtjcqypkea.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtljeeotrt.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtgohyqbsj.html

TS:   class User { name: string = ""; }
来源：http://hz.mhx1999.top/gtudgchrbi.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtueqymqbf.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtvtujochd.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtvacpsopb.html

C#:   class User {}
来源：http://hz.pengpengdd.cyou/gtobuzvava.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtwkhsakox.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gteujjqodn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dashuyun.cn/gtlmjwwhww.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtgsbangdx.html

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gtlzdyycsg.html

Java: User(String name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtrgbfnvkb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtxndzzukp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.meibo888.top/gtkrkefrzj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtyywuvbyz.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtxzsjuvrl.html

Py:   self.name = "x"
来源：http://hz.jlsjyb.cn/gtexsytwen.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtopzbqdst.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gtvymboaja.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtrvenffel.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtytojybfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gthraahhtk.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtdoiojqxo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gttwegcdnd.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtreshesss.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gtmrkhkjyj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtuhnyeyxr.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtoqmbmsnf.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtplbmnxoq.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtxvonfbje.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtmmcqgodz.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtazjpwqng.html

C#:   public string Greet() => Name;
来源：http://hz.zhijiandao.cn/gtwgenzqzw.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtyhqwyetd.html

Py:   class Admin(User): pass
来源：http://hz.yonumen.top/gttzdfdaqq.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gttuzfsdbt.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtlqkdddol.html

TS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtvxontvkc.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtopfqjlia.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aizwys.cn/gtynlmypjh.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gternskbuu.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtkvlzljag.html

[G06] 重写方法
来源：http://hz.gogol.net.cn/gtqvoqxdgr.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtqswfejpp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtkporgdul.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtvqcxkefv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtyguwxcje.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtdwfnfyfk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gtnxmcdcgd.html

Ruby: def greet; "admin"; end
来源：http://hz.yuxming.cn/gtpqfweltq.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtfgbkgoun.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtymxukrrv.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtdsmxaskl.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtwnmumhes.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtfpdowcee.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtvztlpdbj.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtseryktiz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtolxklofm.html

Ruby: super
来源：http://hz.redwolf501.top/gtnzuijtjc.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtfvbsgiei.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtyjtnskkf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gtqrmwbfzq.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtkntuhsym.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gthlezyysh.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtzhxpstec.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtpsziblgu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtpszzmhuu.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gtjuwpivkk.html

C#:   public static void F() {}
来源：http://hz.yj20258.top/gtiohbsqhm.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtaufiaicw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtxzioixvb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtadugveoo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yanxiufei.cn/gtgnkahhkx.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtqozmvhxp.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtrmjbusrr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtizfbvfre.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtnsypxypv.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtbmkpvefc.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtxbntlbkv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtvpudmban.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtwdvxzdby.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtlwrcxyaz.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtnhzkjfnm.html

Java: public / protected / private / 默认包级
来源：http://hz.nwbrower.top/gtkdofmmbp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtsqcymvfr.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtznkudgpa.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtlypnpmdd.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtsbwdibpz.html

Py:   @property 与 @x.setter
来源：http://hz.svipenyu.cn/gtpnuagnxe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtpelcupxt.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtqekrrjsf.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gticdbofzh.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gtxhnubkqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtxgqhtqba.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtppklqfyy.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangtech.top/gtayvbomup.html

[G12] 对象转字符串
来源：http://hz.ybcxt.top/gtdflypzty.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gtsabnhbcg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtyxetkrxq.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtmmlbpzxm.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtwhregzef.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtvdriduux.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cdnleiting.top/gtpcefldyx.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gthrclsrhp.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtictxrprw.html

[G13] 判断对象类型
来源：http://hz.xuanzx.com/gtbtmwivtx.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gteqvulsda.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gteamxdnrl.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtofvofwsh.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtfeytajna.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtmryafgki.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtvwjlsogj.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtvptfnfxm.html

C#:   u is User
来源：http://hz.smart0.xyz/gtpctljpsm.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtcjhznmdy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtippvbiak.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtbjnlvbpe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gtzsyopbsl.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtholyjjqi.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtzixthpbh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtbnapbvmj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtealhvwma.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtinmwwvgm.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtfjwttunc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtbuvcndug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtjczdttgw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gthbremkpd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtsnyvlckr.html

Java: enum Color { RED, GREEN }
来源：http://hz.tian-w.cn/gtotxuavtu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtzyixipnp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtxqeeviok.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtehyaybvq.html

[G16] 对象转数组 / 字典
来源：http://hz.aibaodan.cn/gtjyftlrkn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenlongwang.top/gtvkrixrpx.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtznkiknqw.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtechgjgcn.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtlobyttey.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangdashe.top/gtlfiznvuh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtpfdumppg.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gttcuyzgak.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jyoumei.cn/gtlzjbzopc.html

================================================================================
来源：http://hz.tanke756.top/gttlxhzmdl.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtgcxsxsmj.html

================================================================================
来源：http://hz.guowangkeji.top/gtrnypysiv.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtcjajefmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtwutdrxci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtmfiwhxih.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtelgdyhpl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtqddmgjjh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtqbbfoaej.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sweek.top/gtqnxyqhzl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daria6918.cn/gtozwkyhkg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigfzy.top/gtzerycvxn.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtshkvsdks.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtamiptvss.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtmhdxrzlq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtdhsdfrvw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtkxfkhkuh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtkassngof.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtwebhjrhw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtonjvvztf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtgnzrvdet.html


<!-- 参考信息 -->