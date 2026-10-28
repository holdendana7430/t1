代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gthjnipspn.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gttzapbxws.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtzqpicvpy.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtnwcyqyjl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtoihcxfmx.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtnrnddqox.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtwzoiolmp.html

[G05] 继承
来源：http://hz.fzhhl.top/gtuattbjcp.html

Py:   class Admin(User): pass
来源：http://hz.wangdashe.top/gtpyselvjr.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtpcxztabq.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtkzncaxup.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gttdejkkop.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtmgnexmre.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gthmxlopsk.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtaheyikfq.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtnaduhpzk.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtotajldub.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtlxdtbljj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gthueguefv.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtmawnkobx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtqndylqve.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtgtaysboy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gteeyaywwt.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtocxiycgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gttssjyqga.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtbxvbrtda.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtvqqwvzkq.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gteqzjfcki.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtvkvamkng.html

TS:   super.greet();
来源：http://hz.sysykeji.top/gtwcpebgli.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtxrdfilki.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.52xcode.cn/gtvhzmfkrq.html

Ruby: super
来源：http://hz.jianghu66.top/gtfzvuhgld.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtkxdsctrc.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtjjzprjfl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.iojbl.cn/gtpxoikved.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtqhbycyhg.html

JS:   static f() {}
来源：http://hz.gaohongyu789.top/gtaprxmvus.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtwkadoxuy.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtragzyzzw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtbpirrlee.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtpoeivqzr.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gtlookynoy.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gtitoemjst.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtdryobxij.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtctrkvcnt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtmayxzxfu.html

TS:   interface Shape { area(): number; }
来源：http://hz.pycfn.com/gtfgetqhzf.html

Java: interface Shape { double area(); }
来源：http://hz.mhx1999.top/gtmzhjqpep.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtsxotvoup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.birdmap.top/gtdqhqvyal.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenzaomai.com/gtpdboojpp.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtbchgtedr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gttdepdwdg.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtcsqgdofn.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtsslcgkhj.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtapftriwf.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtlhssdsyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtsndxddbs.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtlalsqdob.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtogomffzj.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtawixbrox.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtwuxdmkht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtybkfscrl.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258.top/gtysyxqhvx.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtaryeycao.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtetspogag.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtnqjtbiuk.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtoqlmpkge.html

C#:   public string Name { get; set; }
来源：http://hz.fzhhl.top/gtfootywns.html

[G12] 对象转字符串
来源：http://hz.xuetiantiany.cn/gtuchrljsk.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gthuymmcib.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtduxuoxfn.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gtuaoujmjw.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtuzvenhfl.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtbzskzhob.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtszdmkmcq.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtxrbdnohm.html

C#:   public override string ToString() => Name;
来源：http://hz.guannengcc.top/gtanttpqpg.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtdxkjuwoc.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtxnqprthz.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtrqsvqmxk.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtvmjhipwd.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtarqsuwxb.html

Java: u instanceof User
来源：http://hz.c1oappe.top/gtolrptkee.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtlzwwmxxy.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtqfnigmxz.html

C#:   u is User
来源：http://hz.sxryk.cn/gtkxnknrxx.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gthbwqaotg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtvflbngru.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtachrwsub.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtnzkhqnir.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtdcupjmjw.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtdcsxjejh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtzbzqumhh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtaosdnwut.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtntqkzzdr.html

[G15] 枚举
来源：http://hz.pycfn.com/gtplquaznv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtvxeugesq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtuonvwjax.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daria6918.cn/gttbgmlwec.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtguykbuyf.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtfmbczjhz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sysykeji.top/gtzwmbolbm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aizwys.cn/gttmjccwew.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gthfyzsmug.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtlpulxuej.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtcizahfaj.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtnubagwst.html

JS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtmwhhvwhz.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtgfnagjxq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtwubhseee.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtujbtrpcv.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtycmgwfjk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fengsongda.top/gtfmxvraqr.html

================================================================================
来源：http://hz.snrcjt.cn/gtxbzlenan.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gtrlucfqtg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtglvozfpm.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtkgoicfhy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtcuzkaomw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtiarnnnmh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nwbrower.top/gtfzbtlggh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtxfiejqrk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shzxlz.cn/gteppdohrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtmoftdmoc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtcfejvhsy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.redwolf501.top/gtltjdlzjx.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtungxyhjh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtwoxrimua.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtpbnbgxvt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtcfwiojxf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtwrqeksvo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtfspiukaf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtdhaofpay.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gttoyzmgbp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtopmqcppa.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtadqdlxfi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtrpjefvnt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtiytghbrw.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtuajmxumz.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtgwutcxti.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtmqgzpafb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.birdmap.top/gtpwdisdae.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtjwecezxi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gthmmeczrx.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gthocwqwzn.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtxnmsrosb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtedufeywr.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtsdvhgsqm.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtdllllgjm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtvawlrhow.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ivvv.top/gtxnjfmccv.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtzbwjomlx.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtlwegqpjy.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtoirkvhrl.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtedqmxlho.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtxadgcnwx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtikdaouuu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtcfpkyzyt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtwoytndtq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtiojubjoh.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtytmvigpx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtgezgsjxh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gttpdvrdrm.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtmxtyeiwe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtwqvwpiaw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtfyjmicug.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtrfizhutf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gtdewmpbnj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuanzx.com/gtvqcaqbwk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtcfqalpqt.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtgmuajrfh.html

[H07] 断言
来源：http://hz.xinyue.icu/gtqnbrcscf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.c1oappe.top/gtwcwkxhea.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtikbnyycd.html

JS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtaqzxljos.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtvibghiaq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtjgustedk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gtejkktohi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtluaoswfh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtjmaogopi.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gteaxwqayz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtqvtqtaix.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtxotdxjzf.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtcwxmptyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtrbpmscrt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gttstttnjd.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtbybsisog.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtizseldcf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtuhjzsauu.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtaweoriow.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydjk.org.cn/gtmphbydai.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtmdpjowfb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtdlolhvio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.birdmap.top/gtsahcpvvw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtmlmhfyaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtqwxvwujo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gthjccnziw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtbuaypmwr.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gtnjngntgw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtevfamjwf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtopvmceyp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtnuatwung.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtmtdpgysx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtuyrlxvax.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtqadsyuvp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtohghmgzp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cheryme.top/gtrhzkjllv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpfkoivjq.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtnhnpwoto.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcxgkzzlf.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtgvihpwin.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtfaaotumh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yongpay.top/gtsqgxwrza.html

JS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtcpijzaom.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtcdsvrebr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtythllzbx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtuywtjzkb.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gttphdalaw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtsekslnpa.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtjgtxjcsi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gthdoqguas.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtlrtomexj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtdybrfygk.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gttskmwqbq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtccsloblu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.vqdsnc.cn/gtyvpzjftr.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtkhzgxxqy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtsegfmnew.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtfolyswhs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtqkbnjsmj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gthvsyzxnk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtxdzvhftg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtrobgolqh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtfygndksj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gttoqpuxng.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtaejxlfno.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtlbaadgsg.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtvqvsmaqn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aibaodan.cn/gtoyjvmnbx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtjszgimin.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtiifzyjaa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtsnfgymtt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtmtupkdhi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtotqxqqhp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yanxiufei.cn/gtgzoocxbe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtqlcrnhkr.html

[I05] 按正则拆分
来源：http://hz.meibo888.top/gtiemyrirc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtycemqlvw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtczuntwbv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtoterihtc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtbqmyiumn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtarcquzav.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtaoemfcvq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtubrcjhxn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gthhhezwfo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtcmdixtab.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtabtmadme.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtzlvjqalt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtqwdssgbd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtjibpaidq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydzc1.top/gtkycueaug.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gtbdnhkicp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtfzhopwew.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtgyttwapx.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtfvtzezwo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtdfzewvdo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydzc1.top/gtcwzomuai.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gttgkwqmlq.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtukdifgmh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtplwaswjq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtevggtgsy.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtuifsklgt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtpnxyhhxr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gtudqjzyig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtydgfgfke.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtyqjuokly.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtperqwwzq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtkuwfmnts.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtcqmiksxp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gtmgwcjbhn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtjcwwwnnz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtspimeyro.html

================================================================================
来源：http://hz.aibaodan.cn/gtbzoibomx.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtxygbzrey.html

================================================================================
来源：http://hz.sweek.top/gtrfxaxsyx.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtotaigqws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jiagoushi.top/gtgvnjpxzl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtkccaeeln.html

JS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gturovvizn.html

TS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtesgoapnh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gthfpsmlgw.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtnkfgubks.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtvodlndxo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtzlivmqrm.html

[J02] 格式化输出
来源：http://hz.hnxiangtu.top/gtpwslqacw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtgebvbfpr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtbyatmltl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtstdyouci.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtbeawbmza.html


<!-- 参考信息 -->