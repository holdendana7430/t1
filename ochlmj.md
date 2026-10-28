代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtmrsyemur.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gttghagjmi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtpkfdputv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.0kj1m.cn/gtgrsvzlym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtyhgvndre.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtixuffpnt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtmutrbttq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtjtmmlzld.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtomqqnotd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gttayfvzfp.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gthufiagqt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtdpurjyjz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtrnqviifm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtohjuxknr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtnyisiixk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuanzhike.top/gtpfnwpitv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtdzvoruhu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtnviasalj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtckdatyzv.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gtdofbruwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtpaeoisvy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gtnsuddswt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtbxfklzke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtwiqsckov.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xingfuxueyuan.xyz/gtylzblosk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtkmarttuh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtpuweukmq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtkokfagmo.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtwsivnsbh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shangyingyoupin.top/gtzbgtuixr.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtlyrhfatm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtzktudjka.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtdnopzgms.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtegobezdd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guowangkeji.top/gtonksfxqs.html

Ruby: File.exist?("a.txt")
来源：http://hz.yonumen.top/gtorgadwez.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtdtltzpdo.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtjqxjcapi.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtxwzawkcs.html

PHP:  unlink("a.txt");
来源：http://hz.aibaodan.cn/gtuozvcfcx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtlvuxrrfu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtoomaweyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtyakhcjce.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtubvchqjp.html

Ruby: File.delete("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtogwqxfin.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtowwrxyfi.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtxtbfmhxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gtnondzohi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gtxgwqnbkx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtxjgpsphu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtgmsiaczt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtjxyezedw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtgkwirlyb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtpyzsphra.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtydjowkgr.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtalqezbxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtbgbofxwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtduenuzix.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtfkucvkln.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtzjnvncko.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtmahnvfpn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtasmluqlx.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtbzbdwnfo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydzc1.top/gtzsrhdjpb.html

[F09] 获取文件大小
来源：http://hz.svipenyu.cn/gtjgswsgdd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.kuanghao11.cn/gtocmkbuva.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gtbacovvte.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtjmayexca.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtrivwyubv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtgmhilnot.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtsntderkt.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtmzfilxou.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtsiznlfnm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtnsdfhslr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtosrtgrux.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtxwgcfrfs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtfrzckdut.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtdpmrfecu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtkysubuzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtaxrexsww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtotnxivie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtalrwrltp.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtygjahzmq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtwqhozejk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtyfzwwdtg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtvdabfmsc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtlnriqvfq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtaylnjhvb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ivvv.top/gtuqtmrgzs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtqtnrgcig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtpjgxjurv.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gthmnurpik.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangdashe.top/gturtrmlgj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cqqwz.cn/gtroquylsp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtawgmdhms.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtxxdnjfym.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtkrgatgyi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtlulnpvzg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtxshmihkw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtiqwwhdah.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqtfofpjw.html

G. 面向对象
来源：http://hz.yj20258.top/gtxtcphdsc.html

================================================================================
来源：http://hz.iojbl.cn/gtfeaimlyp.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtgtvhghrf.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtbvqsbbvw.html

PHP:  class User {}
来源：http://hz.shanyushiyangkeji.top/gtjjhzxwjx.html

JS:   class User {}
来源：http://hz.zycfv.cn/gthrfvlhbg.html

TS:   class User { name: string = ""; }
来源：http://hz.yanxiufei.cn/gtbhsgbnfj.html

Java: class User {}
来源：http://hz.bjfxy.top/gtccsciswv.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtbuuzsuuo.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtqkemtexp.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtlgdwpkto.html

[G02] 构造函数
来源：http://hz.jinqigufen.top/gtpyobcwzu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtsgjehahe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gttmhgcrme.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtjlmhutup.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtdqcadzio.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtwsfbayot.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tanke756.top/gteidlzbgt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtjswdfmjq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gttxwpksaz.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtdxpjsxii.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtpfqbeftn.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtfiewbrsf.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtwoonerse.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtqngovrxa.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtuytivzur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtcfoftwvn.html

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gttuzitjom.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtuhingfxh.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtmozqnxuv.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtfowmogga.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtjrqlapjc.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtsplsynaq.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtseznevgc.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtjhujmidq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gtkxkuqatt.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gthzmarmzr.html

C#:   public string Greet() => Name;
来源：http://hz.chenlongwang.top/gtcyrwhgjb.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gtttkkcbjy.html

Py:   class Admin(User): pass
来源：http://hz.nanxuanxn.top/gtixinyydr.html

PHP:  class Admin extends User {}
来源：http://hz.chenlongwang.top/gtnfhrxxep.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtjexnmblo.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtmqiwnabg.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtndmdcezb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtgebnvpiq.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtcetygdhm.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtxqroxerf.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtmtlsitio.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtvaqafgkc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtbxahxidu.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtdgnaugmo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtnmdhfypu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtrqzyotim.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jiagoushi.top/gtgsvzgkqg.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtiersyspo.html

C#:   public override string Greet() => "admin";
来源：http://hz.aizwys.cn/gtpnbnkckd.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtwbyujlat.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtqobgznwz.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtcgocimbv.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtncyrjhcc.html

TS:   super.greet();
来源：http://hz.52xcode.cn/gteldbffrg.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gtmzpyqzjb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtlqrvpoqe.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtnnauvfnk.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtiowodlab.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gtskvctmud.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtrapntigf.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtanvdievx.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtfggwyksz.html

TS:   static f(): void {}
来源：http://hz.jinqigfzy.top/gtgztoyrmi.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtkccrzvqw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtixkdrbaa.html

Ruby: def self.f; end
来源：http://hz.jqgfzy.top/gtjnqrhmgq.html

C#:   public static void F() {}
来源：http://hz.havefunace.top/gteytychok.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtmubjqucg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtiuzcuuqx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gthzejvhsv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtfnfumqzd.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtdbmrbdvz.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtjtmlohan.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtqkljosav.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xziqi.cn/gtbotcizca.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtlfxvuosu.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gtrbhfmpto.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangdashe.top/gtvsbqwtsg.html

PHP:  public / protected / private
来源：http://hz.meibo888.top/gtzbsoajbs.html

JS:   #private 字段；其余公开
来源：http://hz.yueranfly.top/gtcznwquyr.html

TS:   public / protected / private
来源：http://hz.cdnleiting.top/gttwqtgkbn.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtixagoibi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtejaietuo.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gtdmmzisbu.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtotkqynrz.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtdelhcmrt.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtfxmkpslg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gthximweir.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtwwaqrbvv.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtwlapgpoj.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtxdcmfusr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtrksimjqc.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangtech.top/gtgfmukysy.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtodxfqywb.html

[G12] 对象转字符串
来源：http://hz.haohaochexian.top/gtxtpbqxji.html

Py:   def __str__(self): return self.name
来源：http://hz.haohaochexian.top/gtfsobyfza.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtykqzuuan.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtbmaadndb.html

TS:   toString(): string { return this.name; }
来源：http://hz.iojbl.cn/gtigqomrhv.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtrlsnevlr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gthidlktuj.html

Ruby: def to_s; @name; end
来源：http://hz.yanxiufei.cn/gtkwgyzdqe.html

C#:   public override string ToString() => Name;
来源：http://hz.hnxiangtu.top/gtxqtxzmyl.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gticcotwng.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtiupatjcz.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtjnxmfjlo.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtbqfqugrk.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtscuhaqbj.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtuoemjdab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtueookuag.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtgnyuyauz.html

C#:   u is User
来源：http://hz.chenjidiqi.icu/gtvtsujcif.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtrtvpiqcu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtrmvbcajw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cqqwz.cn/gtdctowvzl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gttgnzywkr.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtjmtmhsoh.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gttghcotow.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtbgqvealt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtwgbiiewp.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258888.top/gtuezktdio.html

[G15] 枚举
来源：http://hz.yueranfly.top/gttvkmwkyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtznbenvcv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtzivpltxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.iojbl.cn/gtxhmtjpol.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gthbriarwi.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gttdhlkwod.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtqbqbjwxn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtudiopomw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtdwtuslez.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtrhhcfosv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gthwgagjsf.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtrabhrash.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gteywivryo.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtgnpvuitk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtkhkislag.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtbhohhpal.html

Ruby: obj.instance_variables
来源：http://hz.guannengcc.top/gtckdkehpl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.svipenyu.cn/gtfkzbfmjf.html

================================================================================
来源：http://hz.9152youxi.cn/gthdtthoie.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtnedtdcjd.html

================================================================================
来源：http://hz.jqgfzy.top/gtdtjoqnjd.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtgjkutwbr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtezxlaptl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtkhkonipl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtqrqpnchu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtzwtnoakd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.52xcode.cn/gtfunexiug.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtkpwwnvuw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtdnwalnja.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtytelcqij.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtxvwttnow.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtjmfmekmb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtokugadsc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtjyexdskf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtfctwqflw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtorqvsavm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gtpugctqys.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtslhzjcki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtqurfkgwi.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtcvcvypgm.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtmqajqlfr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtcxsgaijr.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtaxdvxmsh.html

TS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gtjmvbjosr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtfcklfzey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtvrhzerwk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtxsxlzttk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtpfmbmxkv.html

[H04] 自定义异常类型
来源：http://hz.chenlongwang.top/gthjvzsuxp.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtcxhxdweh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtoerfhfcz.html

JS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtlxvcephs.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtctjlacul.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gthreayoie.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtzfimisnc.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtchjvtyld.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtynibucps.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gtjkqtyoyl.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtwbfwwysr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtxjzwsydn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtzexsujeg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtfmrhorwr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigfzy.top/gtboyjbatg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtabktlaxa.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gtccqoveow.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gtshwsobng.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtmjiaghub.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtzgukizba.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jyoumei.cn/gtbdrcovgm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtmhuaklsu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtldnsonie.html


<!-- 参考信息 -->