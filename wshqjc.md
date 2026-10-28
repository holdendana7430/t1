代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtrutxhrhz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.haohaochexian.top/gttjcceihb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jyoumei.cn/gttqbujsby.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtykhqszuk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ppjwa.cn/gtdimncgoh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxsblcrzp.html

F. 文件与目录
来源：http://hz.tianlin.xyz/gtfuwiywda.html

================================================================================
来源：http://hz.fzhhl.top/gtejnwlibd.html

[F01] 读取整个文件
来源：http://hz.zhengqikj.top/gtueltzkol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnqzz.top/gtrnrqvlgo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtznffaygk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dashuyun.cn/gtqoytzxoi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtqjbdyowc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtclpymokl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtubkkxaam.html

Ruby: File.read("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtgxrohqjs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtdpeerprg.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtzuuxbrcs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtbqlffekc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtnzhjdzxg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtylxcpcpg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtgvthcimi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gttuefmgrr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtwwvmfxgu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtdxmehjok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtquyzuimm.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtekjpyrxj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtvvdilyvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtzoudeptz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gthzhlwxnt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtijdhriwq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtsrkhxhiz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gtsflpqfmq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtmnrxsjmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtkidsnffx.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtiovlqhdf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtzuhavihd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gttjudmeii.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtawmrloma.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtmzwbzuno.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtjdqshnrd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gttyjrnplf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinyuanbaomall.cn/gtmbletmhc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtltdwrpwr.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtinsmorse.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gttmqbokwr.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtaaluvpke.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtzgnzkoik.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtufujuugg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtiuzyxtvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtmwnoaivd.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gttsjzeijg.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gtmumzpncb.html

[F06] 删除文件
来源：http://hz.gogol.net.cn/gttomfgfkp.html

Py:   os.remove("a.txt")
来源：http://hz.snrcjt.cn/gtjrrogmyt.html

PHP:  unlink("a.txt");
来源：http://hz.hnxiangtu.top/gttggvpfoc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtjwxxnwvq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtjryhpgvc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtijcwrtgv.html

Go:   os.Remove("a.txt")
来源：http://hz.meibo888.top/gtjcbozfne.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtrrrssrlu.html

C#:   File.Delete("a.txt");
来源：http://hz.zhixingplan.top/gtynxjqydx.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtaspggfhy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtjyaxueps.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gttijtnkkf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtjhnqdkfi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gthpudawbq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gttadozbjv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtqvpbgugd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtukwqsket.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtuxycanng.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtwgbsuoto.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtnwopnqkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gtvtybzggt.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtqyeyimef.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gttdfhywun.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtkzxufhnf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gtppbnxjve.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtczxljjue.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtifglhzhp.html

[F09] 获取文件大小
来源：http://hz.pengpengdd.cyou/gtxymglpcz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtxxvcepdf.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtnkjthrzn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gthboonxhu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtkvswpgud.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gthkmbamwm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtrdexpkzc.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtkrlopibs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtuiivquqf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gthngrsern.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtjonoawyi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtbiylqwhc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gteqvkdrsl.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtxjnuhouu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtanmccrfi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtzjjllxtg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtwiwixixu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtrvpxttho.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtuawonygp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtgkfhcwxa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtkohantih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtraoofpok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtjgwymttt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtebeaucee.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtfhjnuhuu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtccfdrewh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daxiang520.top/gtxutqlonl.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtgbaimgwl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtlskwdgmj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.svipenyu.cn/gthdhxrjjy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtxrkocjey.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gturryyuty.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yongpay.top/gtddqjpssj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangshuangyany.cn/gtdrcrzwho.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtbtgwunwd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtsdsqocpk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyklkuvir.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtvnsrvfln.html

================================================================================
来源：http://hz.yanxiufei.cn/gtubvtubwc.html

[G01] 定义类
来源：http://hz.meibo888.top/gttbzfqotw.html

Py:   class User: pass
来源：http://hz.chenzaomai.com/gtugcketgw.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtvuszwwai.html

JS:   class User {}
来源：http://hz.meibo888.top/gtddcmdivx.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtzkxpusqg.html

Java: class User {}
来源：http://hz.yuxming.cn/gtjktugzzh.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtyndpqybp.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gttdxhxnja.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtpuwcfzlb.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtcwlyrhyu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtmdgjuwvb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtjgofnokb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtddnfaypv.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gtgjfbqvoa.html

Java: User(String name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtmmcsfoxn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtfmimsicw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jiagoushi.top/gttuiwxsif.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtjfzdzylo.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtbxffsevi.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtakzclogo.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gttkruogbi.html

JS:   this.name = "x";
来源：http://hz.birdmap.top/gtxkablbgb.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtkadlelxs.html

Java: private String name;
来源：http://hz.jinqigfzy.top/gtxtzeobvg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtcpkormrc.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtlnkppnzd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtubjncbho.html

[G04] 定义方法
来源：http://hz.yuanzhike.top/gtkquymlqv.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtotbfxtrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtactqrvoj.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gteyvykxmi.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtqtxxnbvr.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gthmotbkor.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gttftucppf.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtidwjrkog.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtgolabpwe.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtbzuwbqii.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtrrdoohvk.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtkmhetosi.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtqqoqhyef.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtvnywziur.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtrwzewejz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtjmyxratg.html

Ruby: class Admin < User; end
来源：http://hz.mhx1999.top/gtompjtwpo.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gtjnfjzklg.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtvkldqfoz.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtcqwldghp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtfgjbntwx.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtqhpsjdwx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtwjrvfsnw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtitdywgaz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtniccijge.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtzzywjyse.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtycyvufuh.html

[G07] 调用父类方法
来源：http://hz.chenlongwang.top/gtilphappn.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtmjemkmxo.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtfjoiwceh.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtbdlogkkj.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtfjpucoyj.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtiwvadjqz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtqwveeqlm.html

Ruby: super
来源：http://hz.smart0.xyz/gtrfcvdkav.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtsxbmvddt.html

[G08] 静态方法与属性
来源：http://hz.xuanzx.com/gtztyzegup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtxgkuhwcd.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtzwywwfoa.html

JS:   static f() {}
来源：http://hz.sysykeji.top/gtcrgzrpxa.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtgpkuorvl.html

Java: static void f() {}
来源：http://hz.jqgfzy.top/gtqjkyxafr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtxuatzmtl.html

Ruby: def self.f; end
来源：http://hz.0kj1m.cn/gtpirwkbtb.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtcsfpwydp.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtmhfkueno.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtvrzhporu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtctzqrcyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtghbeedvx.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtbapanrxs.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtstrdbovw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtbyjhsfzl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtlkwjmwrd.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtcuvgaptk.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtdhlxuxsa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gthntodgjj.html

PHP:  public / protected / private
来源：http://hz.jiagoushi.top/gtmxkuvscr.html

JS:   #private 字段；其余公开
来源：http://hz.pengpengdd.cyou/gtkikwxirs.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtkpwushre.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtwncinxlk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtxxqmnmiv.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtgnslbzrq.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtqxmdceix.html

[G11] getter / setter
来源：http://hz.ybcxt.top/gttlxrrvov.html

Py:   @property 与 @x.setter
来源：http://hz.svipenyu.cn/gtpryyxsix.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yongpay.top/gtgdoyfgmk.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtohbqmeaz.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtleopansl.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gthvdclxah.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj202588.top/gthysacmlu.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gthxsnfjva.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtovgryauu.html

[G12] 对象转字符串
来源：http://hz.jlsjyb.cn/gtkbaknmvo.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtdwgmuvyi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtnoxdlyry.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtxbwbtifk.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtryklscbb.html

Java: @Override public String toString() { return name; }
来源：http://hz.havefunace.top/gtnieezbsu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gtaksfjhfk.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtmjnxtfwv.html

C#:   public override string ToString() => Name;
来源：http://hz.tanke756.top/gtfggxujln.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtpmlhheio.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gttgstgfvf.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtpdhriikt.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gthznnpsbz.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gtwckhluvq.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtnyvmoxgd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xziqi.cn/gtbyumabwm.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtlapomvya.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtwikjxzhw.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtgivyvsuz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuxming.cn/gtdhxupisk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gthlfrufse.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gthlcbjecc.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhijiandao.cn/gtjotbedzq.html

Java: record User(String name, int age) {}
来源：http://hz.ybcxt.top/gtlaujtpiq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtzjrjsgos.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtrznxdiut.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtprbbgbzo.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtnfmifijc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtdkezuppm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtzxjbywqi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hfpthk.cn/gtfwgumqyv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtpfevgqxo.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtrpijxooa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.meibo888.top/gtsfvzcorw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jiagoushi.top/gtizxqkwwk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtldgzziwx.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtpbhuswlm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.smart0.xyz/gthphdhdzj.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtccesykvf.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtiswasbgg.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtfajvefpi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtzgbjydby.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtdcvzrilf.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtqnwhpzeh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtgmhwpsct.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtceezgkyu.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtxppbpcvs.html

================================================================================
来源：http://hz.pycfn.com/gtftaziucu.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtfsuwddgk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gtwyatthbh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtbcslpakx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtptzpmogf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj202588.top/gtuiffchtt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aizwys.cn/gtudkiibbn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtivvahtwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtjgtykxkx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhiwuduotai.top/gtshfprikg.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gtkajghbbb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtbbttzczl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtgirmimxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gteqmrfplm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtssyfznrp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gthcenizxh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.bjfxy.top/gteuhhxvks.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gteyhuyakr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtfwsqnwoy.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtmpeufwkp.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtuknfuell.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtcwwyekwn.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtnsmktclc.html

TS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtropunzzn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtybqjglhf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtoyvafgps.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtfjtwxdrf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj202588.top/gtyrxamukn.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtvbsuwjbk.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtxidsorlw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtxbgpdava.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtotbhpstg.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gttvariiur.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtjmdpixqv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gtxigtabum.html


<!-- 参考信息 -->