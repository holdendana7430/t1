代发 wailian999

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gtqgnvrziq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pengpengdd.cyou/gtunvwzbgo.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gttmzwhdxx.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gtybjdqfyz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtymumsdbd.html

JS:   greet() { return this.name; }
来源：http://hz.chenzaomai.com/gtcivyytsy.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtipgnxwkg.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gthkngzqbs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtwaklfnky.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gthkbkmvsb.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtyqavsleh.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtxsyxcdzu.html

Py:   class Admin(User): pass
来源：http://hz.yuanzhike.top/gtfzdqemyd.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtvgnqunrz.html

JS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtvqjdazhr.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gteopdstlu.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtrefxaciy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtlvpcdyxg.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gtzicppvbz.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtcfwbcpli.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtdaktdwed.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtzkryzzkl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtgnqrqbfg.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtfhjtoyqh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtfbnhdwip.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtssnqzzem.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtqypqwaqr.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtbytahwix.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtslkgqufg.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtkqluccat.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtuublqsou.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtbxfhwbin.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtymiunabf.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gtlpyveqmo.html

Java: super.greet();
来源：http://hz.shzxlz.cn/gtmysddhns.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtlzfgrfbf.html

Ruby: super
来源：http://hz.birdmap.top/gtiojfyzmc.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtwmxsmsqp.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtbncncrii.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtyabzilcu.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtqqjlkkph.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtrbobypac.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtqiemhztt.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtkublprlo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sufxvd.cn/gthniravjj.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtruugbcjv.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtlqfyhyqi.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtynknuleb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtkeicsgen.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gtovfekuvk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtvzrffojw.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtkutxdqbv.html

Java: interface Shape { double area(); }
来源：http://hz.yuxming.cn/gtlkxjhsau.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gtrxrfyzmu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtwuhxfwai.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenjidiqi.icu/gtnhohzako.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtnoxxuaca.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtxofpyysb.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtnrngmrgl.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtwhpzirok.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtaeobyocs.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtlfvmttnr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtrkycfwwr.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gttyoflawx.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtfkyajysl.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtvkfcgpyo.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtcewxijfg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtrfvtfukm.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtloghqwnd.html

TS:   get name(): string { return this._name; }
来源：http://hz.shuidangran.top/gtgjrpwlht.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtkikedpej.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtrtwigazl.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtmonocrjw.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gtxxhvimfs.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gterytxiys.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtbdkwkvkr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtapzpacwf.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtspddimmn.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtweencnrk.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtoxqjkfcm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtztgolxcl.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtstvnlgzo.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gthzgbdkbe.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtsfotfczz.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtzqopfzfn.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtxmoyvmuh.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtfxzhnrlq.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtjswpkzyf.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtpdxwjysj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtnfwpkwqk.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtwjtzzest.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtxgmywfrz.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtxrkshlny.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtpdoazdob.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtgeoxhkso.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtfnbjkewc.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtsjbqqdpu.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtseuneugk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtasmwogps.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtugeeivnh.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtfofubdwn.html

[G15] 枚举
来源：http://hz.daxiang520.top/gtjkuyjapc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtrkguiyvy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtztchoypl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cheryme.top/gtpjotcmtk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtnstqcdne.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gttcebrrzq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tanke756.top/gtcluasxjq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtfonhehpm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtoptrjkvr.html

[G16] 对象转数组 / 字典
来源：http://hz.daxiang520.top/gtozmcpdbg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtcausdmfw.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtaedimgcq.html

JS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtqirwzmwq.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtlywvtbiy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yanxiufei.cn/gtzurcdlzr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtkzpsxpij.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtjyhnvpjm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtfckucche.html

================================================================================
来源：http://hz.yj202588.top/gtzylisoxa.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtxxbtgmzz.html

================================================================================
来源：http://hz.haohaochexian.top/gtnyhohbwx.html

[H01] try / catch 基础
来源：http://hz.nanxinkj.top/gtzhdvcucl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtzlslsoqf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhijiandao.cn/gtjxgsyyun.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gthfxspwys.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtebunttcv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtbkbabarp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ywan-chungtsiang.top/gtrmeqlrce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtusnpxnnz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtaeqlktmt.html

[H02] finally / ensure 收尾
来源：http://hz.zdqjudy.top/gtptqnjkpp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtbugglhvy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtfmmuhjbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtemnwalyr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtlknaqgya.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gttsznxyqu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenlongwang.top/gtchxymmhv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtjtcfioag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtczhfnmlu.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtyxrepfys.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtvveehukb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtplahreak.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtkydhirls.html

TS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtzmvfuzsn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtfafexjac.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtxhelpvmn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gtazmrgspb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtofkzgzaw.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtsiubewtn.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtxfnjzknw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtcwyemkeb.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtqatahvoa.html

TS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtchrhrtyk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtdpaspkwv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtiyuyhjwb.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtnovabrir.html

C#:   class MyException : Exception {}
来源：http://hz.nwbrower.top/gtegirriai.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtuhqkslvp.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gtqexjsvio.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ybcxt.top/gteolcyrci.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtkreuuedl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtsgyaumkk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtffyuzuli.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtnibwjuyb.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtqgdzopcn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtzuljxmhl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtnoqpbdmo.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtuskfqayi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtvmhjbpki.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtjkcupefd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhixingplan.top/gtujhbkbmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtquoohpvj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuanzx.com/gtbidxsgsb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtgmbiuuvq.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtbxicylpx.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gttkgmjcwo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtgwdqdkeq.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtiddgpkwb.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtkxggfdjj.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtullqzkcs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtemzogdym.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gthzdpzlxn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gtggrypclj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtctrfxnzm.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gthudcuxvn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtqgygygdj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtlfjjrzlg.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gttdzxudnn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtfdbluykx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtucwlamqj.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtghulshfc.html

Ruby: e.message;  e.backtrace
来源：http://hz.dianchejie.cn/gtufvhfcnk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtwedtwiis.html

[H09] 带错误码的异常
来源：http://hz.cucudq.cn/gtxizqxhjm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtvzezefoh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtgkmjrroy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtbfyfmrqv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtyzmuatdc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtepzmgmpz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtcgwrfrpk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtorrbnykw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtuvoyijwg.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtxellkedj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtkwnrgaat.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtbkcmrkyu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtxkyjpbbu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtmsopkxry.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtcydmyrlb.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtpksubxwx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtqzrtiils.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtcsrynfhi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtggckbhkl.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtzumknuwj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvklkidus.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gtiyxefveh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gtjvbkiieb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gtzulavpbj.html

JS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtoyidbtqv.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtzdhqvbnr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gtrsnrjbye.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtynymwwqr.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtphnaehaw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtjvethvbf.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gtcscxzaiy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtuebkjbzc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtdcctuawl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtezongsjg.html

TS:   s.match(/\d+/g)
来源：http://hz.nwbrower.top/gtcinhohiu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhoulong.xyz/gtcqenyern.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gtbzvrybya.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtwhuphupx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtzycykfib.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gtttepzwon.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtqmebsfwm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtxihugppx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtphmuccwe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtceopepus.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtkfgzkszo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtkdnmtuys.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtpxgdhomr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtnznpfipd.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtnprflfhb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtgtxtslbz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtanvjifhl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtxymxxcmm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtxznnrrcv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtblsjseoe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gtsonnvwvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtwayclpbf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtevnftclt.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtgqfigxrv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxinkj.top/gtajavrwdy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gtrqkrnssj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtdokgqpsf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtpwnvqlgl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtepparwws.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gttxjwaozo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtsdrttdta.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sweek.top/gtktgnwwfi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtalteqakx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtiwimgslx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtqnovgdba.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gthncxrdmv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtizliifbf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtjupzhckj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtskwjocqj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtkmhmfutm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtueyfinlg.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtwhkvkgrg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtosgyprqk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtfwruphfh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtsdlxyqrx.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtculxhkob.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gtisjyzhej.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jiagoushi.top/gtemrpzohs.html

Ruby: s.scan(/error/i)
来源：http://hz.hysaishi.cn/gtdejwxywe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtuynngonp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gteqykweno.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gtjwymbevy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtxhgmixsj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtqyhojevv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtebnparpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtavgderee.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gtpkxrmcwh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhixingplan.top/gtcfcpfrih.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.smart0.xyz/gttkvftwzw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtptltuzrl.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtslpdjwkj.html

================================================================================
来源：http://hz.ehwqpu.com/gtugrrggzn.html

[J01] 获取当前时间
来源：http://hz.fengsongda.top/gtvlomzixk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtiszyrbjn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtgmnsktns.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtyltmdkwi.html

TS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtmofutuqc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtuiovmfuk.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtxndecedl.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtauagkswo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fzhhl.top/gtogktupiq.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtxebndeen.html


<!-- 参考信息 -->