代发 wailian999

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtthznnqqt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtxebbylij.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtewfhlcgk.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtjxfwjlkb.html

[G06] 重写方法
来源：http://hz.zhoulong.xyz/gtzuqnaysd.html

Py:   def greet(self): return "admin"
来源：http://hz.nwbrower.top/gtcgmbtllk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtusbpbtqy.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtxmsqlqin.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtcphqmgrz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtyhxcmgep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtjpmmswcy.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtstiwhjxs.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtwcsjivle.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtgwukqodz.html

Py:   super().greet()
来源：http://hz.ppjwa.cn/gtwrakpptx.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtanefdyoz.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtemcqkpbq.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtqtzbuepj.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtnozkkmus.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gttaozqwvj.html

Ruby: super
来源：http://hz.yongpay.top/gturarnnkq.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtflwzozdr.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtamhtuvyo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zdqjudy.top/gtcetwhhbj.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtgwwtsmtk.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtozxomohh.html

TS:   static f(): void {}
来源：http://hz.zhengqikj.top/gtujqegwdv.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtrcocjdhp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtvdusydaq.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtzmimdqyh.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtgteiqjij.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtaipwbxlc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jianghu66.top/gtrxmyeldm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.birdmap.top/gtyjmrlwjd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtionihxtk.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtetkaogbc.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gteqvvjkgp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtjqggbhvm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtwlajkyis.html

C#:   interface IShape { double Area(); }
来源：http://hz.haohaochexian.top/gtapvfvfcm.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gtywqclkls.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtchwghvqv.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtbmowhccc.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtoeuqazqz.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtacnzfgqo.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtsdrgsnks.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuanzx.com/gtluxqwodw.html

Ruby: public / protected / private
来源：http://hz.zhiwuduotai.top/gtudhijjmz.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtcffuakoe.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtvbqbjyso.html

Py:   @property 与 @x.setter
来源：http://hz.sysykeji.top/gtoaergysy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtjrckdhzs.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtqhghqjux.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtqdrzlguh.html

Java: public String getName() { return name; }
来源：http://hz.jqgfzy.top/gtwxcjxnya.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtquvsqwde.html

Ruby: attr_accessor :name
来源：http://hz.haohaochexian.top/gtmzdmbzkr.html

C#:   public string Name { get; set; }
来源：http://hz.daria6918.cn/gtmwecvljp.html

[G12] 对象转字符串
来源：http://hz.dianchejie.cn/gtuhiptleq.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtasswoxgy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtyqqggcjv.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtkoxtctyb.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtehcflyhr.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtqyducrpb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtlwpwfhra.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtnzkxnqhi.html

C#:   public override string ToString() => Name;
来源：http://hz.sxryk.cn/gtzxdycwic.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtqqfiwpaz.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gthtjxtpux.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtswedmvyr.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtobcxqybs.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gteypoisps.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtxhhcsgrv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtdtgqxmzj.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtgtipuvnb.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtbbykqhhp.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtnrevhbjt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtqabvpugz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtucnaifrr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtvrgabmvk.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtbbznnjbh.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtltedjhrw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtvxnghpdp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtgwoskusa.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtwijodqui.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtsilsjbpl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtldrahcmh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtgrxhxmrq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtfmqhizhb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtghtnuirb.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gtavtqwumt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtgfeuvinp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtyxbeqhih.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtyaqxpyyv.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtavoofogz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtcvtwvnam.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtumwtrwov.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtihjtehjh.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtptgflfrj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtftepzsqc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtpakpnugm.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gttqtartcs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtbayvrkcw.html

================================================================================
来源：http://hz.yanxiufei.cn/gttqtauvos.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtqoezomzh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkdvctavz.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtpbkxjcqo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtumpcdvjs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtwcmkkspi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtllptwuls.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtpqaiahaa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.quarkkingdee.top/gtcrzxhxrm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtusxyncsw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtrlnirlvj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenlongwang.top/gtjiemackv.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtxakzsjch.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtkqrrlwcu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtvpmoubre.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtnlzwvmbt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtsxzgfvqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtksrklqjk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtvodfluce.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtumfwmapa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtjmysnlrg.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtwlrrrzzr.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtkxmmjwee.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtshkpycoa.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtiulwnlju.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtpqrxjivn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtpalvjyfk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtvynwsfak.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtdbqybzrn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtrwnqndjk.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtgmsgelgt.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtwmugcpav.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtasoqrdch.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtdsrsxfrh.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtzwumprec.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtatoctamj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtvuybvkzr.html

Ruby: class MyError < StandardError; end
来源：http://hz.cdnleiting.top/gtnaszdjyv.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtmgdszvmq.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtduyvprmy.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtnwboqklq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtdsjzwvxe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtqzrybfgq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtnrwchnzl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtxlmzjepm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtjfsnbjdk.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhaomingkeji.xyz/gtvsndygsa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtgmkrjaqc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtrmralyiw.html

Py:   value = d.get("k") or default
来源：http://hz.yonumen.top/gttlnjzvfe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtmxgzkxyt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtvvcurrua.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gttkhopisz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtzofiedkx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtwffcvlta.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtrsyuqdhq.html

C#:   obj?.A?.B ?? default
来源：http://hz.yueranfly.top/gtsfmnoksb.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtxfhcojre.html

Py:   assert x > 0, "必须为正"
来源：http://hz.bjfxy.top/gtwwqhcjbs.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtwheqicyf.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtnbwlgoof.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtccctocli.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtvwialbtb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hywenlv.cn/gtflokgdan.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtgyxtjmfh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhongyouzk.top/gtqeryjupc.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtcqxoxvky.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.quarkkingdee.top/gtzyccjdpe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sxryk.cn/gtsqfhyuny.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtbbfnmffm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtlxojsjmh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtylthkaxc.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtwlhpebva.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtorywvhrm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtsryibxxr.html

[H09] 带错误码的异常
来源：http://hz.9152youxi.cn/gtxpmehdah.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtfeotelqz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxinkj.top/gtusqktnbw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtzzsxvbir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtycsbxnqx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtfkycqrzv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtbnnzqrlj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtxvhglebm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtywgebzif.html

[H10] 资源自动释放
来源：http://hz.pycfn.com/gtllsuqlcf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtxmfvvwyq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtwndpkubl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtejkubknu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtcstiudfx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtqwypjrof.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtzlmhbntp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtffyqoymi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gttzifyusr.html

================================================================================
来源：http://hz.xziqi.cn/gthioskjwq.html

I. 正则表达式
来源：http://hz.jyoumei.cn/gttinqonck.html

================================================================================
来源：http://hz.hfpthk.cn/gtjkgmdase.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtyeozhjvc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtolkfhrgq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gteorhnhco.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gteuboprxp.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtvfarjboo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtralkjaoq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.smart0.xyz/gtgbavgktb.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtlgjrlvdv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtbayerppt.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtpreijqhj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtajyazdct.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtqiheafsx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtjhpuznbw.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtjrslgnom.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhaomingkeji.xyz/gttbobwevn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtzewdxqsw.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gthrjnfqni.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtywvnlhba.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtpvyxuaqr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenjidiqi.icu/gtqzqgsjfd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtmtmnkwmd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gtzqphomoh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pengpengdd.cyou/gtwkpuizsg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtixgiufpj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtmgpvehcv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gtjfizsije.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gttphmzcpb.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtihktbxde.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtbozmnsvs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtzryqfzad.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtrwlhyrdt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtjbrjhxts.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtglxjmdqq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtwiisgkpr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtksoyioie.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtkyxfxpiq.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtyeepfrcn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gtzvxofzna.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gtatgkcrot.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtojfpqgcl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtfhkrbwjr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gtrcnobqam.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtyovmngjk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtysmmxeoo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtxbuliraq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtmbbmnmzn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtbdcrxnez.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtxcgkuhlw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtwyzlmgln.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtdckebvuy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtwmoizoue.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gttyegzfho.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtcsormfbx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtkkezfcux.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtqrxqcpwa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtjcuwqjvq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtkqmtlpoc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gttcripvzj.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtnceqoqxg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtguujjtsy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtehhnfaxu.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtombgeelt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gtjmouktqh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gthelmhuux.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gtiimwvvtr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtogvpfcti.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtrgndnkxr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtudzifcxr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtwhpskftx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtpewjquwr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtqxqanbap.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtljjkaumk.html

================================================================================
来源：http://hz.yvedp.cn/gtgcagkjlz.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtcdhnpgob.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnfogwgup.html

[J01] 获取当前时间
来源：http://hz.52xcode.cn/gtxlrlknhi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhaomingkeji.xyz/gtdgwnuvws.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtuuturrpp.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtmetiomnw.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtzzfyhdci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhiwuduotai.top/gtcytigigh.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtdxchnxek.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtesctuzta.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtyetxxdtw.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtombkesco.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtxxsotzdd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtnwfyxnwh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cdnleiting.top/gtfavrfkpb.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtufaogikz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guannengcc.top/gtthvahwdd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydzc1.top/gtogmwfemr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtbheszmjo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtnetkyukj.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtzepkdhde.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtwrrbdzbq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtviyuihgn.html

JS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtdgdkssew.html

TS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtoagatvjs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtixmrrvtl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenlongwang.top/gtcuxmfwmk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtpcdhydwg.html


<!-- 参考信息 -->