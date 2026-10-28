代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.yongpay.top/gtwnrbsjuq.html

[F02] 逐行读取文件
来源：http://hz.jinghuilouyu.cn/gteodznzin.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtquzuapkr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtzijxekdr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtojweqxyn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtydzjagpx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtvyybiotn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtmrvcypxx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangshuangyany.cn/gtvkbwoqca.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtmwbbuaqy.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtjpmvdgeh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtadiyjdlo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtjdbuxequ.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtukfdoswa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtxcqlxawy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtghewryix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtptuispqu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtxidgmgiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtzkpktfnh.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtqthgwelm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.mhx1999.top/gtbsdrezhx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtgmydjiys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtowrrkccd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtmeagdawv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenlongwang.top/gtaxyfjccj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guannengcc.top/gttylhyzkx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtszyzusvv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtggktvzbg.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtmfobqobh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtsdknuayz.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtkwcwcwty.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtpldqqslf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtseskqnbr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtdultnwnr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtylaszxuq.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtfgxwesad.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtjyrdkkzo.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtuxupevnv.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtecbxcjuf.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigfzy.top/gtpoxoidla.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtnozujhht.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtkknijskj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtztyjpoid.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtjoeksdqt.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtmcxtajqz.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtradebowk.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtdvaebgqh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtyfxegoxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtslrrwvhk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtrnmsywne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtxzkwsrgp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtzgrgnfwr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtndjpjzom.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtwaosvacq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gtxyoqfaxu.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtzjmboqzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtpenipkmh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtbwbrsyww.html

JS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtxafetovd.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtwvfywpwa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtuuqivxzm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtrxvfgnaw.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gthfqaheec.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtwiqnmfnm.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtnmolkuad.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cqqwz.cn/gtjuwkltew.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtpqmxhups.html

JS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtuslewqxb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtzhivtjxo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtcpbuvywa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gtmochttfo.html

Ruby: File.size("a.txt")
来源：http://hz.nanxuanxn.top/gtqadpiorh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtoagubxno.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtqtnhyhxa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtthdzwnea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gtphapzudp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtzneokhoz.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gtmphxzwrb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtkrkhbwuk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtcxsduhla.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtbzgdchze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtunzbroxq.html

[F11] 复制与移动文件
来源：http://hz.quarkkingdee.top/gttlclrmji.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gttbydyqoj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gttlhfcpdk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtwijtthpk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtqdxnzacz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtmahvtvhn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtdjauhfvf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtsytkbsde.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtmykaghbr.html

[F12] CSV 读写
来源：http://hz.mhx1999.top/gtujigdmbq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258888.top/gtahnfitxv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gthstewuea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtsqjrfuxp.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtfhtjwjyl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtmgnjbdmg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtazukpehz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtqtxpubtk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtibvjmyid.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsiekktem.html

G. 面向对象
来源：http://hz.redwolf501.top/gtznonqket.html

================================================================================
来源：http://hz.aizwys.cn/gtsqgfnlou.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtfmhrkhqe.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtgpkikvgj.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtiwxqqfbe.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtaozvfgwb.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtmimqvepy.html

Java: class User {}
来源：http://hz.nwbrower.top/gtpxrdyacg.html

Go:   type User struct { Name string }
来源：http://hz.smart0.xyz/gtnsaqcfif.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtptfzzewq.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtzroqerba.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtdshvzcim.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtbewhpryo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gthrpkujlm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gthgqslxwt.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangkeji.top/gtlnjmytfl.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtdfnepusn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtblovvfvm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtzmrywjrr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtycijzjkm.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtlkhshupb.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtgqjjuhgs.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtypwnkogt.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtpqvkzrvl.html

TS:   name: string = "x";
来源：http://hz.dianchejie.cn/gtaycpquia.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtjigtnlqm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtljikiobj.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gthdauiixj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtlpffgziz.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gteoovfsiw.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtbokhkuba.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gthtqgdont.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtpheqtfjn.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtgexazeie.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gtsmialzmx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtxychkqpg.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gttywhxpmn.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtepqkkewd.html

[G05] 继承
来源：http://hz.jianghu66.top/gtibvkitvx.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtvwzooihe.html

PHP:  class Admin extends User {}
来源：http://hz.gogol.net.cn/gtlwjguogv.html

JS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtbrkrwdub.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtmozxltpz.html

Java: class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtalfesetl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gtdcprazat.html

Ruby: class Admin < User; end
来源：http://hz.jinyuanbaomall.cn/gtmvduqieg.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtfljwpddm.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtqvohnhfi.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtvvtrtvwb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtbxnvkjlx.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtdpfxlsqp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtgkmmboxb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtqfoifwqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtlifwbyfq.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtnrrhgxlm.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtclbrqzwz.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtcqxnzygm.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtwjsdsmxt.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtrkkhdlnu.html

JS:   super.greet();
来源：http://hz.sweek.top/gtmzxevtkz.html

TS:   super.greet();
来源：http://hz.316326.xyz/gthkvkyxsl.html

Java: super.greet();
来源：http://hz.yj20258.top/gtfjjjnxje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtbodztifi.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtmntagows.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gteyycsnzw.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtxgjimudr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fengsongda.top/gtaqdllsaj.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtewklcoyd.html

JS:   static f() {}
来源：http://hz.yanxiufei.cn/gtcwbmkthl.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtoxvioseg.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtwdpzvwdq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtyprvibyg.html

Ruby: def self.f; end
来源：http://hz.birdmap.top/gtboreheat.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtfaasbeuv.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtsoqzadxe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gtilicbece.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtjrncvohd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtmbrorrwt.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtbcxwcilq.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtwlxikpjg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gteenanrms.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtcfptnury.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtffgcvuyh.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtcjuqkslo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtuvrhlcnv.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtyduvhove.html

JS:   #private 字段；其余公开
来源：http://hz.fzhhl.top/gtmwlvmgul.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtzgpdlvzx.html

Java: public / protected / private / 默认包级
来源：http://hz.zhixingplan.top/gtdjjpnutj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtcqmabeps.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtvnvjrhse.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gttglmlgax.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtjrsehtlf.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtytzzceib.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.redwolf501.top/gttmocwzmg.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtfmrwcxte.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtoejmunyr.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtkwtyukme.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtumrgzkfc.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gtqtsmudxd.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtdgxmpfzl.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtoyqsyqel.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtbsadvlez.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtjywzmmlj.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gteudulrge.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtuzxyyztp.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtudqdkkws.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtotwjefbi.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtfibauiis.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtcxzafzra.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gthsmrmlua.html

Py:   isinstance(u, User)
来源：http://hz.cheryme.top/gtgabeiboy.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtdxbhryvm.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtwypwjzow.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtmrqtcjaq.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtdsrixiyn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtbfuheejw.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtvtoafknc.html

C#:   u is User
来源：http://hz.mhx1999.top/gtkfdmygqj.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtzdjyccxr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtvsnqlycw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtgosmqcbi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtjhwjfaiv.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtwiahsecw.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtmslggtap.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtumdelpde.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.52xcode.cn/gthbsyqppu.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtjpvgtlmf.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtkocyortp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gthnrdvxtd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtxajdvjva.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtrncdkugd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtuprloumm.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtnjisvddv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtoeukhklj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtvomqoxil.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtedklzavk.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtsaicbkbi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtemmrcmmt.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtkrnivgmz.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtfnzmqfak.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gttushpawa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtaalnyooa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtmiuahptc.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtuxxhoasr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtwzzrbyww.html

================================================================================
来源：http://hz.pycfn.com/gtvyhhpowr.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtwguqojzc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjmpxvdol.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gticqdqgwd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtwmmfysff.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtirizilnr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtkrgogwrj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtxiomybnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhoulong.xyz/gtprhxxagd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gthebssclq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtjmiafocx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtyklmhkuq.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtabnjbrpb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtxobplzey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtgthotlox.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtdixcvdub.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtwpxleraq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtwjvjbncs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtkleyhlcr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtviopgfjf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtgedauxhe.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtrdhhoqkl.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtmjmnhdfe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtnpildaau.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gttfgwhyzo.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtoojamdua.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtevlodart.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sufxvd.cn/gtybgnknri.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.bjfxy.top/gtwccndpbd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtokfsmcmm.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtqemoawnp.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtjkaagsni.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtnxbvdbur.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtzoaadoky.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtatmoolxh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtamelwjdn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtypkwysyz.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtlgebibfi.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtzzqflmcg.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtabvqyzph.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtljinznvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtsoruwfuf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gthvjxsmil.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtbjkzopvu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtsjegdrkw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtsgbouwxc.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtsgxebjtm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtyrprontn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtckhsfhar.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtuflzprvi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtxxzqzsig.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtlujkpjxb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtvhvodmop.html


<!-- 参考信息 -->