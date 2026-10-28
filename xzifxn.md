代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtykpxlrwp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gteozhkywr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtrgaxoguo.html

[F12] CSV 读写
来源：http://hz.guowangkeji.top/gtoayainrd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guowangkeji.top/gtmrpqbzva.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gtdskucwkl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gtvmhucnnx.html

TS:   // 同上
来源：http://hz.cheryme.top/gtqilsdnva.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtcieweaqa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtzmnmgnrr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.andypj.xyz/gtogmnvqeq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtrrykfbtj.html

================================================================================
来源：http://hz.shzxlz.cn/gtywwtxnya.html

G. 面向对象
来源：http://hz.svipenyu.cn/gttssshcqo.html

================================================================================
来源：http://hz.fengsongda.top/gtypbusvvg.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtsmmgumwo.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtowpylbiq.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtndrikhnv.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtfzwvxmem.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtrgtbxgaj.html

Java: class User {}
来源：http://hz.iojbl.cn/gtsipcjsre.html

Go:   type User struct { Name string }
来源：http://hz.gaohongyu789.top/gtphptshgo.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtrajtsrdn.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtukarizkx.html

[G02] 构造函数
来源：http://hz.sweek.top/gtsdcwzcog.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtqzvgwiih.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtpaxojxsx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gttkwhmdmh.html

TS:   constructor(public name: string) {}
来源：http://hz.wangshuangyany.cn/gtzntesppx.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtvvcttghe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtelrjtvzk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtibylwkkj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtvswfuvyx.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtnvhfpgar.html

Py:   self.name = "x"
来源：http://hz.ybcxt.top/gtvhhtmahm.html

PHP:  public string $name = "x";
来源：http://hz.snrcjt.cn/gtlfkencny.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtoisshfqx.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtbekxhftf.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtgdcjajqs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtbkqwfuke.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtssvrlzml.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenzaomai.com/gtubbtyrgn.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtxkiekpzl.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtxefyvkgv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtnlgnkdzr.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtqtfaugre.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtzbjkhgye.html

Java: String greet() { return name; }
来源：http://hz.jyoumei.cn/gtbhjpnxbk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtscektstq.html

Ruby: def greet; @name; end
来源：http://hz.daxiang520.top/gttvxahjyj.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtxofkmvxf.html

[G05] 继承
来源：http://hz.yj20258888.top/gtrhqkpnvw.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtwzydpetz.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtdtiwsimw.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtfhbetthb.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtwjuzbgzd.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtfbyzmlqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtiwmzowtw.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtpvxzvqka.html

C#:   class Admin : User {}
来源：http://hz.wangshuangyany.cn/gtqosjbmzn.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gthtropgoc.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtkksmaaoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gttfuebdcg.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtkmkntpqj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtcfttdafg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtdunydihz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtuknaicrb.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtkldubxsg.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtvxybvvgw.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtcypnicsu.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtjephdmmk.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtexinurjy.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtgxlasaqg.html

TS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtdwjonxxk.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtqqzcwvap.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtjslmecsx.html

Ruby: super
来源：http://hz.cheryme.top/gtowhxveoj.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtynbuvvoe.html

[G08] 静态方法与属性
来源：http://hz.pycfn.com/gtkavpvsmz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtpyqmhhvf.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtrbwclbzg.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtfdndrkxv.html

TS:   static f(): void {}
来源：http://hz.xziqi.cn/gtgiguccdb.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gtchdhndds.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtvasxkivx.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtzvuiqyti.html

C#:   public static void F() {}
来源：http://hz.guowangkeji.top/gtyqyeuueh.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtomibvqzt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtfveshwuq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtaafvocsk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtlttgvqeh.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gttanrdtrq.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gthminqvai.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtyoaugmug.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtyiygseoc.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtnnyuinnn.html

[G10] 访问控制
来源：http://hz.cqqwz.cn/gtcbtfnjek.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtcsksjbek.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtcguikmde.html

JS:   #private 字段；其余公开
来源：http://hz.haohaochexian.top/gtrusfrsnh.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtxzhcfwyn.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtcmoqhskc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtnooobovr.html

Ruby: public / protected / private
来源：http://hz.hongshengwenyu.top/gtzrnkyocb.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtvnmbisep.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtwbzpppzs.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtzznwpydr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtcaejndhp.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtdgkqjsht.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtutrvqtcu.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtvqhojqdo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtrmjvnzfv.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtwkhpzctf.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtqgilxoff.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtpwzyabet.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtumfpmsmg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtlwvvkool.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gttvuoehyi.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtkksmzdgp.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtfupjdzxt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.52xcode.cn/gtvshsmkai.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtbfvxdkyo.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtnoijetjt.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtdtnzdxbh.html

Py:   isinstance(u, User)
来源：http://hz.yanxiufei.cn/gtfpictvec.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gtxllnonua.html

JS:   u instanceof User
来源：http://hz.guowangkeji.top/gtpvknkrns.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtcrfjdljf.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtopeyifuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtjuhzhlax.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigufen.top/gtqtlhjayx.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtckfweqan.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtfgzdhlwr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtdrvihnph.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtohyhxulw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtqjipxqbx.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtinpshlui.html

Java: record User(String name, int age) {}
来源：http://hz.cqqwz.cn/gtdghwgfzn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.havefunace.top/gtqbbbschk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtcqqwgaip.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtepekitcb.html

[G15] 枚举
来源：http://hz.sweek.top/gtgevihvur.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtnbuowkqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtgwayfgpe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guannengcc.top/gtdxhjwjms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtnmyqlatf.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtygsedugd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtvnqicoie.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtexbwmmng.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtvvezaekm.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtelcnpmay.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtacvzleju.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gthmhmxarg.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtaawxiaas.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtjnkuordl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtehsqpock.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtkikqqlgq.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtloisczdv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtugvjxpwe.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtedodcdgy.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtorhnkoch.html

================================================================================
来源：http://hz.pycfn.com/gtuwhbgxfk.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gthgmosnif.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtmfcveide.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhongyouzk.top/gthpqsznmd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtygqamnbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gthmdtwytz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gtnukjrybk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtxvlqyugg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtfiqhxuqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtfmerwfih.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtokftxsxm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtbsmfsdao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtfazhjrnt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtbytgrhvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtspemteoa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtkahrjiwf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtnumoqozg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtyatnqrhf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtaghufmvr.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtvrhssnxt.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtonjefhoa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtlmtenddl.html

JS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtgegrtaba.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtzhcseick.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtlelqghho.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtriqfrous.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtrvxbbqdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtrhxmovmk.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gtzcloymkb.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gtsjutvieh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtcosjiblp.html

JS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtmzxlcizw.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtakwxopjd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtnvmqtlfe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gttfrrsnsp.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtwyqgyjjo.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtnhgtnumv.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtcxwuktye.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtbkacgrmy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtdwlpxjfr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtgvmmivpx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtybtpdfpq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtqsjetgmy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gthfyiyrfz.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtnayhzsls.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtdozsgjdu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtmpovdvvu.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtovtlwowm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtykgavbls.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtltvsdrgk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gteciihose.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gttxdflglj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtcbnqlzyt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtrmltcops.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtltfaaxzx.html

[H07] 断言
来源：http://hz.cucudq.cn/gtagnnnkyi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtkpmabisp.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtyslzpbqt.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gthgcxhari.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtjssunfyn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtdtkacypq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtxqayjrww.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtrkvqzxqv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daria6918.cn/gtpkilqshl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtdibqnlxt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gticoydbpf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtljsckjzd.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtsueiefhj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.meibo888.top/gtmqwwrccr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtficpxiib.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gttpswcgsa.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtkozyhihk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtxteeravk.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtemilcqjg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.iojbl.cn/gtpmplvstz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtynnvqqgl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtfgfihdsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gttqoljsrf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtqufscxzg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtcdlanrbd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtbpdgjyup.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtbvdypihm.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtwrriytrk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtfoyebqgb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtxcysdsvl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtdndhlfok.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtyqdminga.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtmmhzqqih.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtfqehsjjj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtiirosydl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtgedwnpnn.html

================================================================================
来源：http://hz.ybcxt.top/gtwiuhnvfh.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtdeywdvwg.html

================================================================================
来源：http://hz.smart0.xyz/gtofyrqota.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtiidyqytg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtgovuxjua.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtylezkmaf.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtvxrjftzn.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtjghwqbgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtszgtoqxe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtexmqegzp.html

Ruby: s.match?(/\d+/)
来源：http://hz.cheryme.top/gtodwimoww.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtucovrvge.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gteuzpnafn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gtwvnbjlfg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtdxizkjck.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtyryqiexe.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtlhljisbf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtovshfuiy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtqwyqxkjx.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtheloeafy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtzhlkvrvt.html

[I03] 提取捕获分组
来源：http://hz.jianghu66.top/gtqabwfpge.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtglnyeunt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gthqymeico.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtqekykxeo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fengsongda.top/gtvkatldtf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtnlwjjire.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtlineeaci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yanxiufei.cn/gtvvckuwsf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258.top/gtukqsecnp.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gtwxddfgdi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtbbhgglyi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtnmbbtxld.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtnfpstcpa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtcgdltztl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtbcrgqvbu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtyrejgaly.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtfbftzldv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtiowceyvo.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtrckffggv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gttjohwmwt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtokztsbjj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtfqetjgsg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtukxcvbdy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtkplojmty.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigfzy.top/gtmneiztoy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtqxgjlred.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtfyxemrpu.html


<!-- 参考信息 -->