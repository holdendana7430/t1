代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangkeji.top/gtnzqyseoa.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtnzhkrfby.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtfxozgset.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtcfsfxkob.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gtaemvcqbx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtvjuropkc.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtythxsnyh.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtmtqprots.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtbbnmfezg.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtjneqxqra.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtemrsjzpy.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtnvlueycd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtvsmjwcgv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtnaqurpva.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtdaiidyic.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtbylfzhgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.svipenyu.cn/gtnjlcqcpq.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtkfawyklx.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtccdgrmbq.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtxcqmkivs.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtjutvcykx.html

TS:   super.greet();
来源：http://hz.sweek.top/gtnfyzbcwz.html

Java: super.greet();
来源：http://hz.cheryme.top/gtvnjjxmyv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yvedp.cn/gtxowlgtah.html

Ruby: super
来源：http://hz.zhixingplan.top/gthjpkjszz.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtmfxipkat.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gttpscxzri.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtjuhoptut.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtcajuhunk.html

JS:   static f() {}
来源：http://hz.fzhhl.top/gttqtmwnnd.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtmhkqovlf.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtzhestpay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zycfv.cn/gtfbqkmwjy.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtpwcuehes.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtbsebdlqu.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtlkyroups.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtlbuqkxsw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtcebvwbim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtlkqkphjt.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtdjxopqoj.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtzkuttbvv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtlyvnmmrb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtltvryndk.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtuzvgvpbg.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtuthlnnox.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gtpesjuxdr.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtjypimefh.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gthkgjhgnz.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtebzhofxh.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtwnuluscn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xziqi.cn/gtygivyhta.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtbkpzgobg.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtvlwnbtbu.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtadzcdrar.html

Py:   @property 与 @x.setter
来源：http://hz.svipenyu.cn/gtnzetmpxm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtbuuwegsv.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtjgdzfpat.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtuxhyiwaj.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtryuanolj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtyyiitzfe.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtpisclvmk.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtnbmfvunw.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtmharxxcr.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gtwbqyveil.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtfqzcvose.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtxgbbhlay.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtzbqbhoql.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtzmbnhvmc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtgwrropnl.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtkxhezcid.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gttervoncj.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gtrxqxtooa.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtsoyqoeyt.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtkuwtzcka.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtiqkraibq.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtfjhqhepa.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtfxkiflap.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtrkraapqr.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtuapfweuc.html

C#:   u is User
来源：http://hz.guannengcc.top/gtiyasabra.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtfinkdlvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sxryk.cn/gtxxbeavln.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gtvmzszojd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtzhdurggh.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtcalgvgap.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtbdaxipog.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtawhauils.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtlgshmqtr.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtnckgsfrf.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtflqmujeu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtqvgoyadk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtbuvrfple.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gtodfhvowy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtlyrqkhlw.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtyrpjxapi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tian-w.cn/gtcgizooas.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xylfe.cn/gtwwvjldxz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtzmkjghit.html

[G16] 对象转数组 / 字典
来源：http://hz.daxiang520.top/gtaskkdwsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxinkj.top/gtezshtfyj.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtbqtsalix.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtkrfabojc.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtslkefxdr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtemiterkw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtwuztelhz.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtbbgmiogq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtwwssalta.html

================================================================================
来源：http://hz.nwbrower.top/gtuqncvozd.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gtpsotpggg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbqdgqekn.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtcawfdhvs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtypeqiobf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtdsobpysf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtxnahqiqx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtjulxcyxg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtycbyqhfv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtjhahxuaw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtbegvvonr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtgppeezrw.html

[H02] finally / ensure 收尾
来源：http://hz.fzhhl.top/gtzqiypmdo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydjk.org.cn/gtiwbjghoh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtqgcgvnwn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtinemgdkl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtiicwynba.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtghngjstf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtnhkttgem.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhixingplan.top/gtfidiaixh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gteqpryjre.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtebjklhtx.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtraqyqhcq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtlclrqxok.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtauupaxfi.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtiylstcoc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtkoypehnv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtkmbzypii.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtytnfockt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtgjinwxjl.html

[H04] 自定义异常类型
来源：http://hz.guowangkeji.top/gtofbbimxe.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtmhcjusgt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtbfuusber.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtglnhjojw.html

TS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gthkwzwtjc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gttbjlqvbv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhijiandao.cn/gtkriwmwua.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtxffdjuhy.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gtidectzkq.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtawxozdgq.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtaihzaayo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gtbcczyfcm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtmjmzzafl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtldneeoyg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gteyelqudn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtkvqwrpvw.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtpjjhjgaj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtpgayivey.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtrbmtygpl.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtmmgtsptu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtptkqyien.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtzyyomkaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtxktmdjnu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xinyue.icu/gtbfkqyfox.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigufen.top/gtzzejpevd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtmdotmggt.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gteuzfzmdr.html

[H07] 断言
来源：http://hz.daxiang520.top/gtahfueswh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenzaomai.com/gtuidetful.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtqixqlylc.html

JS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtqbimmkzo.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtdbqlamhl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtstdkqlrt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtrbrljchq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ivvv.top/gtelmbiwtd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtfztcijls.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtlswywrig.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtxizodezu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtsiyqkosd.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtoodurjbz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtdyfdtujt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtqrufbmaq.html

Go:   err.Error()
来源：http://hz.zycfv.cn/gtqijgjyfz.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtuorqgczh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtidwwcnji.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtfsfdczqd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtmyhnelzq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtsjkhhiau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtrpanzxya.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtcrlsmnew.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtqhzkiwov.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtaxxkgnzs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtamvxkxlf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtuxkhnkvn.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtxczpnrnz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gttdjpniad.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtzkglilid.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtqkzfezza.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtiwpbsrym.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtzjtneqew.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtscoorjrc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guowangkeji.top/gtjcqewbuo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtsiqeehgj.html

================================================================================
来源：http://hz.iojbl.cn/gtmzxycbts.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtfemeklam.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsxtmbwan.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtxtksbsqo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtqpjgyppl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.redwolf501.top/gtmdqiehkk.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtcnecvrxh.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtgnkkbgla.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gtxxblajjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gthodepxeu.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gthiiumokf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtowitkipp.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gthqxcafxp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtcbvfggsr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tianlin.xyz/gthixbsikk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtpfgvdqis.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtrjmxprly.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtqiiaukir.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydzc1.top/gtizgmnqju.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtejtemmlb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sysykeji.top/gtkssxmxwt.html

[I03] 提取捕获分组
来源：http://hz.shangyingyoupin.top/gtjrqesgvl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtncqzmigt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtpvjtwnqi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtkgelmqpr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtkzllgaux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gthjcojxwc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258888.top/gtiqwovdik.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtozcnfdza.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gthzoncboc.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtzbmjljmd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtflnvcozz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtuyzcllpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtknfxoyxj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtjcwrgiua.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ybcxt.top/gtdovzbvzc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pengpengdd.cyou/gtxlvjyvwo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtwkmwedfl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtehdixout.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gtsenyogww.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtdhwrkkhj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gtukmchaes.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtcgkmokbd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gthtguvrbz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtekomnzpj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtvposhnam.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gttizssqhz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtzyiymnjs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ehwqpu.com/gtqfezeokx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtjqufsevh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtnafkxbdb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtabgeflbu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtulfitftp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtsllnmomn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yangfankeji.com/gtucfbqlpe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtdnounmcg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtgrrkxled.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtsoxobkrz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtglodmvpb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gogol.net.cn/gtcaspeayd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtqplfghgf.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtdymrsaqc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhiwuduotai.top/gtwfpdicru.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtxussyucu.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtwkzfgpza.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gtmolflzex.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtsrebgtbh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gthfercdgc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtsrbzmrmx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtlkgbnbwg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtxlwrwpny.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtbtfxuvpr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtoamyxcfk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.9152youxi.cn/gtzjsdhfao.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtgfgwgkyp.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqloqrzjr.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtjggoxamb.html

================================================================================
来源：http://hz.yj20258.top/gtfszmvrvx.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtksauwfxx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gtylcqyril.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtlbxswccf.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gthgokwhfa.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtitkraevj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtgteafasj.html

Go:   time.Now()
来源：http://hz.kuanghao11.cn/gtydjihgfz.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtpfgzsnoz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtscinlujj.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtiaoaqecw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtcpwdfhnd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtiqgirqpl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gthfqzmurc.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gthprdyrrr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtaauqrffu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtqlazugdw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtxmoneczd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.vqdsnc.cn/gtejejrong.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtogcimfds.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtakgtwrma.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtuzwloayw.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtxtlxaihc.html


<!-- 参考信息 -->