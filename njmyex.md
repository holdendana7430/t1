代发 wailian999

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtqimzpizb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtubgpbszh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtgielpyka.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258.top/gtqvecevaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.haohaochexian.top/gtxfgpuuay.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtppiggiwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gttrenaoaw.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gthkajcxvd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtgpntfmur.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtimaatxvs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtprgdzudg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtlexorauv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtuqqoplsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtglfkauwo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtauhpgcel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtwcrslvhr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tanke756.top/gtwpfmivfi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtdosewncj.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtqkeuzbqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtbhnnnasb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtvvdjdzgg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtoqoeccli.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtqxjburij.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtserujayr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtpwgbtufi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtqqgjodcf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtspbfejzo.html

[F04] 追加写入文件
来源：http://hz.zhiwuduotai.top/gtzeqwlvdo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtamvryqwp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtpyygnxon.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtzpusrmjc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtyykhmpok.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtmqyyadfk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtinrppkuj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtstezsjrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.52xcode.cn/gtdammjbek.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtcdlvjrtw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgufenzy.top/gtivlnmofs.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gtxdsyfctp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtqccwifpf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtveertksz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtomvlvpho.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gteurtanyo.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtodrqibjf.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gttkhgvitj.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtayorjllw.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtfoqmubby.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtqbssvgmh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gttuwnnenp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtpcmvqfld.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtzpwayfxy.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtbuhwhhtz.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtqyppxoql.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtmcwvatbo.html

[F07] 创建目录（含多级）
来源：http://hz.jiagoushi.top/gtkzsapcri.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtuxyfnabx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gtnifrtqgm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtmlfsmwok.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtqjiropbi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gtkayizqty.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sufxvd.cn/gtgahjpzij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtuwlpovrj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gthcadxhph.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtkwmehnxn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtvxbljmtv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtlupuiwwu.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtsexjwcmo.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtcyfnynkz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtsjvcakhd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtcutanfdd.html

Ruby: Dir.children("dir")
来源：http://hz.fengsongda.top/gtsruggmar.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtwtrujavx.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtaahasuyj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtwgwlijcj.html

PHP:  filesize("a.txt");
来源：http://hz.ybcxt.top/gtxbsgazts.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtujcdoojc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtsoywstmh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtzefnwryd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtamisjmxa.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtodjxskdz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gthkytvgoi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gttabvzrum.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtguqogcdr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtvuntxbeu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtzokwaeee.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtzicxjrnu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gteingjqel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.c1oappe.top/gtmbqxkqcp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtluqgrmon.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtsisemmbr.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtzmgftden.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtchegwrrf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtrheonhra.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtznunmalz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtshatyzjd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtqwdbcjug.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtsyrjadeu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtqjjdtlns.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gthknwbffq.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtrzktutvh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtxdxsjrcr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ppjwa.cn/gtqmnimvrj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtderznwqc.html

TS:   // 同上
来源：http://hz.sufxvd.cn/gttzwfcqee.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtaezwrvde.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtiurczopj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuanzhike.top/gtxmjidowl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtlznkawhg.html

================================================================================
来源：http://hz.shzxlz.cn/gtdmlrjjdk.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtptjbaohc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtedhduwvn.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtnhkspazm.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtobxgebei.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gthqpabzoo.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtcbjtuzxr.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtnjmkwepn.html

Java: class User {}
来源：http://hz.nwbrower.top/gtiatjgalv.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtfnxzknik.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtkrfqzscc.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gthqddmqmt.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtusskhsea.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtctgcdubk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jyoumei.cn/gtynnestdg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtsthywngq.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtixxvlpwt.html

Java: User(String name) { this.name = name; }
来源：http://hz.tanke756.top/gtassfncjh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gthbnxbuor.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtapeyqpka.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtvmsrmdeg.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtoduceymt.html

Py:   self.name = "x"
来源：http://hz.zycfv.cn/gtgnjqsvdb.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtflvqhebh.html

JS:   this.name = "x";
来源：http://hz.haohaochexian.top/gttmixobjp.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtrlqoqred.html

Java: private String name;
来源：http://hz.yj20258888.top/gtbpxheihl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtywmqizaz.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtajmzhbgh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtzrqgnhpp.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtjsxjyami.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtliqpeqex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtgqcacyox.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtxoiqrako.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtydmgexpq.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtlvjbxhbt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gtlmcqeirz.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtonwvaqxt.html

C#:   public string Greet() => Name;
来源：http://hz.ivvv.top/gtahbkarbs.html

[G05] 继承
来源：http://hz.smart0.xyz/gtzbhplpbe.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtemjrbjdy.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gttpkohiuc.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtkznqnzjd.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtuxurammb.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtokgxprno.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtejxabuey.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtvhgoesnv.html

C#:   class Admin : User {}
来源：http://hz.hammf.cn/gtmnirdzxj.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtnaafyctc.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtiyjyhohk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtuienpioq.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtfeuztrft.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtcpoevguj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtrpspquds.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gthucxhvyq.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gteuxsausa.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtvvkodfvq.html

[G07] 调用父类方法
来源：http://hz.xinyue.icu/gtvltqnwzw.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtiyvjoqdv.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtoygnjyuh.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtvdyecngh.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtafpsrgqf.html

Java: super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtkfsvmstt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtghyuxbzm.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtkbwjwcyl.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtxqymkgtb.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtzsbhfytw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtukojfvdt.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtzfzmcyly.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtomwzpumg.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtegioqjjr.html

Java: static void f() {}
来源：http://hz.fzhhl.top/gtyqxebvxj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtmqdhlsgb.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtalmjyviw.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtcurnylbz.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gteumbwvbi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtcadrxdec.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gtsoifekmo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangshuangyany.cn/gthtgicuhd.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtlgueptiu.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtecyezczz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gttlrwotkd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtgbdghzyt.html

C#:   interface IShape { double Area(); }
来源：http://hz.sweek.top/gtmiozkmvh.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtggbkefmh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtswaljoyl.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtvtagvyny.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtguzivnhc.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtmvkbhzyj.html

Java: public / protected / private / 默认包级
来源：http://hz.yueranfly.top/gtjhjcephg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtksmkptjf.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtplkbedyt.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtimcjrfln.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtoibuwmkj.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gthxuzixhj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gthhodbjqo.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtczptbgvl.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtfbbaqlbn.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtiuimrnls.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtkebzutzg.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtxjbiscxd.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtqaebajun.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gthhpxcwwy.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtuhhwhkda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtdztouavy.html

JS:   toString() { return this.name; }
来源：http://hz.ivvv.top/gtifqrlemw.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtaqvgaqix.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtygjyqvlc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtbbuistcn.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtxblhvnwm.html

C#:   public override string ToString() => Name;
来源：http://hz.tian-w.cn/gtvgqrnrcp.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtdbrwhsbs.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtjndzkglp.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gttdxjolfi.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtjwoyiptt.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtexatcraf.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtjqaljist.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtiyueoyup.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtnzxmnbfc.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtxekhptod.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtwsioimuu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtehmjelex.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtabyxktzy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gthzutakvj.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtznurhiln.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtkednqkee.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtkgqorfda.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.vqdsnc.cn/gtnpyapccy.html

C#:   record User(string Name, int Age);
来源：http://hz.bjfxy.top/gtcuaukkgs.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtfdesphjs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtbmlsjkhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxuanxn.top/gttqquziqc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gthwvnbhnz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gteshxvzps.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtsqyojnhg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtkjvuwkdr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtzfvqqzsi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtelxfdpgn.html

[G16] 对象转数组 / 字典
来源：http://hz.daria6918.cn/gtvafrgjpn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gtokwfxzuj.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtdkucivtm.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtpotxwzuj.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtrvdbtgrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sxryk.cn/gtkwrqwrcf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtobwwuruk.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtswowgaon.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnqzz.top/gthjmasfil.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrpzniifq.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtwzahqlnq.html

================================================================================
来源：http://hz.yangfankeji.com/gtdsspifzj.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtpswlnltn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigfzy.top/gtfnovkuoh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258.top/gtzphcrhfa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtttyhwcwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtizyeueen.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtkbngugbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtfakubfcd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtdpayyodd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtetymsdka.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtitarojyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtwszpzbcs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtczudysts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtoxpsnric.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtbpchgxbw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtalxqauyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtumzcmais.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gtyejmodfd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtfargytnp.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtbapbxwxu.html

Py:   raise ValueError("错误信息")
来源：http://hz.tanke756.top/gtfxitpcou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.havefunace.top/gtbjwuiqak.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtbmfaelvw.html

TS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gticvymzjg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtuwzytmwt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dashuyun.cn/gtgtsrorxb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gthwmumuso.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gttlhslujw.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtmnwofhef.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtnktrqkbu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtbfzeueuh.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtfpzfjvfl.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtwgvqzlks.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtvjsdjgef.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxuanxn.top/gtyirzlbus.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtpxpnsnfy.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtzovxirps.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtczzhgrhd.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtubdaehbz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gttmbqubdv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtncughnit.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gttrjjinnf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtcsnlzgak.html


<!-- 参考信息 -->