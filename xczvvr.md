代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtkzudwmeh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtlrlfqzps.html

Ruby: Dir.children("dir")
来源：http://hz.snrcjt.cn/gtdzhtgazi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gtvndnfivv.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtyewtlgss.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhongyouzk.top/gtvejmfgft.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtvdjfsvyo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtxdozfwuq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gthseqjiww.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtdgylqmqc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gteqkvlams.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gtdqpojmni.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtzbxkukio.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtkuvhwvhx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtzkmooamn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xziqi.cn/gtqjhjkldb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtxxphflcw.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtahgmvpvj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jianghu66.top/gtskpyqwrq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtktybuvuf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtclpvannw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtfvglztfs.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtotsypiaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtghutyyuq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenzaomai.com/gtgwbdjqre.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtsxmrvwum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtcqnhqhhc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gticoptbby.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shzxlz.cn/gtcvaiwzwl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtwzcyqcez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtlquuyssl.html

[F12] CSV 读写
来源：http://hz.jqgufenzy.top/gtblyliswb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtjesgtcez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnxiangtu.top/gtkznklkku.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtknqlvnrh.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtsmnsselx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtudzhvkry.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtbmkpqwmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuanzx.com/gturymlyfp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dashuyun.cn/gtxzlvdruk.html

================================================================================
来源：http://hz.tianlin.xyz/gtgkvqxtii.html

G. 面向对象
来源：http://hz.yanxiufei.cn/gtgilmnvxv.html

================================================================================
来源：http://hz.52xcode.cn/gtkouheefd.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtovepryxu.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtpvwwjdbj.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtjffirjek.html

JS:   class User {}
来源：http://hz.316326.xyz/gtjggjdftu.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gthhwkqmbs.html

Java: class User {}
来源：http://hz.hnqzz.top/gtulvprbng.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtkwjfhzne.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtzqrgstwz.html

C#:   class User {}
来源：http://hz.hysaishi.cn/gtfxzwrgym.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtcnpzwagf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtvdcigjtn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtmpaozfxn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtgzltrslp.html

TS:   constructor(public name: string) {}
来源：http://hz.quarkkingdee.top/gthttjwzbk.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gthspamqap.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtodijklot.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtvrtlqawq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtnvmajqid.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtcvrehslc.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtrewwpbug.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtavsffmtw.html

JS:   this.name = "x";
来源：http://hz.dianchejie.cn/gteyjnojei.html

TS:   name: string = "x";
来源：http://hz.chenzaomai.com/gtwpaqflon.html

Java: private String name;
来源：http://hz.xylfe.cn/gtxiiludlq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtxgxaoezt.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtihreggtq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.quarkkingdee.top/gtsyifjhgg.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtsyproisa.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gttubycjdt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtparniuqj.html

JS:   greet() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtqzyzijoe.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtxhigdwpu.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtszorwxud.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtfvyerddt.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtmiogntiz.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtfkryymdn.html

[G05] 继承
来源：http://hz.pycfn.com/gttosaihxx.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtzazzaknt.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtvuteoxgc.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtngqxapnu.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtsctqbclg.html

Java: class Admin extends User {}
来源：http://hz.ivvv.top/gtjuuexjoo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtlrwcchsf.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtibebfdlu.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtnnwkwjsk.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtzrhqfuas.html

Py:   def greet(self): return "admin"
来源：http://hz.vqdsnc.cn/gtatvuwcap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtzppxluan.html

JS:   greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtqhztwwlf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtiaifdtqe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtjrmckruf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtazuxmjmv.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtflgizmtl.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtwfpjdtxm.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtwcwbozbn.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtsgdsjqev.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtsagvipzs.html

JS:   super.greet();
来源：http://hz.tianlin.xyz/gthaabzeht.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtmzbxjzvj.html

Java: super.greet();
来源：http://hz.fengsongda.top/gtnglldlmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pycfn.com/gthqliwkgf.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtarlosuha.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtaosyezwe.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtpzttojpn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtseeclbmt.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtttypwafo.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtvbghikuu.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gteygeaerr.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtaxjsakrr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cqqwz.cn/gtnpxskkvx.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtehjzlkza.html

C#:   public static void F() {}
来源：http://hz.9152youxi.cn/gtzrifbesb.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtfeuhyrge.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sufxvd.cn/gtukmqaizj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gttjphqxqd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtpknycyat.html

TS:   interface Shape { area(): number; }
来源：http://hz.0kj1m.cn/gtznjcxolx.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtwxeywenx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhengqikj.top/gtshonqsdu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtkuxucyyl.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtphqaagge.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtdnvmbzzz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.quarkkingdee.top/gtbrpbzbtb.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtmqqbifua.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtqlopuyyr.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtuszlwmam.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtuwjqjdhb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtnpsxicti.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtzkrrwskf.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtpnihzuog.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtmjrtcotk.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtnfybsxsd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gthermhnju.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtogsdduks.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtoomsjpwq.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtlbyizjic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtojbdafqd.html

Ruby: attr_accessor :name
来源：http://hz.meibo888.top/gtmmvpmzjx.html

C#:   public string Name { get; set; }
来源：http://hz.mhx1999.top/gtutyfkvfz.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtozlrrajt.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gtamknfqrt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtwhcfdoba.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtfpreejtn.html

TS:   toString(): string { return this.name; }
来源：http://hz.xziqi.cn/gttwwqbrjz.html

Java: @Override public String toString() { return name; }
来源：http://hz.gaohongyu789.top/gtezepcmpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.52xcode.cn/gtvpkhgzks.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtqmefdzus.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtwdvmania.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtkmmicblu.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtjfknakgx.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtqrizfjhl.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtfsgwgetp.html

TS:   u instanceof User
来源：http://hz.gotoacloud.top/gthhaaqfsr.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtbpwzsdcy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtfgaqrifl.html

Ruby: u.is_a?(User)
来源：http://hz.nanxuanxn.top/gtvzhlrdug.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtjlgmjfpi.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gtzlltoich.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtbtbsegxx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtgaptnyeg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jianghu66.top/gtzfygxwzy.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gtlryikdeu.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtnaxneaim.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtwoghfexx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtoncezamf.html

C#:   record User(string Name, int Age);
来源：http://hz.meibo888.top/gtcyuvthaf.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtcfpwamku.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtqomdqjjf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gthbgnmlfj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtszngffts.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtzbqehvmg.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gttlnnmagx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgufenzy.top/gtpqyeqgxj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtkbmreplv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtdczeunav.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtchqavmsh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtruxkvdzm.html

PHP:  get_object_vars($obj);
来源：http://hz.iojbl.cn/gtzilbypvg.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtefekmylu.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtthzgxqaf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtdxvmpnld.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtvbkunwjq.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtppzmtekl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtgoopkvqx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthhnibuli.html

H. 异常与错误处理
来源：http://hz.cdnleiting.top/gtdypjdzea.html

================================================================================
来源：http://hz.cheryme.top/gttewwgyoj.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtlxignwvd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtohydotoe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gttlnqbebh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtlrlcepxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtzzkpeoxt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtyevejjzd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydjk.org.cn/gtnnrdkrkn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtjtydowsf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gttghervxr.html

[H02] finally / ensure 收尾
来源：http://hz.vqdsnc.cn/gtffglpaqi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtunchdzsq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gttgukmgls.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtktrvigbe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gthxmdhpth.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtawxrgqvf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtiqjufmlm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtfcrkhjub.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtpjblqdvy.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtklvldadu.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtsjnakari.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtmcvyugun.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtldjtwqyk.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtspknkrlg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtpopznkka.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtuuliydcy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtdkivwdsw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtlmweqzqj.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gthpcsxyob.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtahyhvzxw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtgltuhbxj.html

JS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtfoytvoml.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtvsbnoozi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtwfbamwdg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtatmfqvtb.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtxiydjbes.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtezaebfus.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtofisfotp.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gteadvzatw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtrxydfiaf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtqwgbopgm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtqquwnvjm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtdpdzhfhx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gtnlcewcco.html

Ruby: rescue ArgumentError => e
来源：http://hz.ppjwa.cn/gttslzsskc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtwlkkzkrh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtdodrywaq.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtckbttcwf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tanke756.top/gtfesljrhy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtnlzcbztl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtwisxepwj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xylfe.cn/gtqcittltd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtkqjpacsp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtkmrmfrct.html

C#:   obj?.A?.B ?? default
来源：http://hz.vqdsnc.cn/gtxildquxo.html

[H07] 断言
来源：http://hz.wangdashe.top/gtxxjuyaro.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangshuangyany.cn/gtqqqcjbxb.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gtmfwazcdo.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtllbzbarv.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtjyokhtmk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gtqihuudwy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gttcsbjvkf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydzc1.top/gtxcbbbvdu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtuybfnmra.html

[H08] 获取错误信息与堆栈
来源：http://hz.redwolf501.top/gteogbkzec.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.feifeiyinyue.top/gteoxhnosm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtaocrdvyo.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gthkbdeqed.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nwbrower.top/gttpqzzllc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtyywzmeqv.html

Go:   err.Error()
来源：http://hz.aizwys.cn/gtuuhvbftd.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtvvbsyzmw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gtrjfqacqd.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtcjtxjjir.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtmyaaxlyi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtrhkywvjw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtzxwwqswj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtvtsjxnss.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtqmvzbsxd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtsyxrfehq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtiqchryca.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtzejojwrz.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtehoruave.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtrccckflb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtjvtcxpqk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtksxoxwcv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtgggxfztm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gtodesrfka.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtezidrcez.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtvvsxxxfd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.iojbl.cn/gtkruqabzk.html

================================================================================
来源：http://hz.ydzc1.top/gttwcnfkiu.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtivcmcpjh.html

================================================================================
来源：http://hz.ppjwa.cn/gtzcocxuls.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtodqgvwju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gttpishmub.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yongpay.top/gtomlkeecs.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtyurxrcli.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtmmcvhpak.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtikkyqlwv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtmzhlgtdf.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gtneljlfqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtlzojvfij.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtdbiccapr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtlbhlgxbo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtiomexglv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guowangkeji.top/gtioxsgklg.html

TS:   s.match(/\d+/g)
来源：http://hz.andypj.xyz/gtoppnbhif.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gttvcdqbrd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtlszrpfgd.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtrmwotqfv.html


<!-- 参考信息 -->