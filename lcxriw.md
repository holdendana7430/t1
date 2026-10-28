代发 wailian999

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtupevjndf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtxhfpyfmc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtkwifypiy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ppjwa.cn/gtwqeycgou.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtoeacnrke.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtbtaereqa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtcuhsuatr.html

Ruby: File.read("a.txt")
来源：http://hz.cdnleiting.top/gtpxwherpq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtenaflqab.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtmettlbcj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtfhpzsveq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtofroudwt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtnelkuntk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtujjgzbma.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtafotpkxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtlvnblrml.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gtnnkbxqpt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.quarkkingdee.top/gtkmzpswap.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtgbcytzor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtoejsinjv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.havefunace.top/gtdtmgdwqo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtruozoscx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gthaahvzfl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtfhqbfyze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtysoylzco.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtumvomexw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnqzz.top/gtorefauhr.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtqezbhxac.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nanxinkj.top/gtfbvwavhb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtsrkqmsdu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtkpgprdge.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtmpemuhcp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtswpbdujo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shzxlz.cn/gtjbbcenjb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnqzz.top/gtoqjgcqqt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtbairmwma.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtcgcqoisc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtnlrxqfjq.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtigfigoei.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtxmoepwsg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gteoovazqu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtquthcvqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtaaszrlbx.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtqulqmicw.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gturhdqxgf.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtrxcedhsx.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtuuvfkymi.html

PHP:  unlink("a.txt");
来源：http://hz.chenlongwang.top/gtxcluguoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtywtenubx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtqmpckoev.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtrxfajqbr.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gthwpygelh.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtzcftgqdy.html

C#:   File.Delete("a.txt");
来源：http://hz.chenlongwang.top/gtnpdupcws.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtusjihpur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtfvfacego.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gtccwwlnyp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtbdvazxjt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtzhsgofln.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtpebnrunm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtcifevdmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtocjussqf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtqtulcuep.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtowrwckvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pycfn.com/gtvykqnzqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sxryk.cn/gtmcabyova.html

JS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtpvugzuia.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtmjgzuwek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtybqnqwua.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtfugrpopm.html

Ruby: Dir.children("dir")
来源：http://hz.jinyuanbaomall.cn/gtmfmrlkpb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtjkyvjjvb.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtornqgodb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtzpgostos.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtamrefupo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtlcwddwpy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtppkksmlb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtrycktujb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtkmezzitt.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtkzxjcgiw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtmydewxss.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtqkyytzyy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtsmlnwqoq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtgolpjrqn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtakgxmtua.html

TS:   path.extname("a.txt")
来源：http://hz.hongshengwenyu.top/gtfbzerlfk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtnrwjkfwe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtjqxhqocu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtyjsgnzhz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xziqi.cn/gtbesizsmi.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtsevlwuqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtkpasqqaz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtaofsbzoj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtgaewigxc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gthythekji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtswndimpw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtxmcdvtlb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtgvfmsxlf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtkfomqfhd.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtllfxcxpy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtcbwfukxm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtntrowkgx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtisqeqknn.html

TS:   // 同上
来源：http://hz.nanxuanxn.top/gtqlyvwdhp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtkqgkbhkt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtzpduprlh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hysaishi.cn/gtelcgozry.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtsicssqjq.html

================================================================================
来源：http://hz.shuidangran.top/gtuqofvodg.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtnedmxblv.html

================================================================================
来源：http://hz.yuanzhike.top/gtfemedmxr.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtdjzbrbzp.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtbmptwjng.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtbdqmvqgr.html

JS:   class User {}
来源：http://hz.zhiwuduotai.top/gttekjghyb.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtmqkrdflr.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtyndlzmih.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gticaixqxq.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtixxlyysv.html

C#:   class User {}
来源：http://hz.meibo888.top/gtdsyqzmlm.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtkcttwcll.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gtapgqmulp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gttftvkrum.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtixvzfhsy.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtsqtvminf.html

Java: User(String name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtgtmxkete.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtqrtlmmpk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.haohaochexian.top/gtisyqsfrr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gttezzhvwz.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gtqayvpigm.html

Py:   self.name = "x"
来源：http://hz.cashguo.top/gtizgncbem.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gthggqktwq.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtivczskrr.html

TS:   name: string = "x";
来源：http://hz.snrcjt.cn/gthtbntzlm.html

Java: private String name;
来源：http://hz.yueranfly.top/gtjnqqkzpi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gthavgtirf.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtboqegtpw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtwqvcoeiv.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtiiyuxjlw.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtjsneqeve.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtlugnivnu.html

JS:   greet() { return this.name; }
来源：http://hz.yuxming.cn/gthzndkfki.html

TS:   greet(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtviprrhex.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtwzmdowyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tanke756.top/gtqbfeohge.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtylfacfpv.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtlvzggzfy.html

[G05] 继承
来源：http://hz.redwolf501.top/gtcsrbunnb.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gtjcvvgiar.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtduyfazmg.html

JS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtkkgfpdob.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtknowfvly.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtpxdfqaxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtrnquzfxz.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtgudhfqtd.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtgfzjbgrq.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtmdzqjhro.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gttyjgmazx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtgdgkrrdi.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtonuplmwo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtsbpfvpjf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtnouadoxt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtaicdnrjo.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtltkzimdr.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gthumorvyw.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gttrbcmtnc.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtohedoynz.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtkqjcimxd.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtvddaeytm.html

TS:   super.greet();
来源：http://hz.9152youxi.cn/gthkqmycjg.html

Java: super.greet();
来源：http://hz.hnxiangtu.top/gtkmygakzk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.svipenyu.cn/gtmybuajuv.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gttwrbkcdb.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtskysmqwd.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gtbmqokqfp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtpvuyxwxj.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtqlhyfxhs.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtubgatylm.html

TS:   static f(): void {}
来源：http://hz.ywan-chungtsiang.top/gtjksgdepz.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gtchjfmelf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.redwolf501.top/gtlapkchss.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtehbtqlgn.html

C#:   public static void F() {}
来源：http://hz.316326.xyz/gtaqqkrjgo.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtxkssmlfb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtnltyhggu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtoohzcpqt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cqqwz.cn/gtrjmaifdl.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtdiuirssf.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtlxctltli.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtidcufoez.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtuxcfsqyh.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtvvtvphhz.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtngpueidj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtizuwlrfe.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtkvnzzzyn.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangtech.top/gtzpygipsp.html

TS:   public / protected / private
来源：http://hz.cqqwz.cn/gtmalzkgye.html

Java: public / protected / private / 默认包级
来源：http://hz.daxiang520.top/gtbhclkuwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtxvwscxcp.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtyunpvhkd.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtpkzxigwc.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtuiaambls.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtltxblwwb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtguozlssg.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtcajzmkue.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtqkxwvean.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtvuqnhyrl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtpqqtnacq.html

Ruby: attr_accessor :name
来源：http://hz.gotoacloud.top/gtwfffddhe.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtcrlvlqid.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gttkxoouiz.html

Py:   def __str__(self): return self.name
来源：http://hz.dashuyun.cn/gtdrzqbfrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtvhlqayal.html

JS:   toString() { return this.name; }
来源：http://hz.aizwys.cn/gtfslqwybg.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtemsfjsne.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtervlasuv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtovijcdjx.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtrlmldypv.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gthjywzcgv.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gtwpfvmpke.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gtwbnljxhz.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtcqggfene.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtegwbormt.html

TS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtupasxuau.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtzvonufzx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtowhurxlh.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtcvsnarzj.html

C#:   u is User
来源：http://hz.nanxinkj.top/gtwianrkhu.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtmlqgxxuf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gthdnkhcrx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gtwxesovdg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtpsyrcstu.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtypnbgfyx.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtjoylzbaf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtclcivvvt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.redwolf501.top/gtbldbiqop.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gtcrozkzam.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtbiogtolh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.0kj1m.cn/gtwbnchjfp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtcifkjxlw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtaotuabjj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtlwaxzzvm.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gteoobxfho.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gtewfdhmbm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gtybtwngan.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtintlmzrt.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtrkxviffr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtdmbwgzaz.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtfmnffvlp.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtmuiqghdt.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtyfvmqmfa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtwqahxkif.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zycfv.cn/gthlemxzzx.html

Ruby: obj.instance_variables
来源：http://hz.daxiang520.top/gtnktyohrg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtlebypwwf.html

================================================================================
来源：http://hz.shzxlz.cn/gtrqtcbeka.html

H. 异常与错误处理
来源：http://hz.vqdsnc.cn/gtpjesqcpu.html

================================================================================
来源：http://hz.sysykeji.top/gtnlfpnexs.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtnwcpdchg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtlxrzxykf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtxaelsfto.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtuvkyavei.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cashguo.top/gtzgsnlkzc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hywenlv.cn/gtfrxsmema.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtfxxkajnz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtmufeydrf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuxming.cn/gtsgglyavl.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtxdrjznqs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.andypj.xyz/gttypuiazn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtsrutipsn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtsuajgixa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtpbacanzv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtcvmihdvi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj202588.top/gteecbtzzh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gthfoljcgb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtdfvucumk.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gttqgkujmh.html

Py:   raise ValueError("错误信息")
来源：http://hz.hysaishi.cn/gtqxwmjhgr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtsnkwrpqr.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtfcayxxze.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtybuyknkq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtczukebtp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxuanxn.top/gtfdfivqpi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtlorqdovv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtwzkbswme.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gtdjxcdnoo.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtpkkacjsi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtaxtsfkvp.html

JS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtxmwbidlw.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtqgpagyyq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtazcrgmbp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtnpxwbjua.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtnmghuskw.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtyxfxcehq.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtidgpvswm.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtxzvprhyq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtaikbtrsp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtkvqitbvh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtmimgvgtw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gtejuzimwe.html


<!-- 参考信息 -->