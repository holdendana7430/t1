代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtuabriblq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtsixqyemk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtlukugzwk.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtmyztlwnj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtlytmfdzj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtchqqgndb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtpftwttns.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtwgxhzxyx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtoxsyxixs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtdlvjyaqb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtytwmlwjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtsnwnecmd.html

================================================================================
来源：http://hz.mhx1999.top/gtsrfwqwcd.html

G. 面向对象
来源：http://hz.guannengcc.top/gtkhxoypyq.html

================================================================================
来源：http://hz.zdqjudy.top/gtoygfvzys.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtercvtiew.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtsektflpl.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtysrklssi.html

JS:   class User {}
来源：http://hz.dashuyun.cn/gtzhcdzlgz.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtrqdazriy.html

Java: class User {}
来源：http://hz.guannengcc.top/gtcobwaspc.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtosmqvccy.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtrefgtwns.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtbarbzjty.html

[G02] 构造函数
来源：http://hz.cqqwz.cn/gtuhkttcgz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtwvyvvldp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhiwuduotai.top/gtffixwyfa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtgogbdjxq.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtmlqenjqs.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtpetkaupj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gturtgnwle.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtsougrmcr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtkssfwwbx.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtposzybgg.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtesevgabt.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gthqclikez.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gtnqghoupn.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtxvkrsqab.html

Java: private String name;
来源：http://hz.9152youxi.cn/gthifburzm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtucmwzcsa.html

Ruby: @name = "x"
来源：http://hz.jinqigufen.top/gtdedhkvlu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gaohongyu789.top/gtxbnmdrcb.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gtojeellgq.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtlyrcqirj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtzqeohomn.html

JS:   greet() { return this.name; }
来源：http://hz.nwbrower.top/gtvtcridhf.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtwielirjs.html

Java: String greet() { return name; }
来源：http://hz.cdnleiting.top/gtivfqvkmr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtzbvpijky.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtdkduhtdl.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtzvcerszn.html

[G05] 继承
来源：http://hz.yvedp.cn/gtoopxzork.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtxoopkwpd.html

PHP:  class Admin extends User {}
来源：http://hz.cdnleiting.top/gtrztaknjd.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtyucunqzb.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtxnjldpds.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtpybcwubu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtyhiuyver.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtnzolswfe.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtfrsjvpsf.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtyhvanwhk.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtgwnaqcma.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtunvjbyid.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gthwxxhchd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtlhstibit.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtdeflbxdi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtasycqgim.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtdlwncwom.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtltbelhil.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtlurwqdvh.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtexrnusao.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtvspzsclb.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtzcnvhvoh.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtgekmxopc.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gttqesgseu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtlsiqawmm.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtggdhxgzp.html

C#:   base.Greet();
来源：http://hz.cucudq.cn/gtnqjjzdou.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtbrrdxsba.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtnnsjejkv.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gteayfdhde.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtjgquiqcu.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtlezhsoby.html

Java: static void f() {}
来源：http://hz.gogol.net.cn/gtkqbeqfbw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtrpfuplbc.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtxgwyijqu.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gttbblpcse.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gtzdhmvclo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gaohongyu789.top/gtxgzuvxtx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenlongwang.top/gtfnftkuom.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtmoxiqakh.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gttncpopwz.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtwzdexfsc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtsaeerfbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtotahmqfr.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtxowwjaaz.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtsrgaxzse.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gttkggzrms.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtaqvrfggq.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtkapkwggv.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtidjkiual.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtoxbuyfqe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtsyoadhjz.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtknctzoso.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gthawqhtja.html

[G11] getter / setter
来源：http://hz.tianlin.xyz/gtmuciulpi.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtnsqenjix.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtdmumxynb.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtvyysikip.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtpojmupqa.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtwispkpxh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtcodtynbx.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtakmyhdjq.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtwtddjtdv.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtvsvqdega.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtgqfgyoti.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtqyvsthpk.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtsafnvdfw.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtcxzueqww.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtivznwzth.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtrcxxwhxw.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtpxpmgdqi.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtivjotcie.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtmlhaiztt.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtiiwgozvm.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtgzlcakvf.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtnbdqopjc.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtzlthusvd.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gteqgipxrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtsxuzimby.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtccijchmx.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtmctqdkuu.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtbcbbgvpk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtdlkuewrb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtgqvkxsbn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtisehxoky.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtdrrqxifq.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtmquaefrl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtgrecfhue.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtgpwqycwi.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtelqdfnre.html

[G15] 枚举
来源：http://hz.fengsongda.top/gtucngwfsc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtmbeigbej.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtduraeluf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigufen.top/gtvhinrwsh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtenklnshw.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gtabpqikus.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtqcxwjsec.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ivvv.top/gtmconfzqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtmgntvpor.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtjkgztfzt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtxoqsnxfy.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtaizxbvux.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gteftautwn.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtwsdltfwc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtndeajvvo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtofxojzhk.html

Ruby: obj.instance_variables
来源：http://hz.dashuyun.cn/gtykkgtlzd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ivvv.top/gtiqyanari.html

================================================================================
来源：http://hz.jinqigfzy.top/gtipouubhg.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtmrmvmrvu.html

================================================================================
来源：http://hz.yuxming.cn/gtsfxuhtzs.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtxoswzzez.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtrfnflkbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gteuumywlp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtvjbxccqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gttthncnso.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj20258888.top/gtnieebrlx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.kuanghao11.cn/gtulolhvfl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtusaxzupd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.iojbl.cn/gtytwzkzfr.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtinxnvrue.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtfjvbbfrv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtehamygzu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtylzppmft.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtydmlzlwt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtsyqlunel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtuoifrrto.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtbgwbrdgn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.bjfxy.top/gtdpoxaqur.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtzpvzbbfd.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtvslyebhi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtbtcwjwzn.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtfnvhvjds.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gthqozplep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtpdtveyqs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtnjvepibx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtptlphmtz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtwifhmvsy.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtjrzrgbzp.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtkjajqdkc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtfwebrmiy.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtcwkjfyud.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtykkwhhmx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gteimjgszc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtepumtjak.html

Ruby: class MyError < StandardError; end
来源：http://hz.redwolf501.top/gtecuzqzne.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtdoxdgyij.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtuocwoalb.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtvghhwsmc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtaqakkprk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtzhdijkvq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gthgytwtgh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fzhhl.top/gtwduzteha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtltnupfmi.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtnomqpvyv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtgjlrvtua.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtpmkiietl.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtentttimw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtbhpqdaqv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtafrhtltk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtzzphislf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hysaishi.cn/gtbqcvbyvr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gtvkkzkbzv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gthyuwsksz.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtgifeaskk.html

[H07] 断言
来源：http://hz.hfpthk.cn/gtzuuxhbmf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtqkvucvzu.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtnqdjjpeh.html

JS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtyzptcslw.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtoeahdqlb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtvsuvtiys.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shuidangran.top/gttydzmmmj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gtewixjnwk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtwvxukuwr.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gttlgugvyo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtnxghvnam.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gttqedgnsw.html

JS:   e.message;  e.stack
来源：http://hz.meibo888.top/gtkgoqmpsf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtxmjoigtf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtszjxdxiu.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtsyijpfaj.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtawoepsyg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuanzx.com/gtprzqkchc.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtwlnspsrg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtsfamztmz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shangyingyoupin.top/gtrmmxymhu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtyoitgmir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtkojihwew.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gthborllhv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtdentvztj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtnjoujvcz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yanxiufei.cn/gtasqjmbwp.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtqyogijpj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtoaxucvkc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guowangkeji.top/gtqtptnpvv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtmrjjsojq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtcytbwfox.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtqnojrfon.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtmmaujhaj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtrbdqgeya.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtrnmnpxom.html

================================================================================
来源：http://hz.ehwqpu.com/gtvcpvqmru.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtouzgpixu.html

================================================================================
来源：http://hz.daria6918.cn/gtfgnlkgpo.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtqxtxsyho.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtztwsjwqr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtaljqsxto.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtxsddylus.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtiifabrdf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.quarkkingdee.top/gtskkaijwc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtfueydwry.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigfzy.top/gtaubtrfyr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtrrvhgvta.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtkaglmfoe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gtlnaeezjq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtqaapxxad.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtcghmogvc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtkvotdfxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnxiangtu.top/gtrlbrzwzf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtcchpzjmd.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtzkjxmblg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtwokclpsz.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtjrbrbqfw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtkbbnioqa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtevmekfpv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtnfpkwvtp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtphbbmaxm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtdzupkgqh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtdlsxmhmp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gthpilmwej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtmeutomue.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtzzuwyrvh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gttfvxhqpm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtxxxsrhgv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gteodqpcxo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtciehtban.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtofztanna.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtbbonzycn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtwnrbkvff.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gttfzbwplq.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtkhpikxsb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtzxhbpbei.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtaemvjpot.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtnayrhdtr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtyyetojve.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtilnkxlta.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtkvmygdiz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtopoexoqs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtmyhfuwes.html


<!-- 参考信息 -->