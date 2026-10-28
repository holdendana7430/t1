代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtfjhqixjz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtrpakkaoe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jianghu66.top/gtcnuhlidp.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtofpfrwem.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtzjzawbvb.html

[F02] 逐行读取文件
来源：http://hz.jinghuilouyu.cn/gtrfldkges.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtndivepqz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxinkj.top/gtkiatmopl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtuadzkioz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtbsjaobbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtfegsfgvz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtrlrommpb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhongyouzk.top/gtymwtyrfn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtgygqoxhz.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtgendusmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtayaqxtlw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtshpxqvvt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtesrtwwjf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtcmjygkkj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtfvfrkspp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtfydfkxii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtvhoawgxk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtegqgqiqq.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtyqrnhnnr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtshpkpxpz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gtwuctdyka.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtyawyvwtg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gttdpuqebx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtpqxybgge.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gaohongyu789.top/gtszmenpwf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtikefbcrv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtirxyqzsl.html

[F05] 判断文件或目录是否存在
来源：http://hz.tanke756.top/gtoffpbzup.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtlwbpepxv.html

PHP:  file_exists("a.txt");
来源：http://hz.chenjidiqi.icu/gtzdfvggxf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtajnpcjaq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtgslumcdg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtxhjtqqmy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtwruwxiyk.html

Ruby: File.exist?("a.txt")
来源：http://hz.shzxlz.cn/gtilhskxpd.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtlnheagvu.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtvwrfazbf.html

Py:   os.remove("a.txt")
来源：http://hz.ehwqpu.com/gtwopnqmdo.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtuzizrily.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtgdsflyrc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gttmemyhov.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtharmplpp.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtaghtfeps.html

Ruby: File.delete("a.txt")
来源：http://hz.redwolf501.top/gtamzvyxke.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtbmooyeag.html

[F07] 创建目录（含多级）
来源：http://hz.redwolf501.top/gtxzemxrek.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gttbirirrp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gteijmylym.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtxeprdnov.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtcktkxxro.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gttgrbfnki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtlxamcxoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgufenzy.top/gtzqukqzku.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.birdmap.top/gtiqxzsnsz.html

[F08] 遍历目录
来源：http://hz.pycfn.com/gtzvilvxdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ehwqpu.com/gttbwywiyg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtpbebwulw.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtaayktayt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtkfohaath.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtdtnwyqgd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtvjcziroe.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtpkxsnnfr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtmaxhaxvy.html

[F09] 获取文件大小
来源：http://hz.hysaishi.cn/gtvxtzrqlx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gteeiqbfpq.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtwvkzogmg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtpyqxfgxl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtvigajgdd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtazkbsegn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtrzcevacb.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtfcujujkv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtatftttfm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtuwhvpuqb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtbetvttfl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gtaggehidg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtdfekrarq.html

TS:   path.extname("a.txt")
来源：http://hz.zhixingplan.top/gtuewmemsq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtnogtkbnt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtzbisfvfa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtodbmllrg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtdklbljgj.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtqctgwbbx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtsnbcgska.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtbvkcvnvu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtjkvyyryk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtroxfphiu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtwpobujxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtdntzrjlo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtccdccwdl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtlpdzjsmz.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtwkvouygc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtxcjrarcn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtidioyvjy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtrrwximtz.html

TS:   // 同上
来源：http://hz.tian-w.cn/gtdsohuxsq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtompokpxq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtrxltfkda.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yvedp.cn/gtzwovboqz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtnugdohjd.html

================================================================================
来源：http://hz.andypj.xyz/gtjkarzmkk.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtawenohvv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvwkfznvl.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtwzbqsfxh.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtezbdkfgi.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtooexjdwn.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtsjdsamhl.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtublasgdz.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtwbzpdtqc.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gticqscqxj.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtutvvhswn.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtttboltum.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtsfeozibu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtxzzayupy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtgeahnawl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtlkanhjvm.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtxsjgecny.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtkxhnmowg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cqqwz.cn/gtderekdnh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtfxfagenw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtpkrnbzur.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gtkxzznwud.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtrmzougiz.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gtdvmlttgy.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtrcfgeeqz.html

TS:   name: string = "x";
来源：http://hz.snrcjt.cn/gtfitjboma.html

Java: private String name;
来源：http://hz.cheryme.top/gtfkhudlxy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtlfqnbtbz.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtoiebxtus.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtyzclpsww.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtodwlfzsf.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtlyluawyh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtzoncekiw.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtbzdzoxcj.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtwjbtehcw.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtnzollnmu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtvucuwkpj.html

Ruby: def greet; @name; end
来源：http://hz.yongpay.top/gtpdwtfxnw.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtscrexzkx.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtferfzgbq.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtvuxvbmua.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtcvqaberw.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtxjfcuiwl.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtokfbwxaq.html

Java: class Admin extends User {}
来源：http://hz.52xcode.cn/gtnucfzzvo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtnublwugp.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtgmdmkypz.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtwkwdtfab.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtazcmnvnl.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gttwhmqodm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gttpwamqpj.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtcazievph.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtsbitqexp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtdqbpnonj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gtrugayhzu.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtrokhxuep.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtjpmiuqij.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtcclwphdn.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtrfnpqtpg.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtppzjqdcq.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtsscwkefy.html

TS:   super.greet();
来源：http://hz.zhixingplan.top/gtuqonoxvv.html

Java: super.greet();
来源：http://hz.tanke756.top/gtpjcztuko.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtslhcpqcn.html

Ruby: super
来源：http://hz.shzxlz.cn/gtkbwjunqe.html

C#:   base.Greet();
来源：http://hz.meibo888.top/gtlzxcymim.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtmkucznoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pengpengdd.cyou/gtdadwidpz.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtcsxdtdjt.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtasrsyifb.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtvmafrtgy.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtacckkiqy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtgslcoagh.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtgzfkxpor.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtjoxutkhg.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtktvlazly.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtkhieyrgt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtkcklwnmj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtlhstztiu.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtjhzlzhyv.html

Java: interface Shape { double area(); }
来源：http://hz.mhx1999.top/gtlrdjdojn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtwlrqubah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtahwjqfay.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtkavozrke.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtcdjdcogj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtwpkosaix.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtoqdmpadx.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtyrqsgnid.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtdhhpauqu.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtalyjgohk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtnirmtbdy.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtkdinzxvj.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtvjogzunb.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtpwdfwqgt.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtcbdcpjdm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtarocqowm.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtudgeqenh.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydzc1.top/gtsngwyigk.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gttklfczvr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtdwsjqlix.html

Ruby: attr_accessor :name
来源：http://hz.dashuyun.cn/gtgparujav.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtjmqpcbhe.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtwdfdupgn.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtzpgeagwe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tanke756.top/gtiummoynn.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtahevjecy.html

TS:   toString(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtuzpludie.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtrlywpmfq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtkzgkmjxx.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtwvfpcems.html

C#:   public override string ToString() => Name;
来源：http://hz.9152youxi.cn/gttzfpwsdd.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gticufpxld.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtxynpqind.html

PHP:  $u instanceof User
来源：http://hz.cheryme.top/gtyrhvpvij.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gttxrbcmxe.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtnvktiaku.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtnvfjqauz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtoawtbsuu.html

Ruby: u.is_a?(User)
来源：http://hz.9152youxi.cn/gtxbnusjso.html

C#:   u is User
来源：http://hz.tianlin.xyz/gtylpkthdi.html

[G14] 数据类 / record
来源：http://hz.ehwqpu.com/gtzeenrwul.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gtjvielsic.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtptoiqkhv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gthyrnbgyw.html

TS:   type User = { name: string; age: number };
来源：http://hz.feifeiyinyue.top/gtcwgmfmkx.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gthxkfrstv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtsxcfmfeg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtxhxstgbg.html

C#:   record User(string Name, int Age);
来源：http://hz.cucudq.cn/gtgrvrwsit.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtaooqwwls.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtprkluhle.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtmrjdpzwk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtkabqdafy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtxhtftybl.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtgjmrupml.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tanke756.top/gtqjwhlhvi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtsgfztpzh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtzfxgnjuw.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtlbvmqnof.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtzzdsgmiz.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtthbpxjyy.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gthnjsvbmv.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtevftefbt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtrftjvzxf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gtnndhdhrb.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtggeqiqaz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtwhzhsyus.html

================================================================================
来源：http://hz.shuidangran.top/gtfpnsnxjz.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtowkgtbar.html

================================================================================
来源：http://hz.xinyue.icu/gtkemzsknj.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtlxknlarj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtpjxiocrn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gttkdeajjk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtjhpwbike.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtneaxuwzs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtdnaeqqqj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtkqbcyjjg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gtiqxvfuve.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtyjbactvi.html

[H02] finally / ensure 收尾
来源：http://hz.tanke756.top/gtlqcnjqiu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gtypajsisx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtidbukdbu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtaaklojmx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtsmlawkjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtvcasgsps.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtobmbxbvn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtegiwzxxg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gttblrbyxd.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gtuolcqyyp.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtvjovtdwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtjfdznrcg.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtsdfhoyci.html

TS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtqflaiwhg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtmyhrlqhi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gtymkulrdp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtnvyknjkv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtaexviyup.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gtouwbcqkn.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtuqjhcogz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtwbbnhjwv.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtjfcevypr.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtooueuzzy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtnsigjrum.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fzhhl.top/gtfnonkzyp.html

Ruby: class MyError < StandardError; end
来源：http://hz.yonumen.top/gtkvspweit.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtdtuwnyze.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gtzesqhoan.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtnhgvwcfw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtjqsosife.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtoomzvutg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtewsvomhy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtnwzswcon.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtddjqhlvq.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtfdyeizbs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtwhuedatw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xylfe.cn/gtejflqjrx.html


<!-- 参考信息 -->