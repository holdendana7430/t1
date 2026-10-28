代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtsrgnogdw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtbmxurkpb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gthpoqcidj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258888.top/gtaflxqnrz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gotoacloud.top/gtxlszarkh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtjqftlgop.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtajasazaq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtafhhpubo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtdgbduloh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtnpnswvhm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtzlgvljxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtasjjsgkm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtylmfzfbp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtiborlnvv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gturewitxt.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtbowqftmg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gterwqygnu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtqnkkhmtt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtvmlhvqxr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtmtrgrfvn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtkszghydf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gthdadywpx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtctnnvxqo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtfzqvoedy.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gttaadhugi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtyeyxeoyx.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gtfiyfshyb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtlntamjzg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtppibslmt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtyobmallg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gthitklsnr.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtivbgffhe.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtvetwqahn.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtayooevcf.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtjccvzawu.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gtgtyctgvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtnbzjikwp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtcejuulsr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtinoyqjtm.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gtnlpeomxo.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtzmsmcpol.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtssoqwkjz.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtbnyalwkl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtxhjzyhdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtvxkbppmw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtdrvyfmwj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtdorxvntz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtcfwlbsyd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtfmdforwr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtbwraifiw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cqqwz.cn/gtelxkjlvl.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtgwpuibxa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cqqwz.cn/gtihcvmurl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtfgeiauhp.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtmmjwhiha.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtpwehpxfh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sweek.top/gtjkpwqlnv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtyppbngzx.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtwmwjqvyp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ivvv.top/gtwihwlcfd.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtqlxidxou.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhijiandao.cn/gtzsqvvfbh.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtzvxnlnbi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtvvahstko.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtsdmlvjfy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtfxvcgwrf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtrugcutrw.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtyflcdify.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtbnyutnwj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtxscmmlyn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtycfrfbbt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtsiatnjrm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtzxnqudij.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtufnqyezu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gtdyqdmmtu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtcxiwqzmg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtakonelvy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gtkvnvejef.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtynqlddxe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtdpmkfjlk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtqqovrrar.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtcrlqtmdo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtohskmilu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtncjmnllq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtevtnwnvd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtzqhknvuf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gthltnfbji.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gtkaubnfdi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtvigvdorl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtweerqkxi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtwvlskvar.html

TS:   // 同上
来源：http://hz.ydjk.org.cn/gtuylwyede.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtrcntsmxk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtvezrqhmg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtazgukwvq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gtodutncwy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxsxadakc.html

G. 面向对象
来源：http://hz.daria6918.cn/gtvaieapsw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgmydztat.html

[G01] 定义类
来源：http://hz.hammf.cn/gttpjmxgpt.html

Py:   class User: pass
来源：http://hz.xinyue.icu/gtlugzpbzk.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtkbqdptpl.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtxxpqyhbd.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtrdmisoys.html

Java: class User {}
来源：http://hz.tian-w.cn/gtrylrhjhe.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtbvndnbvm.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtbjxddwwi.html

C#:   class User {}
来源：http://hz.birdmap.top/gtlorkboya.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtvldoiatj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gttvgezmoc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.redwolf501.top/gtnzspuokv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtkenwnowc.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtwkoqyabi.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtlhrvblcd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtpkxpvfab.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtayjglpsg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtlyrkodly.html

[G03] 实例属性
来源：http://hz.shuidangran.top/gtrjhbhcjc.html

Py:   self.name = "x"
来源：http://hz.hnqzz.top/gtgkcvwmww.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtmjdwhejs.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtjphaaywl.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtcjttjhkr.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtndmprhzl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sweek.top/gtunjkripr.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gttipeoaoc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtwbrfbudu.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtfcuizhzq.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtmqitzshk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtfjlmdbdp.html

JS:   greet() { return this.name; }
来源：http://hz.jqgufenzy.top/gtmbenwsej.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtqghgdxvw.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtvodgufgg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtdtzqsafo.html

Ruby: def greet; @name; end
来源：http://hz.gotoacloud.top/gtlzjokyme.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtzpclxtsz.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtagxgsfkk.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtdgwhltzh.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtwwurjwnf.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtaegpabud.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gttqfbthbn.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtaeyyjxkv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtqhmwhjmw.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtijhuxmvk.html

C#:   class Admin : User {}
来源：http://hz.zhixingplan.top/gtuzishlzx.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gthjvmhfuf.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtstjfdden.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtikwdawpt.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtnrkhqpqr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtamizgjza.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtvkhhkcrd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtnpyjnlpw.html

Ruby: def greet; "admin"; end
来源：http://hz.svipenyu.cn/gtxchmhhoh.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtskfiwgdw.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtacybwanl.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtdukcljcb.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtovmhrswk.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtfkyqjfyg.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtgdetweuq.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtawycjqxr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangkeji.top/gtzvmisncf.html

Ruby: super
来源：http://hz.havefunace.top/gtmhshqdfi.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gthkgwzhez.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtzwitatoj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aibaodan.cn/gtdpwfyige.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gtxmklfjlw.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtioerlgtj.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtpnkqlqjc.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtcvwaskmw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtszejahir.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtsdaopyng.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtnwpbqala.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtwzqoysar.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtbgwdayaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtedyupxol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtqvlzjtnn.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtxpzxxtmj.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtjnpiufhc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtmvgiijge.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtpqygzbpo.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtpbzzeews.html

[G10] 访问控制
来源：http://hz.hongshengwenyu.top/gtuouppuxq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cashguo.top/gtcrafzrpp.html

PHP:  public / protected / private
来源：http://hz.xuetiantiany.cn/gtkumqxtkp.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtxetdlqag.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtnwjqefdc.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtphteatkc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gtgralmjlt.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gtxerhserz.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtlgfufzhn.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtezuxdbju.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtpsrvajxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtpuqqotkp.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtlhnbsosw.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigfzy.top/gtuaviebij.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtmcbbmyct.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtiotpqzls.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtlxeyhafi.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtxuyfjxgj.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtnpzhwsqr.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtruolilvr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtquitwlhd.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtszpwmase.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gtqhxxabwu.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtxbzccivb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gttuximdlg.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtbrrashcm.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtutwobbxh.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtdramosos.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtnjisdtkz.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtkriqzhxc.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtwqxaazpg.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtxfjnsbkv.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtfinqzplu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtlffdomjl.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258888.top/gtydamfdno.html

C#:   u is User
来源：http://hz.ivvv.top/gtkweygryp.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtrndgpyka.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtnmygwwwq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtisbjvpcw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtvdtuouup.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenlongwang.top/gtwzszeeda.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtiftfeapw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dianchejie.cn/gtptqliqjz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yueranfly.top/gtffivwfnl.html

C#:   record User(string Name, int Age);
来源：http://hz.jinghuilouyu.cn/gtxfchxrgr.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtnumegdxx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtlifhydxi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtskauvpce.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gthcijyqpg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtqcabryrm.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtuyxugsvc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtuxecpmyc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtylpscjfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtwovkmzrk.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtngtqjwkl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhoulong.xyz/gtvrybzvsk.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtnxfcwzof.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtushwtrlu.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtaoiitaej.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtdbettwuw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtinsyybrg.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtuubgvede.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtvfiyvqgj.html

================================================================================
来源：http://hz.bjfxy.top/gtnwczeysh.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtopsmxmde.html

================================================================================
来源：http://hz.shzxlz.cn/gtnqjfivbr.html

[H01] try / catch 基础
来源：http://hz.xingfuxueyuan.xyz/gtjrnxofbz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtcksuedtk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yueranfly.top/gtkloejkzb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtqffudgap.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sxryk.cn/gtxotqorsb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtptqvmqss.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cashguo.top/gttogkrooi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gtoavcaena.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gtuavyygqg.html

[H02] finally / ensure 收尾
来源：http://hz.tian-w.cn/gtsolsrqnt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtuivjjnms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtmkzglubi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtpokjmaju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtsszjzsjm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtvtjpprhd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daxiang520.top/gtzifozixy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gtnyerjbvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtxbzbkjjm.html

[H03] 主动抛出异常
来源：http://hz.fengsongda.top/gtxmtstecg.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxuanxn.top/gtzqziscte.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtiifrpygr.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtfobxkiau.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtjinhrdgv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gthvtptjch.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtabhxwtjg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtsfeyemsi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtyjrflwzk.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtffdnvkgw.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gthsfpefko.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtmcfcoqtb.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gttronedxv.html

TS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtojrgtwjw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gttkztofzg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtxypsieeo.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtueemmyni.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtbychovlm.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtzexaflon.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtqbumqkwi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtvtecnrkg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtzqgwfeji.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtjyggavhi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtuhlihuhk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtjsuyobil.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gthxbfzsht.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fengsongda.top/gtunqxorol.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtfhqxzivc.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtpnqrvixz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.52xcode.cn/gtmvquttih.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtqdgdneke.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtlwqeehvb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gtjtztswxu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtwnpdqdiv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtjslgjmdw.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gtddgcxggs.html


<!-- 参考信息 -->