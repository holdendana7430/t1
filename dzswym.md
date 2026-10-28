代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtpquhsnvm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtdvxuguau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gttdjygxzw.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtmefgolzq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtsjxwoszq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cqqwz.cn/gtfdmukdmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtlyjfkumr.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtkuwhapde.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtoagbcbpf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtzkhlmssi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuetiantiany.cn/gtdswclxid.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtneizmjck.html

================================================================================
来源：http://hz.cqqwz.cn/gtqnqtnvci.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtpszjbgwr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthtmqtmsd.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtrjmsyttg.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtyinlkzml.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtmrvipjfe.html

JS:   class User {}
来源：http://hz.yvedp.cn/gtmvnspnkd.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtjifwruwb.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtapgbeepq.html

Go:   type User struct { Name string }
来源：http://hz.tian-w.cn/gtqcsgmzhq.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtdlxdmggl.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtgdjpkgoe.html

[G02] 构造函数
来源：http://hz.havefunace.top/gtfcxotzcz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtcymdibxq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtrymbcspn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtsvunjbnc.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gteyizqnow.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtuiaghsfi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtawdaqnfr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gttljmtijc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj202588.top/gtnjvqfrhc.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtbpdbghxq.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtmthquhxs.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtyhcpqrrd.html

JS:   this.name = "x";
来源：http://hz.zhiwuduotai.top/gtpjjjvdtx.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtlncffomx.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtagowopks.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gtedswjoie.html

Ruby: @name = "x"
来源：http://hz.jyoumei.cn/gtsxwtbqys.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtrntvuuki.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtutrmdyjp.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtzjzwhjnn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtqtjahpgx.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtvpysamrs.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtriucedtr.html

Java: String greet() { return name; }
来源：http://hz.nanxuanxn.top/gtybivlbnu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtevligfcb.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtanggcdss.html

C#:   public string Greet() => Name;
来源：http://hz.jlsjyb.cn/gtphhzutag.html

[G05] 继承
来源：http://hz.pycfn.com/gtksiefprw.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gttghlktlt.html

PHP:  class Admin extends User {}
来源：http://hz.ehwqpu.com/gtujgxfsmp.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcdgmujxr.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtlqkmerae.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtvqzluqqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gttglkpevh.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtgqlealeb.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtgcctqfzp.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtwaengvyg.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gteihradjt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gteurahmwp.html

JS:   greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtoijbuyxu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtxhpzekio.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtcnlpgvec.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangshuangyany.cn/gtjifbvhpv.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtznrrboly.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtxsjgnrdp.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtxvconzwr.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtgvtzwraz.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtbmwubfai.html

JS:   super.greet();
来源：http://hz.daria6918.cn/gtpzfgpnig.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtyngbsade.html

Java: super.greet();
来源：http://hz.sweek.top/gtsinojmme.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtpqytzpwu.html

Ruby: super
来源：http://hz.gzhubu.top/gtskrjfnhc.html

C#:   base.Greet();
来源：http://hz.zhiwuduotai.top/gtyxfqgbmw.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtufvavtto.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gtuoxfuqxi.html

PHP:  public static function f() {}
来源：http://hz.gogol.net.cn/gtgocsxyvq.html

JS:   static f() {}
来源：http://hz.shuidangran.top/gtxusysojy.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtqxxmwxoi.html

Java: static void f() {}
来源：http://hz.jinyuanbaomall.cn/gtiqbtrpgc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtvzpqaxut.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtkrcpwpzn.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtdrflpwus.html

[G09] 接口 / 抽象类
来源：http://hz.hfpthk.cn/gtkbhvqizx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hywenlv.cn/gtfwvrkufk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtuhuzgaft.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtzkxwfgiu.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtiudgllxl.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gttttugggj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhijiandao.cn/gtqhqqyptc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtnzgafviv.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtyaahyqlo.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtvsicljcq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydjk.org.cn/gtqbvjtako.html

PHP:  public / protected / private
来源：http://hz.yuanzhike.top/gtqmewmmln.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtnvstypvj.html

TS:   public / protected / private
来源：http://hz.yongpay.top/gtlgjzwgma.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtzqcozwsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtelrjnvqf.html

Ruby: public / protected / private
来源：http://hz.jyoumei.cn/gtyequusfs.html

C#:   public / protected / private / internal
来源：http://hz.hfpthk.cn/gttlyzaoxy.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtcpkfklil.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtmqbbcdsw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtaezhkqld.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtvtjdnssa.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtnjkfaxut.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtpnofezaf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pycfn.com/gtdajkdydg.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtyaiovhon.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtpvctfwoc.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtvijuduct.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtgtohurxk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtytrlnndi.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtkwxbtduj.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gttfzdahpa.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gthlwfvbda.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtaxjbowmh.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gtiiuilagr.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtvpzspuby.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtzwlgiqeu.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtgbvujqqi.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtclffubpv.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtvlrrlevy.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtaqsmngjx.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtofvrbyxj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtiipdncmh.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtwtwwqvsi.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtabztxgqr.html

[G14] 数据类 / record
来源：http://hz.yj20258888.top/gtegtwprdz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtcymuiram.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhiwuduotai.top/gtmmshiwoy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtbqurtuqk.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtmbldbuny.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gttpppycsi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtmlllksdn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cdnleiting.top/gtfbdsrfbv.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtkzwpfjch.html

[G15] 枚举
来源：http://hz.vqdsnc.cn/gtypblumoi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtvqpoiilb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtgaxdnfsf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gttzcdktgr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtacoijzcr.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtfqyrtkdr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gtypncwjqz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gtfhvivsut.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtkproagxc.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtqkjquczi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gotoacloud.top/gtmrjjjfrx.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtzsxpavlm.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtxbyouagn.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtapfcmqvu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtbvhxoikx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtcubcfhtm.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gterthzzch.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtwclvteis.html

================================================================================
来源：http://hz.hywenlv.cn/gthcjxkadk.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtktfjdnmr.html

================================================================================
来源：http://hz.jianghu66.top/gthexdriub.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtdudzuvpe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtcsokgzmd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtchtpqrtg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtaybieeay.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtpvpyuttu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtodltibga.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtckuzmjvs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigufen.top/gtpjxxzvux.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.quarkkingdee.top/gtxkyirnws.html

[H02] finally / ensure 收尾
来源：http://hz.cdnleiting.top/gtuybrifnq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtecknxxkn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gttgqoavtu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtlvdlaags.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtpxpcvlyh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtskpkoodo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sysykeji.top/gtepzvhoqv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtmzibxqks.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtdobtbnfp.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtwlxewdhx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtklwpdadz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtwfqnxzha.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtpwxwlbqf.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtuskxqkyz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtzdwahjza.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtwifuhxmz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtoagpbtrv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtuurmmawq.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtdigsydpj.html

Py:   class MyError(Exception): pass
来源：http://hz.hywenlv.cn/gtnfttvpqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtzteobmzl.html

JS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtgjpwvlsw.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtabkvcfig.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtsbsxhrdn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtuoxnpmnh.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtzwfpcirb.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtqhsidhdd.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtipkbnwzc.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtzpyfhvvr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gthaysrhdz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtsjxqssse.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtqebjdjba.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtvpzfuzty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtvoniipkw.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenjidiqi.icu/gtltervhju.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yueranfly.top/gtbyirnikb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtiytmmsif.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtqajdrtdn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtacmccxtg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtjtvwpbqk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtzgdhnzdi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtmjpbilcw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtttsmjuvk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtwutgiaiq.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gtsnuyegyq.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtgyyyhlbz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gticqbhkon.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtdrwncgfu.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtxcfuaxim.html

TS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtrcbjyfwg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtltwmqdcj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.redwolf501.top/gtctpdsyql.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtqnnukvjs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtyxilxxhf.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtiiztydpe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtbktyojpr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtbiasbdha.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gttqmxtxes.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dashuyun.cn/gtzpwkwcvl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shuidangran.top/gtwhoebjsc.html

Go:   err.Error()
来源：http://hz.smart0.xyz/gtxpyoqagf.html

Ruby: e.message;  e.backtrace
来源：http://hz.sxryk.cn/gtwguprnrg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtfvucbvjd.html

[H09] 带错误码的异常
来源：http://hz.aizwys.cn/gtsyqbpful.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtdsqazpdw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtsrpdazqt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtgmvryibb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtwrmzoisi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtpdoyfjri.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtkjabqhge.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinyuanbaomall.cn/gtnouqmuel.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ppjwa.cn/gtigvzsian.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtfnknxlas.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xylfe.cn/gtdytcydxt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtmubksace.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtoitkqdgf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtbsosthfz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gthkobrhek.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtusweqnug.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nwbrower.top/gttaxtqidn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtdnrynoqc.html

================================================================================
来源：http://hz.ydzc1.top/gtjoafcswm.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtpzsooewr.html

================================================================================
来源：http://hz.yj20258.top/gtymzuuvjw.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtdwzcqkjy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtetyiiatl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtqmvsgymp.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtfmnsxkzw.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtaczsrxca.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtyfvsltoc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtwmvqdqqa.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtloygzokp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jiagoushi.top/gttnurmnqg.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gthpfowgdz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtnzpidzwl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gtecoqccpe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guannengcc.top/gtfoniggmi.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtawmoxnbx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.snrcjt.cn/gtommcqcil.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtaljlbyow.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtqfdphvet.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtyrpsxadf.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtqfqdnlow.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xingfuxueyuan.xyz/gtvcgfeinj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtmnmtucgz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtwudukhtf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtdkfdmphr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtqvrxzbhi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtahqadpwk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtmzckwxpq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.meibo888.top/gtrghcfflw.html

[I04] 正则替换
来源：http://hz.jinqigfzy.top/gtskbfahvo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.316326.xyz/gtbbfhpikc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtvoftsgpi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtuzqnjzoc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtfvwbvxci.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gttewiwmyu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtsiqyyova.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtmfnvuzax.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ywan-chungtsiang.top/gtemmvxvnz.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtljxpuiah.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtrlhrissw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtuqbncvtb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtaruddevj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtslpdmlvw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gtckpqdqeh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sweek.top/gtnoteuyhi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtrjmskwfc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtzkckynnt.html


<!-- 参考信息 -->