代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhengqikj.top/gtmkquerpa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtvwcdxxhz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtpmqjwpmy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtaomyyiyl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.vqdsnc.cn/gtqoohzfus.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtqvziujru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtxmnajvgm.html

[F12] CSV 读写
来源：http://hz.jinghuilouyu.cn/gtwlwdvkuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gtalakvuiw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gttdsutmwa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daxiang520.top/gtqozzwyqa.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtenxhhjzg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jlsjyb.cn/gtpllvjene.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtmzoddyok.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtvmzwcjai.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gtutksalhi.html

================================================================================
来源：http://hz.hfpthk.cn/gtissxmfsq.html

G. 面向对象
来源：http://hz.cashguo.top/gtraaawgro.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdvajcphj.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtvgfrtgqx.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtsubpsrdw.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtnkbjprgc.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gtagdytyga.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtanhuwhjv.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtzypycxoa.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtjbcpjake.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtmglrndxy.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gteofqfput.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtvctckrft.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtbcutzppn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.haohaochexian.top/gtmxjohyfc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtgoivtecx.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtcvieorlt.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtiomgkvnx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtaqxhjpgm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtutwhvdct.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtisilsawm.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtpgkdvouk.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtmppiezdr.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtyxiwynad.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtojlqaipn.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtopinalfl.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtjdffxavk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtytsoxrrq.html

Ruby: @name = "x"
来源：http://hz.mhx1999.top/gtnfxxzdzw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtwmrovvcj.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtppseniot.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gtvljjukhu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gttvosnwlt.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtcqbnwvlj.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gthtmskbxi.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtsotddacd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtyseqazjm.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtpfzkdksp.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtgtvtvkdw.html

[G05] 继承
来源：http://hz.yueranfly.top/gtrxjocfgm.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtumuxygrk.html

PHP:  class Admin extends User {}
来源：http://hz.ivvv.top/gtsvtsdjsq.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtuxgozugj.html

TS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtippyiyyf.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtrdmxjcby.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtkurhbjsh.html

Ruby: class Admin < User; end
来源：http://hz.quarkkingdee.top/gtvpsvkdzq.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtsxwgjjof.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtbssghjdw.html

Py:   def greet(self): return "admin"
来源：http://hz.xylfe.cn/gtleloibmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtadwnhiyp.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gthgrgavzh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtnlecxtst.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtxfrtilnn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtbjqlpape.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtehkbckll.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigfzy.top/gthbvqmexe.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtsnfljnui.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtwwyxlhts.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtntthrpwg.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtxqoalpxj.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtzblftmaz.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtmxmhlfbk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtqmdlpvjx.html

Ruby: super
来源：http://hz.svipenyu.cn/gtycqjvtuk.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtuhcuuglr.html

[G08] 静态方法与属性
来源：http://hz.tanke756.top/gtiutiniee.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtanfltiae.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gttdjsgubz.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtgvterkwk.html

TS:   static f(): void {}
来源：http://hz.ydzc1.top/gtcqibtouh.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtlwttvsnp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pengpengdd.cyou/gtbubczmfg.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtnjabtodc.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtegjjomlv.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtjjapdxmn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtxzbfbohq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtygeorhhh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtjhsgtfan.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtqpxyiohe.html

Java: interface Shape { double area(); }
来源：http://hz.cdnleiting.top/gtvhvnlytq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gtfpswhjeu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtkdveootg.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtbvihqlmb.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtsmnkiffr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtzhtmsete.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtstcuztej.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtzstbrgfo.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtvegnpeky.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtneodbjwv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cashguo.top/gtuezqdfph.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gtthydsxew.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtkxeonyej.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtokaphujn.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtdqwkhabx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtspcnycfk.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtvwdzjpwh.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtjxxywigo.html

Java: public String getName() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtrxzqsrfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtodhsvlpk.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtggwmlrxg.html

C#:   public string Name { get; set; }
来源：http://hz.guannengcc.top/gthqjkfdtj.html

[G12] 对象转字符串
来源：http://hz.hnxiangtu.top/gtrvcyuppn.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gtjztidice.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtzncgthet.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtfnyerxdy.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtnbrkiulm.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtsmbbwrml.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sweek.top/gtocfkrbxj.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtjewgzoov.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgufenzy.top/gtvuhdfjpx.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtsnqqoakz.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtlucgmajn.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtogjmtgvd.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtrlnxoacw.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtegghpdwu.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtfygmfioe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtzrhcwryx.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtzwletsmv.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtgxmxydlk.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtjrftydhb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtwuovxxnp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtywgslqqj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtcexjibnu.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtdygvgjej.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtwvxejill.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtvtfegndc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cdnleiting.top/gtfouvyrjr.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gteimlvzes.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtmawiefmu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtozpqsbgw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtoytqrdsa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gthzsjkokd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtfeztcvgg.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtqtdixxwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtnjtfoqvg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtscjaswpb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gttzdhrriw.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtpvpuupks.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtpdrzggma.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtnsaumebe.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtsnwiinep.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtdeibvyaj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtkdjdhepk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtzpfptxff.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtskpalmvb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtjyaanpid.html

================================================================================
来源：http://hz.yj20258.top/gthdadmrig.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtiktutbjf.html

================================================================================
来源：http://hz.yonumen.top/gtyshewhzq.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gteoukcekt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtvcodtgfa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtntzajtjn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtcnakltgh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtcczzonhi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gttluszjkx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtijhduloe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gteuvdlxuc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtqgkubjmi.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtevwaqygj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.haohaochexian.top/gtlgivjfzi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtxekdwxmk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtvwjgobmw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtafwiktms.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gteanawpuy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtvzapjlmj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtrbyjcien.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtlijxsnyk.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gtpiybubfp.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtvncqoslq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtumfknmdv.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtiuopaqar.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtonbfkxvw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtgelxvpug.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xinyue.icu/gtqrevsyjw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtlazgitcf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtehyaqfmp.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gthxkwymcj.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtbdwqinuj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258888.top/gtcvrsmlnp.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtsurrnmjo.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtppdgdmfv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtzanvapzx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtyfvluoqo.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gtwblusgov.html

C#:   class MyException : Exception {}
来源：http://hz.nwbrower.top/gtogsprijh.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtdgtizuvi.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gtprqrqkab.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtqksjfgtg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtiohjgmin.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtmryrzblg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtzvqitcwf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtjibhurve.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtwitszlvb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtxazydaec.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangkeji.top/gtetugwzbb.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtulrnbpta.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtmnbzpozz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtzawlvpfh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtseyipmqk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtlsbdinrh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gtnvikkiem.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gtxavwoyvr.html

C#:   obj?.A?.B ?? default
来源：http://hz.ivvv.top/gtodikeinh.html

[H07] 断言
来源：http://hz.fzhhl.top/gtsolfewpp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtqibrjcka.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtjtszxolo.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtctpjlrjr.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gttkntdhcx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigfzy.top/gtidqhwuor.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtwevyqwpt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtfxtsrkem.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtxokhmrfk.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtxctwuxen.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtgynsdvbo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtwbexqbnf.html

JS:   e.message;  e.stack
来源：http://hz.tanke756.top/gtkrjlaxsu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangshuangyany.cn/gtnynoatkt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtnhqiysdv.html

Go:   err.Error()
来源：http://hz.snrcjt.cn/gtyouiaesb.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gtfqntopbm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtqefikklh.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtlpofwdjd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtwveqlqlq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnxiangtu.top/gtzatpmmhh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtzgsoatue.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtxdkeynpy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtsjsahsxb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtmjkmhgxk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gteopoajos.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtfbqrxhsl.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtvpydpyup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtzcmlhtml.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtpgarhxca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtoiaqobcq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtqxfmlpgg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gtjqhveveb.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtcspkttdq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtlwjldaqz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gtctoyiags.html

================================================================================
来源：http://hz.zhijiandao.cn/gtchfexnza.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gthylddaaq.html

================================================================================
来源：http://hz.gogol.net.cn/gtsxizfbai.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtfmlkmvto.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtcmxmybgz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtfheignpr.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtjjtwswet.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtmyciadmt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gttrzltdis.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtlnbenouc.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtpjzvtzwc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtrhurpmbi.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtjlandjij.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ppjwa.cn/gtfvkvvcxz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtsrdwvhpm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtsfuuwoug.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtoaluilzo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtlmbkzdrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gtnqjjoglk.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtsccbmmob.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtdofeqyah.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtgjgerfyc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtpgrgxvsx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtqodsster.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtgeptwkmj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gttrqbbnvq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtbtezzeia.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gtrfpegjux.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtzatxnbye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtfsfskqux.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtdklgdgvg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtkhslikam.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtopzhvqeg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gthbnqzqxe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtizmsmdup.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtqajxefxx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtrmrldjzo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.meibo888.top/gtwuxmjcte.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtwuoaiupq.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtmkezlamv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtyzvxguce.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtsmqazbpz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtqllouien.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtytaptntd.html


<!-- 参考信息 -->