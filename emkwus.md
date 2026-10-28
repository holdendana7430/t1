代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtqfexxheh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtbnlbfpmr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtxnkbsmvr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtxzmvyhbt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmimhhxje.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtfqurnajp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlfyduoru.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtudhvcdob.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtapzvtqcb.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtsmjlzkjf.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtcdmvtdnk.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gtlqyyjpje.html

Java: class User {}
来源：http://hz.smart0.xyz/gthdeudmlb.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gttldiekgi.html

Ruby: class User; end
来源：http://hz.hnqzz.top/gtuiotqxqh.html

C#:   class User {}
来源：http://hz.yvedp.cn/gtjhubcqdd.html

[G02] 构造函数
来源：http://hz.yj20258.top/gtmbjmmvcs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtlgxgwegq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dashuyun.cn/gtzypspdiq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtljyxmgiu.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtixwkvrgb.html

Java: User(String name) { this.name = name; }
来源：http://hz.ybcxt.top/gtiwnkoydn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.quarkkingdee.top/gttaweirba.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtucjheyyt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gtckfbzpax.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtlmlxqfge.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtbdygpncl.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtmuouchgx.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtajlupmou.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtarrajpbs.html

Java: private String name;
来源：http://hz.redwolf501.top/gtafuadthn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtfltiwuhp.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtskcqyboe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ppjwa.cn/gtnikkjuaa.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtmpvqjmqq.html

Py:   def greet(self): return self.name
来源：http://hz.shzxlz.cn/gtashxcrwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtncndipck.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtyufyhpcf.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtddbbzecy.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtlrkwdbvu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtpqvfglxu.html

Ruby: def greet; @name; end
来源：http://hz.hysaishi.cn/gtuvbaeemy.html

C#:   public string Greet() => Name;
来源：http://hz.aibaodan.cn/gtuaftvjhy.html

[G05] 继承
来源：http://hz.daxiang520.top/gtjpnfqwbi.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gtlngvcfxn.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtxwegczvl.html

JS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtncnycjgf.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtwrjxfgvw.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtjlryvgfs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtnwafmxgw.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gteyrwsgwb.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtpikvepzm.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtlnbatove.html

Py:   def greet(self): return "admin"
来源：http://hz.xylfe.cn/gtfoshzgdu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtphganptr.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtumrdhhjj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtabeseqey.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gttsqqpftk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtvxrxsnkp.html

Ruby: def greet; "admin"; end
来源：http://hz.cdnleiting.top/gtwowtpnoo.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gttcyahsln.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtamwfprnh.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtmqafrqrn.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtcqmvwhrj.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtrafrgwwk.html

TS:   super.greet();
来源：http://hz.tianlin.xyz/gtkqypbjjm.html

Java: super.greet();
来源：http://hz.sweek.top/gtgzebncrs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.bjfxy.top/gtnzvmzliq.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtxhzekpph.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtdstvbulp.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gthqofefzo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gtrycuwnfh.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtaryeflye.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtueqbjalj.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gtvlsbynlk.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtixshiopa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gtpxxyecvu.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtyxxdqdqf.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gttbcrtguz.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtftbvkkoq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtcrfnfydk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuxming.cn/gtcjeikips.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtykwmqzuc.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtagkanvao.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258888.top/gtqsdgmxeu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gtxiluaodg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtgsgoxdgj.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtdoppmkrm.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtodknhmkl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gthphxdfxu.html

PHP:  public / protected / private
来源：http://hz.redwolf501.top/gtabrzdgxz.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtfzypyakv.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtumppweri.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtmeclisec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtkmpolufo.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtvbznqdas.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtprchxxfa.html

[G11] getter / setter
来源：http://hz.jinghuilouyu.cn/gtclhgzinv.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtjqaasjnv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtlkjhnnou.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtliiyoyhd.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtkxfyjyax.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtfqxqggef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gteqqjfqgh.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtzqrdwirg.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtwushpadq.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtvqnzshgt.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gturuygyvy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtcjcfzumt.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtkvvkfioc.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtxqgmwvrq.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gtsackldxc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtbcjbcswp.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtudizxfee.html

C#:   public override string ToString() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtjgvbdwom.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtrnubnlwh.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtziqxeogd.html

PHP:  $u instanceof User
来源：http://hz.tian-w.cn/gtqhenalkh.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtixiixpww.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtwicuwbys.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtzqnegavb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtocjzhstc.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtizfdoicc.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtrtctgmwb.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gtoxcvdaay.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtyirktzxh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtdbsffchf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtqwctywig.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gtanlsdhqk.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtwlqmuyzj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ybcxt.top/gtdzcrllnx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtqngyggkg.html

C#:   record User(string Name, int Age);
来源：http://hz.chenzaomai.com/gtlbzkbmxm.html

[G15] 枚举
来源：http://hz.yueranfly.top/gtwktbtfvi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtpnwggcsi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtowwlhscz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gthbmcthkp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtpdblztni.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtpaceujps.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gtdjudefew.html

Ruby: Color = %i[red green].freeze
来源：http://hz.haohaochexian.top/gthtsxsozk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtlvjrtyyh.html

[G16] 对象转数组 / 字典
来源：http://hz.chenjidiqi.icu/gtpxtqcmji.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtavgibcjz.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtmwkukktf.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtmojpshtl.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtunltmopp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtkgaqbzej.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtftbtxmqy.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gthkifshrj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtisdzfmed.html

================================================================================
来源：http://hz.quarkkingdee.top/gtaihhdifd.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtqdzkcana.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmduytljs.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtcsxnqasr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtrcekgwch.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gthfjjbzoz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtcswwvvme.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtzwiamdbz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtkplacgbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtsujzdqjw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtmgjrdqdn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gttxkuynaj.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gthjcxgron.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtlmvuzygi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtbkhcjxfn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gthchkabuq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gttpecfvmr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtyxbqvmhf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtoqrhcwlp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gaohongyu789.top/gtfhmdjwzk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtfqcmxgfa.html

[H03] 主动抛出异常
来源：http://hz.yvedp.cn/gtbfgabzpv.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtxzfgmtsh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtbhmtvozm.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtkdlafgqd.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtkoghucjf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gttpvnncqe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtpwnzazso.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtzvyqzgff.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gthlblrwnu.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtrxgqdzzq.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtvxofmlaf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtpwtqbiij.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtmzdjgnyr.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtzvmynxkh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtpstfobnk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtblxgeehi.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gtormwqqgw.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtwthurbvi.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gtekjcrqcy.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gttjepgeco.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtnzggzbvm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtpbdsxnaf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtqndfqhad.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtvfledvyz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhoulong.xyz/gtemvehcnw.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtltidbyvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtkhgifiya.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtjjmzccci.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtiqaquyem.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtnkermkix.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtvocqlvnu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtqaefwnrj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtscymjfrm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtewyugdrl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtzditrarf.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtkrbcohqc.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtwpfczpha.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtkhaawlel.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtfaxvldwd.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtdvopxzbu.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtidzjvajm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ppjwa.cn/gtcsjsogtg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jianghu66.top/gtkcuppycj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gtpugmqwkz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtoifgqlof.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtehfeinrn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtqprtzqwb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtojyejcbq.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtezddkfbe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sysykeji.top/gthoytnxnj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtzkpskubc.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gthlaazpad.html

Ruby: e.message;  e.backtrace
来源：http://hz.shzxlz.cn/gtxyymyvqt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtzabdcakp.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtlddsbqjh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtunnoamde.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtmslrkevc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gthclviiid.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtlbrnacgu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtpigbqase.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtwjxsxwdc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtljfjavvl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gtuciaitqi.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtvehateve.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtohrevhwx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtnyhlinji.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtnkppjcpk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtjepfwlvk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtiidtzkek.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtaomzgpas.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtcoeoesib.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtppzkcdzh.html

================================================================================
来源：http://hz.havefunace.top/gtftcrxodn.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtuyjoilra.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwbormoeu.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gtxoisjrqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtylxdvsny.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtqkkidhwq.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtfzwnthjq.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtsjmiwafb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtkmpdisij.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cqqwz.cn/gtdclmpost.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gtbremjkwb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtbbxqhube.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtiwldrzdu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtsxxwouux.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtxnsrxshw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtbjtlvbrg.html

TS:   s.match(/\d+/g)
来源：http://hz.yueranfly.top/gtnfuufqhz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtlyvptcgq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtqfdimhaz.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtfkhiesqp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shangyingyoupin.top/gtfbdwflns.html

[I03] 提取捕获分组
来源：http://hz.cqqwz.cn/gtznydpnko.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtmolhlouc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gttnonrjrq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnqzz.top/gtxamttpxc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtoduchctt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.iojbl.cn/gtjrhiywsc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gthcxetxcb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aizwys.cn/gtjobqxmfl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtmircdueh.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtnzvvtxzo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtcgyepvfs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtcojffpsw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtqjhzlksa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtipuewwhb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sweek.top/gtdiejjlsy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gtbrvvnnmn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtsbefjbro.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtcdgemzwj.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gthdhgwftg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhengqikj.top/gtfhchdizw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtftimjzqx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtvmcpkzld.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtemyifnxz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtwiicbzob.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtcabkecac.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtixeyabhm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtzjdsrhvp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtmtajyfzr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtvmnxnatg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtcpszhraf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gteenvyxxv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtwhdigwqv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtquagapsn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gthfmyptec.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtfykwfojl.html


<!-- 参考信息 -->