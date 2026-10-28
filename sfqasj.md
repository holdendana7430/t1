代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtcmfcrhiw.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtdvmiaepg.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtmusaiqzr.html

TS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtzbjuzjsi.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtkecpsopu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gttysjrajq.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtiwtyfrrc.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtgrqslkrl.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtmtdrtcmv.html

Py:   def greet(self): return "admin"
来源：http://hz.shangyingyoupin.top/gtwusgdfxn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtadkalcrj.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtjvagkbbr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtzwrnktlk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtteadizdh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtkhlukrjg.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtvdutqaww.html

C#:   public override string Greet() => "admin";
来源：http://hz.haohaochexian.top/gtjsfwygqt.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtbafhkckz.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtwujxgurs.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtpcxczdch.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtnliyxkem.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtdukbnvgy.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtvtdzrane.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtjdzkfels.html

Ruby: super
来源：http://hz.cheryme.top/gtiufixrbo.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtuyxtgcet.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtfcttgeur.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtfzgfkpom.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtfpkuosni.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtwmbrssfx.html

TS:   static f(): void {}
来源：http://hz.jqgufenzy.top/gtzjkdgjok.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtzkkbsvrk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gtqxxjgnzh.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtwhhteaov.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtleabqzit.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtnkdoxcoq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgufenzy.top/gtxcqnupum.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtoymdzvpg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gthdyylsgp.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtfestdyxj.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258888.top/gtmfukysgi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gthqnphihp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangtech.top/gtretwumzj.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtylaljgqy.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gtbexgtruz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtwribjbuu.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtoqprkbgo.html

JS:   #private 字段；其余公开
来源：http://hz.52xcode.cn/gtppcankmr.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtqygoxwlr.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtyvlgjznz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtmzbmoojr.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gthooreiql.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtcaqhtobb.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtehkakihk.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtwasmlbmf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtcktdmtog.html

JS:   get name() { return this._name; }
来源：http://hz.zycfv.cn/gtrctrtcqw.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gtsvapzpja.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtlbtmpfwe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtnmmitibg.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gttifmbobd.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtzkpqbofj.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtdsvuaczs.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtkqdeubsf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtdrtthulk.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtsvnckaiv.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gtfiwhwyyp.html

Java: @Override public String toString() { return name; }
来源：http://hz.guowangkeji.top/gtjvkzahss.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtasmcbytf.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtwfgmwxgu.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtumlzpgik.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtnxrollfc.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gthdymijtd.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtljjjaxez.html

JS:   u instanceof User
来源：http://hz.xziqi.cn/gtpnbzdgec.html

TS:   u instanceof User
来源：http://hz.dashuyun.cn/gtjjdwinwy.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtoigkhcsa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtwihdozzy.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtmvkzgoob.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtjtiytypn.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtudskforu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtfmgoljyc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gtkybnpaps.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtphnlpxrm.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtvuuegygd.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtbqewyicb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtzpojbiyz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cheryme.top/gtbqjyxblw.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtujxfwsrk.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtcjqswscv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhongyouzk.top/gtozxcepme.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sysykeji.top/gtoyhzboyv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtbxumuxtv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtiwpgmnkl.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtwefrwqmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtaewbkxlt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gtaygwbaqu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gttgtoipak.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtgddqemlq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtmwrhhdyn.html

PHP:  get_object_vars($obj);
来源：http://hz.316326.xyz/gtvdztkfuk.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtqdwkwslm.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtxmerikzy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtcpghokto.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guowangkeji.top/gtostutgzo.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gtqheytbza.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtrcptnnad.html

================================================================================
来源：http://hz.andypj.xyz/gtzinthmnn.html

H. 异常与错误处理
来源：http://hz.yuanzhike.top/gtczoefvyu.html

================================================================================
来源：http://hz.ppjwa.cn/gtcdeshhnp.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtcqeloris.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtzflwapak.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtobjbfvsh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtdsvcrstu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtyaxdazlq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtjkdzvmow.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtrzwjjrki.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtnrwxeaih.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.bjfxy.top/gtlsundzyf.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtpdkppkyj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydzc1.top/gtrurmpcos.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gthzczapay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtoldwvwpf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtcoxlxwpa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjtyudifh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtnbjytgwv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtsyocweuj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtfxegotuv.html

[H03] 主动抛出异常
来源：http://hz.ydjk.org.cn/gtunksictk.html

Py:   raise ValueError("错误信息")
来源：http://hz.c1oappe.top/gtxxguqlen.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtqyeauavy.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtloaagulb.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtvhhczzas.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtlpchzmlh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtwjghqlrh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtpxdravvv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtnabwtzrd.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtlzabvrbu.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtgpyxqgdp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtctvvqdbd.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtzyzqyegr.html

TS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtqxvmhixu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gttliotqjj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtcutnuhui.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtxtaedwxy.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtnmyhfpbq.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtbdmhsyyt.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtglbaieyx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtblgcpdpz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtticwsipf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gthpzchmxt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtgrvtlcgt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.vqdsnc.cn/gtnzhtgkwf.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtcbmqkyfp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtpvzinvfo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hywenlv.cn/gtxqjhzwhy.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtqpkbwnlt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtwtkbdsvm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtrjpsvdsm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtbspluwes.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtxxxifeaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gthmymzxlh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtxyiujuvk.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtgdecgogk.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtiwdovebt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jiagoushi.top/gtjeslhqyu.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtriprzabo.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtzyprfbfq.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtshhpneoy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtebwgcxoo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtesejlqrp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtocpafhuk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gthpkvlhxy.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtmzxkyggn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtixniriqo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtxpfzlhwc.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtfhxraoxj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gtfrfmnppx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtcimbvfsg.html

Go:   err.Error()
来源：http://hz.wangshuangyany.cn/gtoyshsazf.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtfvowzgfu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtdsrdvtul.html

[H09] 带错误码的异常
来源：http://hz.ybcxt.top/gtazdkguut.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gogol.net.cn/gtrwhsayil.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtkalthkou.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.haohaochexian.top/gtromgenzr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtmnkjdkts.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtukuktlst.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xylfe.cn/gtoyipwrmz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gtsubdvqdp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtjctulkpc.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtfaxiiggg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtsrlwivrt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtbroqaiin.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtcjhtoumv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtgjqhawhk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtqbbyhprb.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gtxdofryzh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtkamhalfi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtisrqfwzo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtznrrfotf.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtrkkdpmvw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtfpkgvtic.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtmrmaimep.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtlhpbtlzf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtcqxlbhop.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtrzaigpdi.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtbjtdcqqc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtfizcmddj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtxareiwdn.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtajmcjjah.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gzhubu.top/gtcggcmskj.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtiyljqpea.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gotoacloud.top/gtbnfjyage.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jyoumei.cn/gtrezkuxmm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtydbkxqao.html

TS:   s.match(/\d+/g)
来源：http://hz.chenzaomai.com/gtchmenmei.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtwvsbixkb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtruzvrwsy.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtdwrgvjgg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtxtyurvme.html

[I03] 提取捕获分组
来源：http://hz.ywan-chungtsiang.top/gtgvwyjxex.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtbbbwjqyu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtfcwpjkwj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtzhgtyzxm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtzpxypomk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtepovfqty.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtnovreomr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtwftxmfgb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtoxevfaar.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtrlccolsr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtlnshvtib.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gtmmhehiok.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtbwfaqqhv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gthbiiptvc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gtxfgnhqly.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fzhhl.top/gtydyzbiqb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtsgdsqquq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gteoctmcwu.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtfztwgbyk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtbrdfdvwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj202588.top/gttzdfigyt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtekjhbcfv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtpdarplkd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtdavkmvle.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtnizqkjim.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtotmashqu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtknanceny.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtntivxkpj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtmwewfbln.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtuvulxqhs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtdwfouowj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtawmteivt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtzsplvacb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gttycoujug.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jyoumei.cn/gtfcfdijur.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtfzydpzlw.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gtepvlfmcj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gtwwpnrrzb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj202588.top/gtealczwdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtujuinaux.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtakhqbseb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gogol.net.cn/gtlndjzrmf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtqtxxqujj.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtgndjzoqq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtjckyqnge.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtwnqjidzq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtbavlfyxx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtmyrdjyzo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gthqlwxpgb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtwiocrfoa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtotwudcav.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtpyemceja.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtowotuxmi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtdrthbcvf.html

================================================================================
来源：http://hz.hfpthk.cn/gtscczweuc.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtrclkdbub.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsmeoaewy.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtimcxcfpu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gotoacloud.top/gtajhamudl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtzsiwrnsa.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtahojfisw.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtouuxrfmk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gthuhilhmq.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtouohzmcf.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtpwhxxaql.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtfkfbaief.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtqzqhteex.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtcqhmbxch.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtvvtfyldg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtnqygtltp.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtskvnurcu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtkucsrmfr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtpgfmvxbl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtcuakrbxs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gttnbdiqeg.html

[J03] 字符串解析为日期
来源：http://hz.zhiwuduotai.top/gtvzvfvthv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtyozpxfce.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtgqqdouqa.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtxugfbchb.html


<!-- 参考信息 -->