代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtokxvmvmq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtkddfijuv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtcdsawoon.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gthmfakdbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtccjlmdzu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtvqmwfgcs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtbdidpspx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtdehosudp.html

[E22] 字节长度与字符长度
来源：http://hz.hnxiangtu.top/gtcxqrkjqu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtqvuqhcge.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtpopbwvje.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gteyzkbape.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtjdahysoq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtplvjzlqm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gogol.net.cn/gtdwschbev.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtqayszlce.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtbratrmby.html

================================================================================
来源：http://hz.yuanzhike.top/gtypuujbua.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtvjxgpsws.html

================================================================================
来源：http://hz.daria6918.cn/gthowphpvf.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtemnbqezj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtmmllskic.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cucudq.cn/gtahcghskg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gtxchretyj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtfxsnujqf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtdjpkkogn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtxhecigbe.html

Ruby: File.read("a.txt")
来源：http://hz.kuanghao11.cn/gtearinman.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtbxedhcju.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtvpwzuwug.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cqqwz.cn/gtoaazfodz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtrrcfzwlz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtwoshrznh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtumxpxvsy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtrpdooxpk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtcegwiycv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gttmdmwffy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtnksiutwg.html

[F03] 写入文件（覆盖）
来源：http://hz.gaohongyu789.top/gttmwsrmkb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gaohongyu789.top/gtsehphwzr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ivvv.top/gtjrproybv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtyzomhiap.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtsxnnegeu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtauteudgx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtvebdmmdg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtndhvbxjw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtnrfmspqg.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtsmgqdnrd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sufxvd.cn/gtbuqaectp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gtzqppjayo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtymincvlk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtcwnvoprh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtiudltavo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtmwgrmfxy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gthjjnuzrx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtduccjcpj.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtnuwnlesk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cheryme.top/gtngsqrimp.html

PHP:  file_exists("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtzroqzhtd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenlongwang.top/gtukjjeyov.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtbzwaifdm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtwoznrtxb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gtkrewlgph.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtpnmjzmif.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtygzacewg.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtluflvlvn.html

Py:   os.remove("a.txt")
来源：http://hz.jinghuilouyu.cn/gtyzhphehd.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtzlummbee.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtrjqhbaiw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtdjzodvtc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtzxsoadns.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gtabhjklvb.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtodtibsjb.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtgztyruzn.html

[F07] 创建目录（含多级）
来源：http://hz.yanxiufei.cn/gteikkrkqh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtghukmyou.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gtzkgaylrd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtcoonlend.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtmnwvlquk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtygcbycaz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtwvpidoki.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aibaodan.cn/gtupdwwarm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gtfgbbkzzz.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtlfamskvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtaliheyel.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtroicjrth.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtwbpyopxs.html

TS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtjhhgbklr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtfpyilxny.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtdaweytto.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gtmnvaohpl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gtynkgcpmq.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtnexzqvly.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtkgsxjera.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtuhfljvnb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtfakepydc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gthlpbipdn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtdwurccbw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtjadsghia.html

Ruby: File.size("a.txt")
来源：http://hz.hywenlv.cn/gtdlkpcksu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtrrewtqlm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtxpvficwf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtyuybhrnr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtryidvxcg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtnugyfdbq.html

TS:   path.extname("a.txt")
来源：http://hz.tanke756.top/gtqjaxshao.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cashguo.top/gtqzmpradq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtldejtkat.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtnafmnlru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtmwecmqap.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtowdehzmm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtumaetmaz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtlcozruis.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtgpuspjtl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtzgzddcsv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtlzljkrme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtakavstjw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtvncyqrdv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtazspvlcl.html

[F12] CSV 读写
来源：http://hz.vqdsnc.cn/gtryxfijcd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.havefunace.top/gtudpmcgun.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtmqwdmfng.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigfzy.top/gtvmkrfrdd.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtsnuuhrvj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.kuanghao11.cn/gtabqaptvw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtbeklvcvl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtinwnvgjc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.mhx1999.top/gtgvuymyll.html

================================================================================
来源：http://hz.hfpthk.cn/gtrslukbvf.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtvmibnzwc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtisbhxehr.html

[G01] 定义类
来源：http://hz.yongpay.top/gtiwfccoar.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gteyahlhxq.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gtvzhcgiis.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtlxrmifbl.html

TS:   class User { name: string = ""; }
来源：http://hz.ehwqpu.com/gtjcxxfinp.html

Java: class User {}
来源：http://hz.ywan-chungtsiang.top/gtzmrphpkz.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gthdiqxvzl.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtepvyiwgh.html

C#:   class User {}
来源：http://hz.xuanzx.com/gticdqksbt.html

[G02] 构造函数
来源：http://hz.sweek.top/gtuyrqwbqb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtfwnusyry.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xingfuxueyuan.xyz/gtutlrwifl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtrcxftlso.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtqhzxuamf.html

Java: User(String name) { this.name = name; }
来源：http://hz.bjfxy.top/gtzvwespmg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.birdmap.top/gtfovzcjbr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtgqxkgypg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtfmbukbbq.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtsadnwnia.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtebopiicr.html

PHP:  public string $name = "x";
来源：http://hz.smart0.xyz/gtlrhqpkmv.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gthzxrzgcv.html

TS:   name: string = "x";
来源：http://hz.snrcjt.cn/gtemclkgvz.html

Java: private String name;
来源：http://hz.zhengqikj.top/gtulckoezr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtlfvhxwyf.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtbjbhqfmv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtpjcekksu.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtvacmbuuu.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtpphppfuh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtnyccnvux.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtoxawfkyw.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtskdmbmnz.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gthnreipsm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtjfzijdjo.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtiqgwoevs.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtljhxvvdo.html

[G05] 继承
来源：http://hz.smart0.xyz/gtiiesdowu.html

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtxnarwkle.html

PHP:  class Admin extends User {}
来源：http://hz.snrcjt.cn/gtrbhsmhbc.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtfavhdtkb.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtsgvydmfu.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtbwvqrwsw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtiqyowqmy.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtcqzhprhe.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtqczujkaa.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtrtkxxant.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtxbmmtppz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtshgtcyfw.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtgartikee.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gttaevrbip.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtkfcjyfsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtnlkgyqzt.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtwgnpldzc.html

C#:   public override string Greet() => "admin";
来源：http://hz.gogol.net.cn/gthtjkyyhn.html

[G07] 调用父类方法
来源：http://hz.jianghu66.top/gtglvduelj.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtzbjzzyan.html

PHP:  parent::greet();
来源：http://hz.0kj1m.cn/gtwosoetfb.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtnergzfdd.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtlhewjvoa.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtqywxzsjk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtczzcqyay.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtmwaxnmem.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gtoqzvmlss.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtwszqfwol.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jiagoushi.top/gtxkmbgccy.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtumzvitai.html

JS:   static f() {}
来源：http://hz.cdnleiting.top/gtlyiikdig.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtaytdderd.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtupixblxp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtegeoyuuw.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtvgsheshp.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtayaitdlt.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtnnjbaslx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtsistjinv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtpykmwjjz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtmhlrxbhz.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtorbopuqs.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gteaskjhob.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtkcsrzrup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtwkongdcc.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtlvrkqtvd.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtfxgznynf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtxmysdawt.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtguimbnvy.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtygxfcazs.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtaeaqfegk.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtkrlgzdoa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.meibo888.top/gtednykowm.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtlnyhooap.html

C#:   public / protected / private / internal
来源：http://hz.ppjwa.cn/gtxeembarp.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtvokvvanr.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtjnmmjqdi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtillvvzyc.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtofktykfy.html

TS:   get name(): string { return this._name; }
来源：http://hz.cqqwz.cn/gtmxozcwwl.html

Java: public String getName() { return name; }
来源：http://hz.hywenlv.cn/gteqsbjiev.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtbsdgxbwq.html

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtjbvefnby.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtvodmgkzo.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtueeioeci.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtnbmgetfd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtydlsqwyf.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtgkrfniyg.html

TS:   toString(): string { return this.name; }
来源：http://hz.fzhhl.top/gtfymaszqy.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtenrdbyuq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtezyaibft.html

Ruby: def to_s; @name; end
来源：http://hz.yangfankeji.com/gtefgwyekp.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gterbpcoik.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gthmbpcpbz.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtzcgofcfj.html

PHP:  $u instanceof User
来源：http://hz.daria6918.cn/gtfuwspcvd.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtiqhxuoho.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtmzfjnrhw.html

Java: u instanceof User
来源：http://hz.zdqjudy.top/gtldwcbmhl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtwvyryxzj.html

Ruby: u.is_a?(User)
来源：http://hz.xylfe.cn/gtymnbpxdp.html

C#:   u is User
来源：http://hz.meibo888.top/gtnssulelz.html

[G14] 数据类 / record
来源：http://hz.yangfankeji.com/gtqkioklrs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtrhucovur.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtcwxwyihs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtspwhpedy.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtmpihhqir.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtsxbhzrtm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhiwuduotai.top/gtcphxkvkd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtrsvurihu.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtxslidrtj.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtejgrkzqd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtulfeeccp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtktaxnupm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ppjwa.cn/gtgemxpmjo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtclohopjf.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtengidizh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtgswgzpbe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtnapvcprr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gttluonqrj.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtbnxuftft.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtwhsuxogn.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtowpoyeaw.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtkrzrlerz.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtdfduczbv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtmtiwkyaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtzjddrlnd.html

Ruby: obj.instance_variables
来源：http://hz.guannengcc.top/gtwxgorcut.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtnqzkjgrs.html

================================================================================
来源：http://hz.gzhubu.top/gtiwtclorc.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtprombgaf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnrvmrlxs.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtntscywmy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gttdtwugaw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gtejwekulk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtqmxriuaa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtrxrkimgv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtlhqeiuww.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtvwrfdqan.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuetiantiany.cn/gtzrcakfzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtcabgcudp.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtckvuzcfr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gteurzpgcc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtttpvvxhv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtmfjuuntb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtsvemrffb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtcecgsnvc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtqfeviscr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtrsvdjzqr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtekiarohp.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtrjzyqnys.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gthqqyrrmk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtpwkltkxu.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtlhxuvvin.html


<!-- 参考信息 -->