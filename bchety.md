代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtdoepqror.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtwifygbul.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtujdnptbk.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenzaomai.com/gtawsxosio.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtpqegjvxe.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpaqjzkow.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtrdvjrcij.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpjktwhxz.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtnpjioynv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigfzy.top/gtfueyjhcd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtqlmtnozt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jyoumei.cn/gtyiuayeoh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtrfxojjwv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtuuhvmcwp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtndqbnlux.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gteiyztluj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtvviwyqya.html

[F02] 逐行读取文件
来源：http://hz.zhijiandao.cn/gtagmatgiw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtqxqfwgoq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtrbygheyb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtmhtobuof.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtdvzrrbaa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gthauhoxet.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtdcimejdv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtpmzqpmow.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtxkzaybob.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258.top/gtpiebdusw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtiuvkytaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtowrwfuju.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtzqwcsvex.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtvkkbqhew.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtbfdtjkyg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangtech.top/gtxsycevxb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtkioteenb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtpnbmcqla.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtjimttwtn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtftkedmfm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtrjuwbudu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtcjphwbap.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtaecuebps.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenjidiqi.icu/gtquudcpin.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtxahhhxbe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtffwbmnua.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtsvgfezgd.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtliqibwvp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtuaqpxbyz.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtlykdztua.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtweojmoys.html

TS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtnsryekgh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtzmalequb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtriffckam.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtzrbpkpfj.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtjyxjtgxk.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtqwvtdrar.html

Py:   os.remove("a.txt")
来源：http://hz.sweek.top/gtbzxcgotf.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtzebewsch.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gteqiiaxfm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtpocbmcbv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtiqufpnrs.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtvxcfhqlg.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtfzizcjzc.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gtzxwwothi.html

[F07] 创建目录（含多级）
来源：http://hz.pycfn.com/gthgilduxf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sxryk.cn/gtursjsoyt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtsuqscryu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtazufofvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtsxaafbpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gteyvzxkkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtniikhjmv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gthiyaeadv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtrttrpkse.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtjpzbvsvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtchedddxu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gogol.net.cn/gtepsibotg.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtaxvglqwa.html

TS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtbtahhvix.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtkqbsqasi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtngaovkkh.html

Ruby: Dir.children("dir")
来源：http://hz.yvedp.cn/gtpingunif.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtqlndvjal.html

[F09] 获取文件大小
来源：http://hz.xziqi.cn/gtagmfecmp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gttzfyntqb.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtwuntmucy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtkhqreobz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtsmdxzdnt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtqqgdldsq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtkykodafz.html

Ruby: File.size("a.txt")
来源：http://hz.jqgufenzy.top/gtrayvciea.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtzxhbptuk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtmsbwhrqp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtxopmtibt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gttmbmhyrg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtihdjauew.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gtxupeiaaw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtgwwxiczs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtowsmumxg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtnivzutwa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.316326.xyz/gtmizynneq.html

[F11] 复制与移动文件
来源：http://hz.wangdashe.top/gtndptfkrw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtqzhqairs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xylfe.cn/gttqzrnrso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtfpiqjpsu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtwthltahc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuxming.cn/gtwlfqyhsp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtnchkjziq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtlykyubhs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtrmcinbet.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtjykdqkfz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtpbxauxrq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.vqdsnc.cn/gtpllovkbz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gthodqccwk.html

TS:   // 同上
来源：http://hz.meibo888.top/gtodonnhto.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.vqdsnc.cn/gtwclyiwja.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.52xcode.cn/gtbconkqrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtbmlgxszw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtjyddzguw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtigkgwdns.html

G. 面向对象
来源：http://hz.hnqzz.top/gtaofurznu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtupwwvjkz.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gtbhfskhav.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtljszwdob.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtgmwtmzhp.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtiwgazkiw.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtfpnvekmd.html

Java: class User {}
来源：http://hz.aizwys.cn/gtwddknofa.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtaqtumuht.html

Ruby: class User; end
来源：http://hz.svipenyu.cn/gtrxovzngj.html

C#:   class User {}
来源：http://hz.cashguo.top/gtzjkrwcxn.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gtuzhudlge.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtdvivzgei.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shuidangran.top/gtqflmlubj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtbrccxgee.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtpywlldtz.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtddriigef.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtajhhzfcl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtmfqwgvhh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtcvmbirfv.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtvhjzxwxm.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gtugfipkat.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gtcgbvrloe.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gturcmjhmv.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gthchnvhti.html

Java: private String name;
来源：http://hz.xuanzx.com/gtfmcyrfir.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtdpipewqp.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtvdtvrzje.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtlxrofwfw.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gtzsgpdxjp.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtkyyfjnvk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtuhlmryvk.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtlhqefntl.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtwicmfdqh.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtfuutdhut.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.snrcjt.cn/gtperlbnvr.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtmaqkcyhs.html

C#:   public string Greet() => Name;
来源：http://hz.chenlongwang.top/gtfguhmjpo.html

[G05] 继承
来源：http://hz.yueranfly.top/gtrggtdrmm.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtckocudoy.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtgtgttxon.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtvriwtegc.html

TS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtktxglzil.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtliqkkwcp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtoscuygib.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtqryxokbp.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gthbbjotbn.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtvuqqosyo.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtttbvsvbn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtruskfqwt.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtbdtcvzrj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtddjjptoq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtnvhfcynu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtzttwnafb.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtowfoxmgv.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtehqbybwa.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gthezntkab.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtnpaursqc.html

PHP:  parent::greet();
来源：http://hz.jqgfzy.top/gtribvbxte.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtfvhpjxvx.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtrqoznknn.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtcsmaxozv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtiurdoakh.html

Ruby: super
来源：http://hz.9152youxi.cn/gtojohguxm.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtzitualqz.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtpmflrqzk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtdxiqzgwf.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gthgmgiugu.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtutopzkwi.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gtkoruoevt.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtpvbabtqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtgfykrypz.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtnyhrcdqc.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtjdnocbyj.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtnsfmpfwr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgufenzy.top/gtxhhojupw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtuzldddur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtetbfzcsf.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangdashe.top/gtjtyrkbtu.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gtgudiwswf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gturrzwbfd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guannengcc.top/gthvfyzqex.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtsjtznppc.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtttsqsaap.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtojwdcnee.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtbjtnqzia.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtvpyzhfsd.html

TS:   public / protected / private
来源：http://hz.sysykeji.top/gtngdobtgf.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtubnnxhxv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtmwyshdqg.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtxkemnrmi.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtxuhnxprd.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtiasxcvga.html

Py:   @property 与 @x.setter
来源：http://hz.52xcode.cn/gttspxpvgr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtqkdjjbyg.html

JS:   get name() { return this._name; }
来源：http://hz.pycfn.com/gtcsqhvgon.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtmxbnygsb.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtnguxvnax.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtjuqxhfrn.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtgdknztut.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtudtkoccq.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtddgkumxv.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtfixjktdz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtbqazvhjl.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtxaynxdsj.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtvedhhhig.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gthjlrqhur.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtfzonursp.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtmgqdazzh.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtngixzlvk.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gthymvsmwj.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtvntwqhil.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtjddzmbyh.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtxjogljhq.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtroerhrvw.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gthctfijgp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtlksxzonk.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtwttantjz.html

C#:   u is User
来源：http://hz.xziqi.cn/gtlnnnmnyd.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gtkkteldag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sweek.top/gtodrmorfk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj202588.top/gtirlnfwlr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ehwqpu.com/gtuqpsrnau.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtizazicyr.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtityoqtkd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sweek.top/gtchbpzsvs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gtvdchvdwp.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtrkqktqyo.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtqpqaalvf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtzckffagv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtnobnofdw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daxiang520.top/gtaorhfmgy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtfhaydovu.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtsokyexlu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daria6918.cn/gtlhytmmni.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtkeoofquz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtstauurvw.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtfpzkipcu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigfzy.top/gtgmxyyscp.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtdasanesn.html

JS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtskdalclh.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtirldkxek.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtuafvaozw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtagxkadls.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gttsgzonmq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtodusdsza.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcqbvpvcy.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtpfsryurk.html

================================================================================
来源：http://hz.vqdsnc.cn/gthxtgtflq.html

[H01] try / catch 基础
来源：http://hz.zycfv.cn/gtollqocdv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnqzz.top/gtaffxuxxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtpywdqxwd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gttgqabytp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtruqjpuhh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yanxiufei.cn/gtvxpiekgs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gtgzsnfzuj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtzqboyfle.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pycfn.com/gtsyjcgwmn.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtlmlukwmz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtonoizswg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtyonzygvd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtsynsdfxe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gthidtdput.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtqifgxzuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtzgcxsqnh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtmaqhqgph.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtwmqgxluk.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtubqfqsam.html

Py:   raise ValueError("错误信息")
来源：http://hz.haohaochexian.top/gtsuqwwwde.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gttwjfctfg.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtnxnrckqz.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtupdfaoxz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtzveowaif.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pycfn.com/gtftkedtzv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtfwudxihp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtanhakqmn.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gtyqlmqzgf.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtutcszvin.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtbzujkpoz.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtnmgwrftw.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtrgwjbmqu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtyvtdrgaf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtdgjvuicu.html


<!-- 参考信息 -->