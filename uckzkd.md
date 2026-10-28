代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtrcnshjjh.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtmzjyuooy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtyiqruopx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.9152youxi.cn/gtnyopenty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtzalodevo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtqrpikmqn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtzguzaqqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.haohaochexian.top/gtxdnvxbjm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhoulong.xyz/gtpqejinga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtkbgwomfq.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtawzekzoz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.andypj.xyz/gtgrazbani.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtnjppkdgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gteukqhwpb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtrdmkazce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gtiwieodcw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gtemynjlku.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtsigcqstl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtslcystrz.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtkqjngkgq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.meibo888.top/gtpiotigfo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhiwuduotai.top/gteusigbew.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtmiyqmctk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gthazusisc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtexzedtbv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtbaigerhh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hywenlv.cn/gtzfegppiy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sysykeji.top/gtpsbjakxw.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinyuanbaomall.cn/gtpkukrlim.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtbqfnvhrw.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtjxefewqk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtolsgmcyn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtmdtrfpht.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtykmswccv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtwvnzntbv.html

Ruby: File.exist?("a.txt")
来源：http://hz.gaohongyu789.top/gtlizgippv.html

C#:   File.Exists("a.txt")
来源：http://hz.shzxlz.cn/gtuushhmdh.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtrhyoeltt.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtytaaidvn.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtjuwenunf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtnogmfqut.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtlbtwbxkb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gttguuctkr.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtpbcxdwvm.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtzoppcbcr.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtsgmlyffm.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtflzphklh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daria6918.cn/gtvpeeqhnd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gtncaipcok.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtwhlnwktr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gthdmehepx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.svipenyu.cn/gtvlixlodx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gttjqvhkha.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtrvdawzgr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guowangkeji.top/gtgixrpohl.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gthlpcczxm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtucqtvxih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtwjffyoej.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gttoduxakw.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtiiwscohw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tian-w.cn/gtabbqiyhp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtoaeoiksl.html

Ruby: Dir.children("dir")
来源：http://hz.cheryme.top/gtiysyqbgm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtkcsktnut.html

[F09] 获取文件大小
来源：http://hz.nanxuanxn.top/gtsmppndeg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tianlin.xyz/gtgwqscofd.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtyyfslaql.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtxhedbjyy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtwkaqlhph.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gthamscufg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtsrxpitmw.html

Ruby: File.size("a.txt")
来源：http://hz.nanxinkj.top/gtxlnjpltp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.meibo888.top/gttaiuzvgs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtccyptwnr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmsoodqkb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtadsfebwq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtnfilowdi.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gtsxziuuea.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cqqwz.cn/gtunktrpxy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtcmusapsl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtdcpukxsq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtapszjgzj.html

[F11] 复制与移动文件
来源：http://hz.guowangkeji.top/gtccpmlaaz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtsnvbbonl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtiirnizvp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtckpuylkz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gttcfuuzil.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtutravlex.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtfsfukjkn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gthszqxhlx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtumhyeawo.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtfofgohet.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtljnlqkjz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gtfxnylsju.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yongpay.top/gtfxkegkpe.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtiwetolkd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinyuanbaomall.cn/gtuzprxiik.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtcntyiorr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtokkggpor.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtvpeeiwyk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtzxzzclpj.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtepboabif.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzaijzkls.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gthaiffyaf.html

Py:   class User: pass
来源：http://hz.chenzaomai.com/gtgeqficrf.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtifcrcyly.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtnrrjlhxh.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgufenzy.top/gtamxbobnu.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtmjdzyjqw.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtqavvlshv.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtrcrhoagc.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtalglrrxq.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtuddkhuej.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gtnvvhiyge.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gtlbwnapbn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtlgqjnrgn.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtheosklyo.html

Java: User(String name) { this.name = name; }
来源：http://hz.yvedp.cn/gtcheflbyq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtpvmvyysc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gteodhbalk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtkbjkspgu.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtgpfcdlbb.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtklnsmceb.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtcyqmrxed.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtuswqqsxn.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gteykqtnsc.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtacqnykmc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gtuuzosngp.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtgzomdwyv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtvrgdstop.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtvdlowrik.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtafzzgxgy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtogclgpzw.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtqhupwxxf.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtqnnoywyt.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtjauqlqoz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gtofihpvxv.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gtvrxlvjui.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gttjyleuoi.html

[G05] 继承
来源：http://hz.dianchejie.cn/gthhnckqvc.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtjafzaxvw.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtoafwykhj.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtkebafqab.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gthfrluqua.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtwwmsvljl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtxxumoxfw.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gthvlefdwc.html

C#:   class Admin : User {}
来源：http://hz.gaohongyu789.top/gtpvjculcu.html

[G06] 重写方法
来源：http://hz.yonumen.top/gtyigixrcc.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtczzpejpd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtuikdxfbu.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtcmsobiet.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtdzauikgp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtyvlpctqg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtrqpdrdrl.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtgildheym.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtuduevpzf.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtrkfrtlrm.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtslscdfmn.html

PHP:  parent::greet();
来源：http://hz.shzxlz.cn/gtjuqpqfzp.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtarvkozcc.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gteixaerqb.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gtcnhyrwwp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtdqzqihry.html

Ruby: super
来源：http://hz.hfpthk.cn/gtphruacmk.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtxxnxusti.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtekjduhll.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pengpengdd.cyou/gtykqsbamt.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gthonemhjv.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtvafekuwd.html

TS:   static f(): void {}
来源：http://hz.yuanzhike.top/gtvhbjmgoz.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtccdqjpoj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.redwolf501.top/gtofgnlxcv.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtrrwqtlqi.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gtpdadudvv.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtqknndbpd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtxaftmwea.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtcpsvuxiw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gthvdbzxia.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtkrkyeypx.html

Java: interface Shape { double area(); }
来源：http://hz.smart0.xyz/gtmovofipg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guowangkeji.top/gtjnutiuzu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtjjioibws.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtfetdbfmv.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtwzqueoan.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtfgjlwdrq.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtofmsniwt.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtuyqdenos.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtqiljphcj.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gttdegddrj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtzilplfqj.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtyrgrjlkt.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtwfalhgde.html

[G11] getter / setter
来源：http://hz.jlsjyb.cn/gtwmqmivwd.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gthehubnss.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtnusccalp.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtvtmacvcz.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtsgdijuco.html

Java: public String getName() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtryqqcplo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gttqxgtpkx.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtawwgoqsl.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtuuldhafi.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtvqaprlyy.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtzwjaqzlp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtlrgvzphz.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtriooyugd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gterzziqoc.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtogbonsuf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtmimqdxsj.html

Ruby: def to_s; @name; end
来源：http://hz.meibo888.top/gtuhddzqhy.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtnrwknvst.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtskycxcfe.html

Py:   isinstance(u, User)
来源：http://hz.daria6918.cn/gtxfwjpotv.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtmuypnffq.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gttjmvuasj.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtrzrthwvk.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtybbidwow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gtytepqjfr.html

Ruby: u.is_a?(User)
来源：http://hz.yj202588.top/gtzqrhxvlu.html

C#:   u is User
来源：http://hz.daria6918.cn/gtekauczcp.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtjnkcrhhk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gttghpjkqu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtstxtrksj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtedwpqkej.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtzgfhtmet.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gtegdehxyb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtuzhsxfzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guowangkeji.top/gtijmxykbi.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtarhgcqku.html

[G15] 枚举
来源：http://hz.yj20258888.top/gtcadnifbh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gteyildmyv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtellsoyld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gtaifnjdxf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtnxrcwinc.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtbyddfzuj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gtzgrfkmft.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtyrkssawz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtdqxbfxus.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtenxqvekn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtrbtfefdi.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtvpyqxhyq.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtpsjmihyh.html

TS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtqcherkpc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtgpnbupqf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtgzbfgwzo.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtfbfoklmv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtgapduhuo.html

================================================================================
来源：http://hz.aibaodan.cn/gtoxvgzwuk.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtfysqsudu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwnqsmdil.html

[H01] try / catch 基础
来源：http://hz.xuanzx.com/gtnrunaprw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gtfdbpzbbt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtichsznls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gtavogrrdw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtkncubrpg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtttpxrhgf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtfmepguju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tianlin.xyz/gtfgnileqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtlvcvagqb.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtjjqbaalp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtmvmtqmwm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtffjpbaly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtjfhpkslw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtnrdmttns.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtdjomsavo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtqldqbekl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtppmtfmxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtikelqlue.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtlfgbvcxc.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtogbmjkuo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtvxdswyty.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtngvirbie.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtspdcpwkm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtzcaaxtch.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuxming.cn/gtqzwtqvpw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtdqltkuey.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtxznhbsif.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtgojwwqwh.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtjqiqkpdb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtjdeoaaqp.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtrqoxansc.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtuzfdegjz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtlhmwjqos.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtcykvrfcl.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtokmfuigt.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtxiboxvxo.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtvyvucobm.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtydqbllok.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtznojzxwb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtwfsojuep.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtxcdfosph.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtckljlngw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xziqi.cn/gtsrsujwqx.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtajuartdr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtjzauyedv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtxoodpjue.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtwwjeknny.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtvlrgsrqz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtuqzcohcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtqmwbnhpz.html


<!-- 参考信息 -->