代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtyifdphfe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtjkesqmjh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtqsujylgv.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtsdgrfseo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtansutayk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtdixoanys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtpvsycurm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtrrkcwjor.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hfpthk.cn/gtwstysdgj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgfzy.top/gtggxtqxnp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gtfufsffwh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ybcxt.top/gthendlhva.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtoomybswn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtoyubgzyq.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtqacjhaff.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtyealjfuh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtwiaqtpod.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtjcwyrvlz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtwqpmnwmf.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtsyqfoppw.html

C#:   File.Exists("a.txt")
来源：http://hz.hnqzz.top/gtkmrcgmvg.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtlezdnxtc.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtzjsxfoyq.html

PHP:  unlink("a.txt");
来源：http://hz.gogol.net.cn/gtexoiuxhj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtfljkplws.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtjmjpgbjc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtldoctjjq.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gtlfxybqes.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtoqxmqqkj.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtbmxyhwsp.html

[F07] 创建目录（含多级）
来源：http://hz.zdqjudy.top/gtjnzqjvkf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtvxxwhpzo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtlanssiti.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtsnyrkobp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gttcxkywmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtdsokkbwq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtplzdaisu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtcszfqpry.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cdnleiting.top/gtdczgtoth.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtyrbfptob.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtlzlfimhr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtyctfamvv.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtbtawoxvv.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtxhzxfgra.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtcnyjuude.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pengpengdd.cyou/gtwrjpvbay.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtntyhtczl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtbasjgymq.html

[F09] 获取文件大小
来源：http://hz.nanxuanxn.top/gtaezsaznu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtnkkvqdhs.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtsijisuip.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtpklfeyth.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtofkttkxy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gthbkurjzb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtsiuevheu.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtxmcdeslw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtjlzxswdh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtyovzlgip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtwhgmputh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtavasplvj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtayhkrkfj.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gthrtwpsin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtuzhtbaej.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdkswqwpa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtabtgiuct.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtecswycom.html

[F11] 复制与移动文件
来源：http://hz.yj202588.top/gtptzsxsnv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtjjnlolkf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtiryusnzk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtgvipckxe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gthuecfose.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtskimbfwr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtltljakdo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtlkmxjrjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtoxojgdwn.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtojzzbter.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gteggwgqfr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuetiantiany.cn/gtpkgaxpko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtdjjridtu.html

TS:   // 同上
来源：http://hz.pycfn.com/gtkkgrpocw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtsnnoddab.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtpsufkvqf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gthvcskijp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtlbxfieso.html

================================================================================
来源：http://hz.cashguo.top/gthezmisvv.html

G. 面向对象
来源：http://hz.ydzc1.top/gtiybmdhxg.html

================================================================================
来源：http://hz.jqgfzy.top/gtqtkngkdt.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtlncetkgf.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtfdiitqeb.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtydxrqapn.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtacezbxbd.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtwfclybnt.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtyqgouoao.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gtrxlhqnrr.html

Ruby: class User; end
来源：http://hz.hnqzz.top/gtuhksjtta.html

C#:   class User {}
来源：http://hz.fengsongda.top/gtlzhwnlbr.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtfnpxqngf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtqfapstqr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtubtutqej.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtvqgmrkwo.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gturbblzcm.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuanzx.com/gtixodetbx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenzaomai.com/gtsdkjyvsi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gttfmmiiqd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtfnesmuxu.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtvsokvvqt.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gttkhmndtc.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtveedfxhr.html

JS:   this.name = "x";
来源：http://hz.52xcode.cn/gtegjylrup.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtvyjsociu.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtnktktyxl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtamylhirt.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtjmkolqvz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtupsuzsre.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtustndgil.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtbxuebzsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtrjcclyoa.html

JS:   greet() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtdcjyjulu.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtandzklbu.html

Java: String greet() { return name; }
来源：http://hz.hywenlv.cn/gtszvrbyrd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gtslmdxnat.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtuckfbdxp.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtdjxivxuw.html

[G05] 继承
来源：http://hz.nwbrower.top/gtuixrlnrt.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtfjtghaby.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtzytkkqvk.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gthhhasizj.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtzhbabwiv.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtkivpswgq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtvxfrsdjo.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gtdrtirlom.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtoxygwjmo.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtonfjillk.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtimrhjowv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtgozzvyyx.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtenuqmsxb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtpftefnfw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtbpltlllo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtfxcepmob.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtehlltjry.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtjccqphva.html

[G07] 调用父类方法
来源：http://hz.52xcode.cn/gtfihychzv.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtxuyhxqds.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtcbnobxjj.html

JS:   super.greet();
来源：http://hz.sweek.top/gtndbzgeht.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtrxixkgem.html

Java: super.greet();
来源：http://hz.shuidangran.top/gtrfaliyvg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtyxrzflmm.html

Ruby: super
来源：http://hz.jqgfzy.top/gtiqxisngx.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtlxzblekt.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtnwfgrbzu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtlhxepxlt.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtfvrwobgx.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtowsrgdfh.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtrbjqdtev.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtthzssliz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aizwys.cn/gtrcbvbwab.html

Ruby: def self.f; end
来源：http://hz.jinqigfzy.top/gtkywoiuzs.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtcwijoban.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtcfcrbivp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtzwxelwdl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtxoizlcls.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtalhhbqxr.html

TS:   interface Shape { area(): number; }
来源：http://hz.cucudq.cn/gteiifbunp.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtnkdrsqdw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cqqwz.cn/gtfsmxfagq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gttpxerxvg.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtrommcsfp.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gtkgjwwreh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gthptltmfp.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gtscpopdyf.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtshzzktym.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtmkpretqg.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtnkgjgbim.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtfsczykre.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gtqiwtujbz.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtorjwodnw.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtvifjlxqy.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gteiimudyc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtbmtexvis.html

JS:   get name() { return this._name; }
来源：http://hz.pycfn.com/gtttmznrgj.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtbluuqgqw.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtghrvbhlp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gthrgxmmmk.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtqlnxmsll.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtrjauqram.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gtvptmdbwa.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtswwzmgmt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtkxeqiumd.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtwggypvqd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtbkjonhyv.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtyrosmfeq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cheryme.top/gtttlmrher.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtwllvemxo.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtpvsoazsh.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtrvtmlqkr.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtwhqmllkj.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gttireigiv.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtgeflvvlq.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gttrtfzasf.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtowbqbahf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtfqqvzhsu.html

Ruby: u.is_a?(User)
来源：http://hz.aibaodan.cn/gtrhbfeebg.html

C#:   u is User
来源：http://hz.yuxming.cn/gtrdjgigej.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gtfjywactf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gthqctajpm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtjcwzdtaq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtvnzcxtzp.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtnzupctsw.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtzsncuddw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtgklwgwxs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtultmpted.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258888.top/gtpdiiazgy.html

[G15] 枚举
来源：http://hz.sweek.top/gtmqtcnedp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtajvtyalf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gttvvjatab.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtnwojsebp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtribbcalk.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtiohuqafv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtmxhargdq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtqwhjuzmg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtbvopidkz.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxinkj.top/gtlvdjiwnu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtkpxuseua.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtnbqmtcbm.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtyhhnazwu.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtkonemjzm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtowjmezng.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gttgiltlbp.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtsfvlpaqb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtqqsciplo.html

================================================================================
来源：http://hz.xinyue.icu/gtjppjfxae.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtdwnbuhyp.html

================================================================================
来源：http://hz.daxiang520.top/gtwodmeupb.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtfgzhthvx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtrlrvzycq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shangyingyoupin.top/gtxbteiphl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtthpzbiyx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtidiqjquf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtvilcgdwn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtupqfwxju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtymlkfepn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ppjwa.cn/gtwluvqrbv.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtelskkqfs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtickzwcbn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtfxhgddar.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtgododnld.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtilqxoiup.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtoozrdixr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nwbrower.top/gtsgkefezp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtpzmmfwbe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtogiojgsl.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtzsccoayj.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gteooiunzc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nwbrower.top/gthipmthfn.html

JS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtwadvjwxp.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtzgwtcbuk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtnppgbjxx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhaomingkeji.xyz/gtkfosbwkr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtzcyvcrnm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtbtjwnwoi.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtqwshfcpo.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtjtdvdqrt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtnewhmgoi.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtvadmljid.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtcqkstwcl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tanke756.top/gtypctcpqk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtzmavfeed.html

Ruby: class MyError < StandardError; end
来源：http://hz.aizwys.cn/gtjdfmlcgz.html

C#:   class MyException : Exception {}
来源：http://hz.birdmap.top/gtgugnyckd.html

[H05] 捕获特定类型
来源：http://hz.cdnleiting.top/gtyfdslwlr.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtpgookgmg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gthnbhbqyz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtmbkdvmzv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtjwbrgiqe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gthfbfjtkd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtgbrqlqcf.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gttnzkpwby.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtcqhtmzpk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtapsiagow.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtfzbqcomm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtrtqvvqha.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtcjtvrjoh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtjbqaiffx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtegwjwbsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtybcrnboq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtbgpydhua.html

C#:   obj?.A?.B ?? default
来源：http://hz.xziqi.cn/gtbxmknjbg.html

[H07] 断言
来源：http://hz.daria6918.cn/gtisybubtc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtccayaxxh.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtxzonovkz.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtuaoqbmvu.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtdobxsuca.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtdvrwyxoh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtvubyaunx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.snrcjt.cn/gtbnlpitno.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtosqfpntj.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtqfwczvhf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtsuprvnmb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtndmwznyu.html


<!-- 参考信息 -->