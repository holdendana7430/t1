代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtoziptndb.html

C#:   File.Delete("a.txt");
来源：http://hz.wangshuangyany.cn/gtejeisirj.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtjauhxxly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtvlwhrxbp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zycfv.cn/gtphglypoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gteosvonif.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtmvoswscd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtxuyskxen.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenlongwang.top/gtjlolmkxi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtwwxzgmia.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gtsjcaarir.html

[F08] 遍历目录
来源：http://hz.yuanzhike.top/gtdorrqhix.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtdmrsgqmi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtwnqablfl.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtktmzudry.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtjimbscvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtjbfwxdov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtpjmhjcbm.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtjjxhhhrl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtjqvxghcu.html

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gtnynelhkq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtdbsxopcj.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gttqwhmjgf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gttoodfxiu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtgjiipgsw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtehlnlnta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtackdgtqp.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtoaxjbvfr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtlvpxdfob.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtoslnbjtb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtsrsizeob.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtviqqslrt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtrvoapuaz.html

TS:   path.extname("a.txt")
来源：http://hz.sxryk.cn/gtzangtgwo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtxpnzyuyh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtpbergoau.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtgbxtcrwu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtnlqueaij.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gttzatckdl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtztilendi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtwkmootav.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtbtceifpr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtyneufgcc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtpfkrsfsh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtxltvxtxt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtyhbtwquv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gtbiliprvd.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtwtvtmjlx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gaohongyu789.top/gtaobgrvqy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.feifeiyinyue.top/gtusqpdtvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtsxolrgxw.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtlkyxqjyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gtqaeqcerj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtorpvfbmj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtuvmohnuy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gtrwletezl.html

================================================================================
来源：http://hz.ppjwa.cn/gtxyqldxah.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtntumbwho.html

================================================================================
来源：http://hz.guowangkeji.top/gtztkmurvi.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gtnkvppjaq.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtjocsiias.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtrhhsdati.html

JS:   class User {}
来源：http://hz.wangdashe.top/gtqwvoafea.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtuasinpoe.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtabeqlslo.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtpbrrugyu.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gtcktvjxir.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtsgmqgfbz.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtsggeyagf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xylfe.cn/gtxxqxkpnt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigfzy.top/gtjdxtzktt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gtelbgzlyl.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigfzy.top/gtscnsdccr.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtejntcyzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtubgrmpho.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtrgzqnxff.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtgcfkvyjl.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtobfgfzhu.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gttaswqhjg.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtiipdesbn.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gthptglvif.html

TS:   name: string = "x";
来源：http://hz.yuxming.cn/gtnrqouald.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtsnyloysp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtqlwyozac.html

Ruby: @name = "x"
来源：http://hz.redwolf501.top/gtlmautvyg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.c1oappe.top/gtsfgozdpa.html

[G04] 定义方法
来源：http://hz.daxiang520.top/gtecvwjtjb.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gthxhkenap.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtwwbobyzm.html

JS:   greet() { return this.name; }
来源：http://hz.jqgufenzy.top/gtjromxdqa.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtjycszuke.html

Java: String greet() { return name; }
来源：http://hz.yuxming.cn/gtmsyidcem.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gtkonwiyel.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtetowavcb.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtnolduupc.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtsfvtrhlr.html

Py:   class Admin(User): pass
来源：http://hz.sufxvd.cn/gtoqehcqji.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtezcwlbvz.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gthyzpeihj.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtmjfvlibv.html

Java: class Admin extends User {}
来源：http://hz.xinyue.icu/gtzshcdoxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtessnngbj.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gtljelftdz.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtzomsucqv.html

[G06] 重写方法
来源：http://hz.xziqi.cn/gtvebwzmyt.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtyqxgftim.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtbpyvbmwl.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtzsaxbjkx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gttbenmfys.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtebbucgnc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtbwnxcebt.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtzzycnslg.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxinkj.top/gtnphpdemy.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtlalckfeq.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtdzyxhnoi.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtaqqfyuoi.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtgzkstbhl.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtwmbaqjqq.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtcwehcguq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhengqikj.top/gtqpwhvoou.html

Ruby: super
来源：http://hz.hnqzz.top/gttkfdqghi.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtndtuhfph.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtvsatujxs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtfoavchzc.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtimjeufmb.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gttdcanory.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtbhyymcye.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtscueezei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtdpjgbzim.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtcjkgrhjj.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtkmxijpat.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtgqussswe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtnxwvwtcn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gtcobgqmiu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtmutgjbys.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhixingplan.top/gtrsoeyqoh.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtovngzdrd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtfqlvrmhl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtljgzedpv.html

C#:   interface IShape { double Area(); }
来源：http://hz.sweek.top/gtrbgliqlq.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtvpbnogkc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtfcifxerx.html

PHP:  public / protected / private
来源：http://hz.yuanzhike.top/gtswnqocxu.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gtazyuwafl.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtcsskknex.html

Java: public / protected / private / 默认包级
来源：http://hz.aibaodan.cn/gtfdpwtron.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtvwfihhvt.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtnvkwfiqb.html

C#:   public / protected / private / internal
来源：http://hz.zhongyouzk.top/gteedstmxo.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtrthprujv.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtuijzztkl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtxnejlgaw.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtoiwpnvqh.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtxksxzykl.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtvnsyubkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtxvnaqvns.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtgmknyzac.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtvsmjwngx.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtiwpxcoyw.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtookunpnw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtaikynqxw.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtiztauwbw.html

TS:   toString(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtlaxrwazl.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gthobgsbqr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtueuvnjyt.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gtqeqfzpyk.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gtvxtssnrm.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtgrwfvmkw.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtwmvzrslr.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gtwzhutjdl.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtlwwqezga.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gtbflwdyqb.html

Java: u instanceof User
来源：http://hz.sweek.top/gtnhmpenko.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jiagoushi.top/gtjqwxcjrz.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtcqedoivw.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtkquwjmqj.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtcfnyytox.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtaqvpdzrz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtvrbsazpk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gttijhrtlt.html

TS:   type User = { name: string; age: number };
来源：http://hz.xinyue.icu/gtupmwjzwc.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtejngtgxw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtcfbuahhi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtdkyinhbg.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtofdpcoyy.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gtcceozyyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gttjimlatx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtbbrbvbyz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gtxlblagbi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtzjjpeuck.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtanhuvvss.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gtrgogmuqn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtmpwklvdd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtpianrlfq.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtvdnigksj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.9152youxi.cn/gtjfkfvoeu.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtqwlpailq.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtgshdwilk.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtxfyxumkw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtsmzemnpf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gogol.net.cn/gtkvdlygnz.html

Ruby: obj.instance_variables
来源：http://hz.xuanzx.com/gtulcuelwr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtgpmfkrik.html

================================================================================
来源：http://hz.ydzc1.top/gtjonwlpoa.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtrwqjeqrr.html

================================================================================
来源：http://hz.dianchejie.cn/gtnpwzgezb.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtapucnqrq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangdashe.top/gtzuzckfhx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtpmvxntrb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtkrweekwn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yangfankeji.com/gtupruarsh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gtxieqmnfl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtkwedhnur.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtvscukcqc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtmuwflcvv.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtfhqsmztq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtcteglgbw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtdzgwfijt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gthzfhugpf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtgzdjclze.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtfkvlbscl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gtjtersxvu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtncalxusa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtgvcrcpju.html

[H03] 主动抛出异常
来源：http://hz.jinqigfzy.top/gtwpyqwqst.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gttdwdjesz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtxcgornwu.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtmcsqolia.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtvdznjayu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtlvlntsyu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtxhewnjti.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtojxtsqqo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gteluqzrrv.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gtcjmbuavb.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtbtyphgwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtvqjnkttb.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtqwwofdhe.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtvwctgcac.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtbpjpuocz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtiqdiukeg.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtrkbxwhjk.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtlvwpssuj.html

[H05] 捕获特定类型
来源：http://hz.yonumen.top/gtkaeqkvqg.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtxecpmrpp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtxmtbbzch.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtjefvkvdh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtmiwvcicq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtixobfqge.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtiefxhadc.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gtthbsopgt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtrcokpxue.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtrsdoasqo.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtqbxtfnzr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtuyfnqyrs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtpbkuegdy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtocemhbea.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xylfe.cn/gtgyxqjstd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gthyugfrsj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtwzxxuvhm.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtrnewpomh.html

[H07] 断言
来源：http://hz.xziqi.cn/gtctstdnze.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtkytclzfv.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtmkbrhyms.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtiwoevylp.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtwfmjeqvk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtfiambvwh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gtzeeosoux.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtfultxfvf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtevhhhzny.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtcrmlqvcw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258.top/gtwmkuhyoj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtreunbtak.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gthrlvtoit.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtkxvhgnlb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gthyeukuqb.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtplgcpoch.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gttkifpjtz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gteipkqudf.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtzzhrqyfc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtgcaqtjxv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtudnzodrn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtgyjurmtw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtlbzyttam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtbdiuxskf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gtposzrouz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtungmzkpp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtifczvvqb.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtyinwpoun.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtoqdjwrio.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yonumen.top/gtwapdspwn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtithronor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtahdrpatc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtmjxafmzw.html

Go:   defer f.Close()
来源：http://hz.cheryme.top/gtjvlivnmn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gzhubu.top/gtrpxajjme.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtmdkoltlc.html

================================================================================
来源：http://hz.redwolf501.top/gtrhhwslbg.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtbyzdruom.html

================================================================================
来源：http://hz.yuanzhike.top/gtxlrfgwbv.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtepdubkvw.html


<!-- 参考信息 -->