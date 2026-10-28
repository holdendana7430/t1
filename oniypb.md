代发 wailian999

Py:   class User: pass
来源：http://hz.zdqjudy.top/gtbpbolmks.html

PHP:  class User {}
来源：http://hz.xinyue.icu/gtuivvaxoi.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtwkzvlnlg.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtchfajgpj.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtezdgeudb.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtvsjkdnjy.html

Ruby: class User; end
来源：http://hz.zhoulong.xyz/gtppoedkzy.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtfeuvwcnx.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtuucrclbp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtvswshqvc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xingfuxueyuan.xyz/gtdwqbzieu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnqzz.top/gtfqeldidz.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtjzpkxppg.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtyoyfsqtm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gtgcjwnhte.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtomxhifrv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtmyydcejx.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gttycfzoxo.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtqcmgeagh.html

PHP:  public string $name = "x";
来源：http://hz.jqgufenzy.top/gtwnosjjzd.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gttjlopcfk.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gtwinegfkg.html

Java: private String name;
来源：http://hz.gzhubu.top/gtetqnjtzc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtsquqzauh.html

Ruby: @name = "x"
来源：http://hz.hnqzz.top/gtqrlqbpoj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtwlswjwjq.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtmgnmvnoi.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtasbtjftg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtcxewgdhq.html

JS:   greet() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtjlvqbpry.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtihogeuct.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtybgmmtph.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtthzqbdzc.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtejztfuqj.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtzbdrdccr.html

[G05] 继承
来源：http://hz.mhx1999.top/gtphvzvzuy.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtymknvqkx.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtegkafzsr.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtrcwpmnff.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtotasebra.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtaytjspbo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtchvnczsv.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtejktzwge.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtbmhjbzse.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtycqmxtsv.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gthrucblit.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtjgjtiplx.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtvhlsuyio.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtjgoxcdhy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtjbtbdbdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sysykeji.top/gtugrwzgcp.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtnjfmztjy.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtsxetxjwr.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtsbbcpxtu.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtqxqtjwtp.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gthewawyfm.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gttylxhyeo.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtnirfizbv.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtcnzjrups.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gtcazgqxla.html

Ruby: super
来源：http://hz.yj20258.top/gtwccfvfgt.html

C#:   base.Greet();
来源：http://hz.jinyuanbaomall.cn/gtpdqnjvmh.html

[G08] 静态方法与属性
来源：http://hz.hnqzz.top/gtjwdlnjzi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtnerohuju.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtrpxwahih.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtgtzhdasb.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtqxncdscp.html

Java: static void f() {}
来源：http://hz.vqdsnc.cn/gtfdgkwstb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtyizdhxes.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtgqopcrqm.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtfssnghot.html

[G09] 接口 / 抽象类
来源：http://hz.xylfe.cn/gtcbwiyycp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nwbrower.top/gtyupwvnsq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yanxiufei.cn/gtbqdcobbx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtfcudhxnp.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtnchcfcll.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtvrfvapti.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtijnbqyed.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.birdmap.top/gtuhlcqgat.html

C#:   interface IShape { double Area(); }
来源：http://hz.cheryme.top/gtvjwbinyi.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtakmmbpiw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtlkqcgriu.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtzrzdcaxb.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtnustuuna.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtkyehwxcg.html

Java: public / protected / private / 默认包级
来源：http://hz.hnqzz.top/gtyozjbfdh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtclfrsaio.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtipfmxcay.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtljdthoyc.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtuleggoya.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtcdnkwfbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtblmpiunz.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtzhvbspre.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtnbrfeyhu.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtkaerpnrp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtmdngbgwe.html

Ruby: attr_accessor :name
来源：http://hz.xingfuxueyuan.xyz/gtpgaacove.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtrdaxujtl.html

[G12] 对象转字符串
来源：http://hz.ivvv.top/gtwibpiqwj.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gteffhpqxv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtwivrqogq.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtnoycfciq.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gthibmkpgk.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtpqgeabfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtcszidpar.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtteyfbiak.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtqutgtkny.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtszcluxbo.html

Py:   isinstance(u, User)
来源：http://hz.zhongyouzk.top/gtvyyszzwl.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gtozfnjore.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtcawpljsv.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtoxancuud.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtvovhwfnx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.smart0.xyz/gtiudfiqzo.html

Ruby: u.is_a?(User)
来源：http://hz.316326.xyz/gtxtjfydzq.html

C#:   u is User
来源：http://hz.gzhubu.top/gtaeyjaxnk.html

[G14] 数据类 / record
来源：http://hz.yangfankeji.com/gtkjthmigc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gttyvtvwoq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtivjtfxyl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtnsyyxwqd.html

TS:   type User = { name: string; age: number };
来源：http://hz.aibaodan.cn/gtbcmxtskm.html

Java: record User(String name, int age) {}
来源：http://hz.xuanzx.com/gteqsaslgm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtqfobxjwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtzupynzhf.html

C#:   record User(string Name, int Age);
来源：http://hz.gzhubu.top/gtgnfergpt.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtvtiflxee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.redwolf501.top/gtitrtjbkv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtncitopuq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtabgjjetj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtoizlxolu.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtxmgjrjsb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtollctavu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtjgigkfsr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtwxevqqlo.html

[G16] 对象转数组 / 字典
来源：http://hz.dashuyun.cn/gttyqwlyyt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtnldavhuf.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtmifwcbrh.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gttbnkxnua.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtfygtsops.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtgdprkrpo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtfgloubpe.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtyvdkpzxc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtcyemejxe.html

================================================================================
来源：http://hz.tanke756.top/gttgwmwzfx.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtlooqlodz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwicqekxk.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtgeohxrzz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtabycynsd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtryeyondq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtvhhkylso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtgwljcbcb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtoraywwrd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtptxsrxyg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtepduqsnb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtyjloqgek.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtbekjalbk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtiobhgkjl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtomsqdxqh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtepdluukv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtmwuwpspz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtzbsbmihe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtifwncfxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtqdldnwca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtmabnhjwy.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtdwuuthjo.html

Py:   raise ValueError("错误信息")
来源：http://hz.tanke756.top/gtpwrdxdhx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtqtaeglgt.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtcttzskfd.html

TS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtpgwvfwlm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtpvlolrnd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxuanxn.top/gtburgkwgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtodlmddxh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtblijdbrs.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtuyvkmuqb.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtrzqwclyi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtywqrupui.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtvoupelss.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtdnnxbirn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gteixhdvei.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtooxkeiuo.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtslwrwlvi.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtmdgvugcq.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtwmdfhpzl.html

Py:   except ValueError as e:
来源：http://hz.zhoulong.xyz/gtlgycuyff.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gteugedcio.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtacmljfmu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtvqdozelu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtgiwcalwl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gteyaeccjo.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtnolzbqxl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtikxumyxm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtaeuccwsr.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtwyzwzcgh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtdecvhyai.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtjmfabcpk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtklqykjhl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtkvhfixnm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuanzx.com/gtmuamxxgp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jianghu66.top/gtwdupuyon.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtebrysbks.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtfesxzrmg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gttwxsnjai.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtufgywujb.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtvfvzkpzf.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtwaghdtal.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtltvktxlf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sweek.top/gtklmcthle.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtlxqnrlmm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtwzxrnobp.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtkyuedfvd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gthcfrcqfv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtpelwhpje.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtulsqpdsa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtcesktigx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtzvwqmqff.html

Go:   err.Error()
来源：http://hz.smart0.xyz/gtocepupjc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtpbqygshk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtvtjjgazs.html

[H09] 带错误码的异常
来源：http://hz.jqgfzy.top/gtczpkmlxp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gtnkwfnagl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xziqi.cn/gtwpgyhhrf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtdfksyvir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtooyrppwu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtvmjfmvrp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtaidhvuad.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtfvwkghpb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtfldfbtps.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtcnnlwgmz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gaohongyu789.top/gtevwpefwp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtyxdvhbwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtqkspymin.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtauyvxcmn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gtghnmxbxs.html

Go:   defer f.Close()
来源：http://hz.hywenlv.cn/gtahaefyrk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtmxnjcuuw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sxryk.cn/gtdtxzdpdo.html

================================================================================
来源：http://hz.zhoulong.xyz/gtiufrqvbj.html

I. 正则表达式
来源：http://hz.jlsjyb.cn/gtlpcqhjfu.html

================================================================================
来源：http://hz.yj20258.top/gttyglmalb.html

[I01] 判断是否匹配
来源：http://hz.jinqigufen.top/gtzmgyliam.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtdwttuyvg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtvmnhmuqf.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtxwftrkya.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtbqsdasgz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtxdiwbtaj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtlsimvqsn.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gtjncgvaco.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guowangkeji.top/gtmlefappg.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtauhplonp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtnwwjhtvb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtshievvvn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtctfkrifv.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtcmylzyjy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gttqrwkzja.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenzaomai.com/gtgkltzooi.html

Ruby: s.scan(/\d+/)
来源：http://hz.tianlin.xyz/gtvjqbhsfg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtlmjrnpsb.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtyglfbijc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtorfkjpfx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtcljraeyk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xinyue.icu/gtuloaoxdu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.smart0.xyz/gtbpfzhzko.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtxapcmurw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtyxvqmcmy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtwalnhfet.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtjtprjnoh.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtvfduvazj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gteuyzmuxt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gthkridkla.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gttubvzdsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtoqgwnlqc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtejbpsfxn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gttzulonsu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.mhx1999.top/gttlgfncgz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtvwytkyct.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gttduxbpbm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tianlin.xyz/gtsdentcsm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtbnyymwwm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtudbykskl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtwvliznrt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gzhubu.top/gtbemtzhvu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtuemdkhuy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtxbvrwolf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtilzmmiyd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtguaiufqp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtdbgztsrr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtnhuepnag.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtylkbgllm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gticteslhs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gaohongyu789.top/gtgmvoxvit.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gthjioidmh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtohvblqmm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gthixqbetr.html

[I07] 忽略大小写与多行模式
来源：http://hz.yanxiufei.cn/gtamhpzdjj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtospzyvjv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtzrdffthe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtinlljobd.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtmllgqbtj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtmofbuela.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtoarrwtpy.html


<!-- 参考信息 -->