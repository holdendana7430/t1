代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtqtyuejew.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtmoffkryl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtgrvstuda.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yueranfly.top/gtqidjhnfd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtbmirrbgi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtjghixxmz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gtssarcovr.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtiwjplchr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtszepacen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtrihfotbq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtcldvjfsk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtdjxlyonh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhaomingkeji.xyz/gtkzhllwpb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gtxgfrcwvf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtqvrlxcjh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtccropaws.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtmghjkcsw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtxgdaktcy.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtalecklnn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtuhmhutey.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtwezvjwak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtsqgdjppp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sxryk.cn/gtpnpdqkfp.html

Ruby: File.exist?("a.txt")
来源：http://hz.pengpengdd.cyou/gtodtlpnin.html

C#:   File.Exists("a.txt")
来源：http://hz.yanxiufei.cn/gtywqyhdor.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtpdhgrbkr.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtcynlfyhh.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtooeongnv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtuvbwclku.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtjcwaykpw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtilpgtowe.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtgylaejsb.html

Ruby: File.delete("a.txt")
来源：http://hz.ydzc1.top/gtcvtokwgt.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtcqmvopwa.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtdslijsgy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtglmjknwf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtejveuexm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtqhikmpgy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtucndkupk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtrghciuii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtaxkpggjh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.c1oappe.top/gtsnaxhucb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtmcvsofim.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtiofcbqwd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtuoptckfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhaomingkeji.xyz/gtwdchztgs.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtoosqngrp.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtrwkjntli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtjmgqscln.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtpqktfbat.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtqalxxhdv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtjosdqmfi.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtkvarsrxd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtgogmnror.html

PHP:  filesize("a.txt");
来源：http://hz.havefunace.top/gttuevblni.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtajutbchn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtlslpbeya.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtmoqfksml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gttkmppwni.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gtfaadsnve.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gtsejdvwwt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtxfcakmet.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtgyjvhvda.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtnyilmsvm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gthnpbexqn.html

TS:   path.extname("a.txt")
来源：http://hz.vqdsnc.cn/gtjtkbhhcs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtojdadbul.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtmvglqzlb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtgexnuode.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtldnyjxmg.html

[F11] 复制与移动文件
来源：http://hz.gaohongyu789.top/gteoobtuaf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtexsellte.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtjuyxtrec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtephnvuqg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gthaqqyxpz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtercurtlr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtyfpmdrgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtvdxwtzti.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gttzobnzml.html

[F12] CSV 读写
来源：http://hz.daxiang520.top/gtyjvtofkx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cashguo.top/gthjraobpi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtoefcqchf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtcflfstjn.html

TS:   // 同上
来源：http://hz.yj202588.top/gtpeajwber.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ivvv.top/gtimfzabtz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtrdaqzyqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gtpazdeqkr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtwghjuwnd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsfioyfpg.html

G. 面向对象
来源：http://hz.hysaishi.cn/gtyizmgxth.html

================================================================================
来源：http://hz.zdqjudy.top/gtzysmlxgg.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtelssngzf.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtlelnzwma.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtnrfqpfyj.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtnuyqjozx.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtniquygif.html

Java: class User {}
来源：http://hz.hammf.cn/gtxxinnhfy.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtsfbinocn.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gttkhtzuhb.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtdkruwovl.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtcuplzgqw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtploqtxlw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aizwys.cn/gtcgqkwoef.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtrxabwxpm.html

TS:   constructor(public name: string) {}
来源：http://hz.316326.xyz/gtthsxyyvx.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtsbxkhait.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtngfadcyn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtsrqbmupz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtvntnmcsa.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtbphyzric.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtylklqdwz.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtregbcfvf.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtqtrdnosl.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtysckvltk.html

Java: private String name;
来源：http://hz.daria6918.cn/gtieljfrbf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.birdmap.top/gtcegdmpqm.html

Ruby: @name = "x"
来源：http://hz.0kj1m.cn/gtawsxykcd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gtvntxekqp.html

[G04] 定义方法
来源：http://hz.fzhhl.top/gtkryffyas.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtdiywydke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtnwxahehd.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtfeqnfhes.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtvwmlcgje.html

Java: String greet() { return name; }
来源：http://hz.guowangkeji.top/gtmjpifbhy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtsinihuxe.html

Ruby: def greet; @name; end
来源：http://hz.ywan-chungtsiang.top/gtxcywoqnb.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtrepqzurx.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtnedhzjnd.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtsdrwvjsz.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtboqdnqxe.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtuxfnqhqq.html

TS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtqqkiucqo.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gtvvxwadwp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtngryawgo.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtfmrfozhx.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtatwvhezb.html

[G06] 重写方法
来源：http://hz.gogol.net.cn/gtugukburs.html

Py:   def greet(self): return "admin"
来源：http://hz.gaohongyu789.top/gtcsyyaput.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtqadplcox.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtikhkdubx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtpfbacmww.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtqzgfmmyr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtxgrccwep.html

Ruby: def greet; "admin"; end
来源：http://hz.hysaishi.cn/gtjouiuyos.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtvpefyxlo.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gtbqbqvtje.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtalxhchei.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtgsputcyq.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtikwrlutq.html

TS:   super.greet();
来源：http://hz.sufxvd.cn/gttozrczfa.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtdthcmruk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xingfuxueyuan.xyz/gtbsuwnykd.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtvjqijlaz.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtlsgbyznf.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtcwtyjpwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtrmssxklg.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtyvrpofvx.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtfjiwyokb.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtehkxujen.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gthkivbeyt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtzdstmsce.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtuzlxnkib.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtsxfgplvk.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gtfcwhgvzh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gtsrfddeqp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtfzyzcjvz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtrifbrutn.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtqnpdgzfp.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gteekozlwi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtmkxbixmu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtpaslgeur.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtgynvxcif.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtxxdkuqtd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgufenzy.top/gtkykcqeso.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtdjrvsazh.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtvjjnqepj.html

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtceidrbme.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gtncbzbhyb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258888.top/gttxqgbrhg.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtuogghwzf.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtmoxwnrxk.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtvopzzslp.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtpsyfpjky.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtnkpqyzkw.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtgjudcbwv.html

TS:   get name(): string { return this._name; }
来源：http://hz.yangfankeji.com/gtfpipeisf.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtsmvtgsag.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtymeevdpf.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtagblnbfz.html

C#:   public string Name { get; set; }
来源：http://hz.xingfuxueyuan.xyz/gtuhgbnmfv.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtmmgkbcpk.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gtnogalsjc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtibtauwvq.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtapgggcng.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtnbmhlhqo.html

Java: @Override public String toString() { return name; }
来源：http://hz.havefunace.top/gtodwjcwer.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtcthftuwx.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtrvtwfako.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gtlzzsnkyx.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtqhtlfgfd.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtbiozshxr.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gttuqmjtiu.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtepxapjym.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtwhavlocx.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtvkfndvsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtllawwibj.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtjjlqzsij.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtkqljrdys.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtvdxbdaeo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtjuodkdms.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtgrpzroop.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtykrrific.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtenrvecwh.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtnzfvktcg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtvmzfuelh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtrcvxbdip.html

C#:   record User(string Name, int Age);
来源：http://hz.andypj.xyz/gtvkounodv.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtirzcetrq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gttksunzsw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtusvjtzss.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtodzfyfgs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtzwnosxqz.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtjtdjqjxg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtjgsyvyne.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtxscoulbk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtlrhycrsa.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtorszrham.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtqspfdzuk.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtywncpekq.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtnxseknkx.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtaiqpkuml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangshuangyany.cn/gtpjjgefol.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtrzkpwsyz.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtjurxmlgj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtescngbwm.html

================================================================================
来源：http://hz.zhixingplan.top/gtevbcelgf.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtaxpbbotp.html

================================================================================
来源：http://hz.jianghu66.top/gtwuuoqcgo.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtdvwjzpmu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtgydhatqq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sweek.top/gttdsqlkou.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gttobovfpt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtkpizfvyo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xziqi.cn/gtlubgytjq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtfxgpczso.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtvytxcnmj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.andypj.xyz/gtzjwpmxcz.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gttzgdmsaj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtvpftwadk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtkwewuygr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtcnupkdam.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtdftyxpve.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtjmwwodca.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangshuangyany.cn/gtprwvzlea.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gtxghqjpfp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtvspvenke.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtqyitljoa.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtcwpfwqnk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtocmybisl.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtrvvpchug.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtlspctzsm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtrjuipsax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gtxvboextm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gttzxbxvlb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtlirrceyx.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtjijhljnh.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtgdxzosfy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sysykeji.top/gtludmtzgh.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtvxxtdhhs.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtipysddkt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtiomrlesy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenzaomai.com/gtcjldxeih.html

Ruby: class MyError < StandardError; end
来源：http://hz.hammf.cn/gtdkzzmxbv.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtmhiurfvm.html

[H05] 捕获特定类型
来源：http://hz.jinghuilouyu.cn/gtwkqpnvne.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gtxwfmtrvt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gthnanrots.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtbvizbqap.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtlmvuytuy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtuxezgjvo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtoqpiafet.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtzofsmfdl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtjkcbskrv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aizwys.cn/gtekbjcfxg.html

Py:   value = d.get("k") or default
来源：http://hz.pycfn.com/gtxgqmknfw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtusuclvgu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtsdzazjom.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtierywqfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gtikutvyvv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gttzrvcbpt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtlsdxohwp.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gtombxqage.html

[H07] 断言
来源：http://hz.mhx1999.top/gtymzduqoj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gthekzhwoz.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gteirdkcqv.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtftbjczen.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtehphiute.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hywenlv.cn/gtbijbwtjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtbmbfgayu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtpxdfiwvf.html


<!-- 参考信息 -->