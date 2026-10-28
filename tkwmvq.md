代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtgajhytzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhaomingkeji.xyz/gtkbjgexmd.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtuzoexjqm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gthxbxgmlh.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtoxlnckbh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtsjmcmxmp.html

PHP:  filesize("a.txt");
来源：http://hz.316326.xyz/gtibznkbvm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtwdxljwnh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtlnzgdauk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtvrjohnva.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtlnptbcyq.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtcslnxmmh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtprkdhalu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cdnleiting.top/gtxesiohlc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtvvllymcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtslilnmol.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gthvlmcdnr.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtdkizemoo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtlsbwurvn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gthvotaixr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtxxjbixqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtuqiqyhfw.html

[F11] 复制与移动文件
来源：http://hz.tian-w.cn/gtwnhrxcuy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtoczbebvf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtxvvzmzuq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtqsabarve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtolypcaml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtflyjztjw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtckjychgu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtzplpirtq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gthaekqgeo.html

[F12] CSV 读写
来源：http://hz.xylfe.cn/gtvnffviog.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtvgzeqesm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhiwuduotai.top/gtnzciswfz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daria6918.cn/gtzwotydbv.html

TS:   // 同上
来源：http://hz.feifeiyinyue.top/gtzkgposnk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtfvzdmqbf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtdccrbgkz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtauhnhmkh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtfqcelcqf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdbzssdla.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtrecowhbd.html

================================================================================
来源：http://hz.nanxinkj.top/gtowlneoor.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtlmsxxyzx.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gtspoqejhm.html

PHP:  class User {}
来源：http://hz.xylfe.cn/gtdrssjagl.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gthacjkrix.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtystvtmgd.html

Java: class User {}
来源：http://hz.nwbrower.top/gtwwptsddy.html

Go:   type User struct { Name string }
来源：http://hz.cucudq.cn/gtyylcsxfk.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtitnhfqut.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gttkpuqbcf.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtctwtnulj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtzgncevis.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtyhjlqlvm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtlipkrfwb.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtlkizdzmn.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtzwcilntq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtgrnfwqcs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangshuangyany.cn/gtnvkvhnih.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtapboyjsq.html

[G03] 实例属性
来源：http://hz.hongshengwenyu.top/gtzstuimiu.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtuchrbyck.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gthwvpcbrc.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gteyzwqacm.html

TS:   name: string = "x";
来源：http://hz.svipenyu.cn/gtxvdkalaw.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtebnbneri.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtkbshuyih.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtefwymypx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtsjbkazqg.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gtelllltcx.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gttzmgolok.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fengsongda.top/gthclvmvkq.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gtgmgcoaty.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtjjulptrs.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtcicfgpdz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtdoczcroc.html

Ruby: def greet; @name; end
来源：http://hz.jyoumei.cn/gtkhchnykd.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtsccyxxkd.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtuktvxvjs.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtmjhqiodv.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtooruboxc.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtmovmtnyx.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtyhkioxkb.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtveiovfqv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtzktmqpje.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtqbemtieo.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtgwcglyjf.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gthvxchbtk.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtntouseoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtbyxamcav.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtvkmnsqpz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtpgbejmqc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtaaombvzo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtqqukkbpj.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtlkskvwef.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtfgipmymr.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gtgufrtqsh.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtgctknkkw.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtyxsfafxb.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtzdzlvoag.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtaikdvyir.html

Java: super.greet();
来源：http://hz.xuanzx.com/gtjixjrkdi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtxmmttyxl.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtaamedyef.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtgeopvxqz.html

[G08] 静态方法与属性
来源：http://hz.dianchejie.cn/gtxvppmfvq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtmcjuiiwq.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtijmnrjmb.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtbmzkqpmj.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtuqapwxbo.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtmqozkoit.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtpumegkyn.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtlradpqkf.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtpcxbefaj.html

[G09] 接口 / 抽象类
来源：http://hz.nanxuanxn.top/gthpcovxdd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gternhixcr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuxming.cn/gtsdpuaukt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtzmnusvnv.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtocpzrqux.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gteybevclh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtwttezgpd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtwwyiwutq.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtgocfseyi.html

[G10] 访问控制
来源：http://hz.tianlin.xyz/gtgsbtciax.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtdejovdne.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtmebdgttu.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtsscpyefp.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtysugayiu.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtiajwuyqy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinghuilouyu.cn/gtsyspyxxu.html

Ruby: public / protected / private
来源：http://hz.daxiang520.top/gtfrywlqsp.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtmuxatitu.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtpttygfse.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtsrnwjkiv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtgeawqqno.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtuabczizg.html

TS:   get name(): string { return this._name; }
来源：http://hz.shangyingyoupin.top/gttidscxqz.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtnqwgscta.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtbrrtfwzw.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtdxgixgwv.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangtech.top/gttmxvivct.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtunmfmqhl.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtwqgnlgqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtfortcdud.html

JS:   toString() { return this.name; }
来源：http://hz.jqgfzy.top/gtojsrhsyb.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtkllvrfep.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtbwywwiva.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtnlfgczgz.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtxilgfvlt.html

C#:   public override string ToString() => Name;
来源：http://hz.yvedp.cn/gtttgxswvk.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtnhcyhqaj.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtnupddwam.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtaothkrlm.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtgkgaqbld.html

TS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtanrjxfxp.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtwefgtlhx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fzhhl.top/gtxnevavma.html

Ruby: u.is_a?(User)
来源：http://hz.ppjwa.cn/gtftodlbjm.html

C#:   u is User
来源：http://hz.yongpay.top/gtaiuwwfsd.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gtudgckgpe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtptdsugxa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtefoucafn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtmxzejbyv.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuetiantiany.cn/gtplucxyjw.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtnmtheizh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtddnqllfw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtxekfphls.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgufenzy.top/gthjlzzrsm.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtogufrqkv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtsadprpse.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtklimionu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gthshizely.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtiylizpmf.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtxguifdkf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtmrudnqmy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtxpauaxua.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtugncpunz.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtxwzvuxeu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtevosmlwt.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtpquvgbwu.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gttbuxdemu.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtjrevvpgt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zdqjudy.top/gtnqdgjgxp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtximiicym.html

Ruby: obj.instance_variables
来源：http://hz.ydzc1.top/gtmshvuqda.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cashguo.top/gtjxilvdyn.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjallaobp.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtujhebrjd.html

================================================================================
来源：http://hz.birdmap.top/gtsnaorrlp.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gtorcqujrk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.meibo888.top/gttwszxayr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtkjjockff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtudeovqgp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtlvzesyxs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtwpmshunr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtjsanvujo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigufen.top/gtysccqdyg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtupcifnkb.html

[H02] finally / ensure 收尾
来源：http://hz.hfpthk.cn/gtpaedpdwz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtdihmxlko.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtxqforxsg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtyidnqvft.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gthumbmxwy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtnhjuwfms.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gtcrmlkrxj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pycfn.com/gtufeqcmvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtubzrgxmj.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtwotzijyd.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258888.top/gtjmsuxggb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtptequniw.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtkikcpuoo.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtxqfvugve.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtvyqazlia.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtdcgioenp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtizkagpws.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtlrimhqbz.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gtxtsgrkaq.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtewnqzsou.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtbbisjpxy.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtsuogfrck.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtjgqtiode.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtbpvrxkpx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gtnhevzjxs.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtyawkymsh.html

C#:   class MyException : Exception {}
来源：http://hz.zhixingplan.top/gtidbcbsqf.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtcmlcvxfv.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtwqiewbtb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtytfewemk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtjveiwdig.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtjabjokpk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gttzydbpzs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtvvsufxjp.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gtkgiocyzc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtipiyfmbz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtdnlvvjrt.html

Py:   value = d.get("k") or default
来源：http://hz.tianlin.xyz/gtmhtlghhb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gtzmixxvcz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtgabgferi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtvrtydaee.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtteqhvyac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gtabpedvqd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtlvsamkyu.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtiblfycvq.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtlruywdem.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhixingplan.top/gtbocnehcb.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtsrweyyrs.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtyhmedfyg.html

TS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtaxlzxkud.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtgifxiiem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dianchejie.cn/gtkxuudzbt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtncovuboi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtkalkbiyb.html

[H08] 获取错误信息与堆栈
来源：http://hz.zdqjudy.top/gtnojfgvdv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtrdhejwbz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtrsjbqhhg.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtbvwkofcr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtbjrycvod.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gogol.net.cn/gtvddjokyy.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtodfztouw.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtgjtqlafq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtwiqtvuho.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtsnrygyet.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtrlkspooa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtatpfxklj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gthxpjlphz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtocaxmwcw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daria6918.cn/gtkonnmhss.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtghnemfhs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtwjktjktx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sufxvd.cn/gtpvoplwin.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gthnsephid.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtygjltaxi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtozagecuc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtohaeoxea.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtzoptkilv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtkcxztrmx.html

Go:   defer f.Close()
来源：http://hz.ydzc1.top/gtslftwwuv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtwajngpxn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtgvrxkrra.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtyeavlegl.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtqsmtcksj.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjffwzewe.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtqhzgqrdh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtlkafzlqx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gthrdtaxfl.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtfmprwvut.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gttoikiozu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtmowupent.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gtczlxhsek.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtavlstwfw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuanzx.com/gtcxanxbyi.html

[I02] 提取所有匹配
来源：http://hz.hnxiangtu.top/gtahhrlvll.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtgiljjxsi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtrqqasbvo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sysykeji.top/gturygjobm.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtxhagysmw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtvgrusxdl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtgectwzth.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtgrslzauu.html


<!-- 参考信息 -->