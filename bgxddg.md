代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtirxkctfa.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtdcsemzrn.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtqgkhhrfj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.meibo888.top/gtkskirroj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangkeji.top/gtnpbpxoxb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtzofnphsl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gttvczkbrp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gthqkbjyye.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtgnogxsio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gtarozhsar.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gttqvmppfx.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtqtydknsx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tian-w.cn/gtihhwgmrv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtpxdehaqi.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtbeqhfkeu.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtgestwqfo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtpegdmkdi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtjtqnzwes.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtoxscgvpy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtrmvatkhw.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtzsharipw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtvxngszhu.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gtsprjpbsb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtclpdrfoq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtxcxwxwhk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtqmlihkew.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yongpay.top/gtiwztzfal.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gthjtkauxj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuxming.cn/gtgvhbbwtq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.bjfxy.top/gtdxwqnoss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtabmwuokf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtapqcfubx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gthwkfvacw.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gtkrzkimgu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.meibo888.top/gtsxoihgal.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttxjjqdil.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtzxgcmamn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtinvnkqip.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtmgrsekxl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtmxvquogn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtkwekvgff.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtlbcetavu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtqjvmveqr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtpwbhbkio.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtkrheavwz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtmcmglazr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtknzrwfyi.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtbbjbnazb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.redwolf501.top/gtnyxguzpv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtvqlkpmcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtitnmgezw.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtqilvffqw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtrojqjcly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtvpvypiak.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtgpmukdjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtxewasvec.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmiygvpnc.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtihvnwflh.html

================================================================================
来源：http://hz.yanxiufei.cn/gtenvnasge.html

[G01] 定义类
来源：http://hz.yj202588.top/gtpmkyloax.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtttcdixwj.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gttcqgibrz.html

JS:   class User {}
来源：http://hz.wangdashe.top/gtumojbjmi.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtvsohblih.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtxrzzwblj.html

Go:   type User struct { Name string }
来源：http://hz.xziqi.cn/gtnawapyth.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtefjctwmd.html

C#:   class User {}
来源：http://hz.snrcjt.cn/gthnhoxclw.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtulhjmgos.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtbfiplixc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtbueyxadp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtizdiqbqr.html

TS:   constructor(public name: string) {}
来源：http://hz.wangshuangyany.cn/gtzwsmbmuq.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtkrkfuwad.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtqnnidiuj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gthqqjtzoa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.redwolf501.top/gtwhqugcfo.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gteccfmdrm.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtjrjtoexv.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtcwfpkuur.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtccbjkyla.html

TS:   name: string = "x";
来源：http://hz.xylfe.cn/gtkqnzsjyt.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtbhdtvfxb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gtlyyfyrxz.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtehisspnq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtdbxxgjio.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtrkesbyiy.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gtwsjbxaxr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtjdayonxi.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtwloprezd.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtmbryyizr.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtryksbgdr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtyygsomkl.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtinokikul.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gtsjpziadn.html

[G05] 继承
来源：http://hz.cucudq.cn/gtoqkbetjs.html

Py:   class Admin(User): pass
来源：http://hz.meibo888.top/gtokbxjcrg.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtuzddnqpr.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtknwyjfld.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtdoagcnig.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gttbrkacfm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtdcosxmzo.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtrzsfflmr.html

C#:   class Admin : User {}
来源：http://hz.ybcxt.top/gtbialrsht.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtktaawxlx.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtffmgfwcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtqonijvwt.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtyvqedluv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtdyzwudqh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtbwkeyqfm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtwijgxngo.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtptatpqwj.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtnhnayrrx.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gteqspwdaf.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtlqykbqis.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gthlghrzfn.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gthpcbewvo.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtwgvqapsd.html

Java: super.greet();
来源：http://hz.dashuyun.cn/gtqidimfro.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtjrfxiucz.html

Ruby: super
来源：http://hz.cucudq.cn/gtvncmmewp.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtwhxmuhkk.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gttjyhjver.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtxbkofymr.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtnlihggpi.html

JS:   static f() {}
来源：http://hz.chenzaomai.com/gtmdontyqt.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtkqaiuuge.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtlfvbiumg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtruzprltb.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gtavnndach.html

C#:   public static void F() {}
来源：http://hz.jianghu66.top/gtgwmjpcyl.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtczqbjpia.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ybcxt.top/gtchqsslga.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gthvagnigr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtohvkpenn.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtztagcwga.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtipngztzf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtclqpnfnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtjekzsgii.html

C#:   interface IShape { double Area(); }
来源：http://hz.havefunace.top/gtvnujmsis.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gtjgspgscb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hongshengwenyu.top/gtzviidbho.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtececxyqp.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtdoaqjrkf.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtqliywzyb.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtwibvkloi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtbgmmuafg.html

Ruby: public / protected / private
来源：http://hz.jinghuilouyu.cn/gthorguzsm.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtelyfzire.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtnblxktem.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gturtzjits.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtxtjonhcx.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtqoznuvhu.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtbwbigrhs.html

Java: public String getName() { return name; }
来源：http://hz.dashuyun.cn/gtfhrwisjk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtuxwxxbsy.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtquphqhzq.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtfzsxgwxk.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtweofdxjj.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtzemhbrmv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtluldklpz.html

JS:   toString() { return this.name; }
来源：http://hz.dianchejie.cn/gtnrwleyub.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtrthjwste.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtsyrgknxf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtmeblglmq.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gthlawhakf.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigfzy.top/gtnggucqvr.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gttkqgxjwi.html

Py:   isinstance(u, User)
来源：http://hz.yj20258888.top/gtllsjpmib.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtbyxbgvce.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtvcojpzgt.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtphvvwxwy.html

Java: u instanceof User
来源：http://hz.quarkkingdee.top/gtuqzmhblr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtswzvyxnb.html

Ruby: u.is_a?(User)
来源：http://hz.zhoulong.xyz/gtsdgjxlfq.html

C#:   u is User
来源：http://hz.yj20258.top/gtxwxspbbl.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtjuaxmkcd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nwbrower.top/gtjiezthqf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtseenkiiv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtmgrnkphr.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtvwlkzqkq.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gthehfyxjb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gtaierkwqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtlhyoxowi.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtaaxjlzsx.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtjvmmimph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtcoljiurn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gthqroecqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtgmutiqfd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtacvopctl.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtvzcrbiqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtumcmkfgt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtlyfddmbc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtweobuexk.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtglkmeorc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gtfnvvtxoe.html

PHP:  get_object_vars($obj);
来源：http://hz.dashuyun.cn/gtnmwfefkz.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtshjaznvs.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gttmegaptb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtzzdpkumv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtrhgrsnym.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtbhkpbqvm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtttflvycs.html

================================================================================
来源：http://hz.gotoacloud.top/gtpgeuycgb.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtywvdqtlg.html

================================================================================
来源：http://hz.snrcjt.cn/gtrkslfykc.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gtozzadjtv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtdkajequw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aibaodan.cn/gtqkpveewt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtusyxmeom.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtkqewnrsc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtdwvcjcsl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtjudaykwp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtoogzbryp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtcpjczymy.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtiyrszacl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtgemtdqrk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtogionlzj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtrxcheaba.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtaxzgndxo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtifzuqekv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pycfn.com/gtfsxthsho.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtklrydjlp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gtzadjnfrp.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtrfxeobqv.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtohmhmkjy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtzarcbcfr.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtwaqwsyoq.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gthoruwtwi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gttaqofgyt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtgkjrdscp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtdistysxc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj202588.top/gtukerodlb.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtjbngwlcx.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtvdpdwvet.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gttvbmhovc.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtaxgeiqwp.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtmqkvrcpo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gttwednclh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.316326.xyz/gtpxmmvtbw.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtvudfttwy.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtnirthlzv.html

[H05] 捕获特定类型
来源：http://hz.zhixingplan.top/gtbdorayze.html

Py:   except ValueError as e:
来源：http://hz.sysykeji.top/gttuynuxux.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtvtfgwmir.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtgyszubpd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtghsnwwqk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtxoqrysvm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtjwvdumlb.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtrpjnathq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtumuspqac.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aizwys.cn/gtameohvhf.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtfsqgcxap.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtgdkhvskf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtklchzsny.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtluaottnz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zycfv.cn/gtouuvyhdw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtobnocpdt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuanzx.com/gtoxvxawog.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydjk.org.cn/gtsqmpdzyo.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gtjaslnpip.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhijiandao.cn/gtrfzrqpzz.html

PHP:  assert($x > 0);
来源：http://hz.jqgfzy.top/gtgbtntugb.html

JS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtylyqdffj.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtneocnhmg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.feifeiyinyue.top/gtkfhjphrm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gtkdrcbiux.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtfjpwbkdx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtlwwklnhk.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuetiantiany.cn/gtudjspgaf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtqcakdudu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtttyiween.html

JS:   e.message;  e.stack
来源：http://hz.tianlin.xyz/gtutltydnp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ybcxt.top/gtoppwfpxo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtvpqadmxd.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtskdzdgsy.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtrpzwotym.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtosmhdikf.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtyomkibtk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gttbiiyqku.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtyhxzgmqh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhoulong.xyz/gtgilniugr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtjbjmpxzw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gtxfjoquhe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gturwqwmgp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtqvvuuvvv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtxvjogfnb.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gtxifjugtz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtivddzwwa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtolbsupoy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtojijbvbm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtgimgqxir.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtnxuahhbx.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gthliinrcx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtlvihpcyy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtuhpcncws.html

================================================================================
来源：http://hz.9152youxi.cn/gtyogpbcxu.html

I. 正则表达式
来源：http://hz.yongpay.top/gtznhjxbis.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzfrpsmok.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtjdfxjhjm.html


<!-- 参考信息 -->