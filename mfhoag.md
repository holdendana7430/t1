代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtlkfmvcvm.html

[G07] 调用父类方法
来源：http://hz.cashguo.top/gtnchsbuzm.html

Py:   super().greet()
来源：http://hz.tianlin.xyz/gthogpwuej.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtnzaktrlb.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtfvkvsmvh.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtmfyntreg.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtznzxwgzk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtioxsjebd.html

Ruby: super
来源：http://hz.aibaodan.cn/gtjxeedztd.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gttazplowe.html

[G08] 静态方法与属性
来源：http://hz.pycfn.com/gtpnlexatk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtfuuqfnml.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtdskbzjdb.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtsmgcoylu.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtzhlctxdr.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtzvyapdtg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuanzx.com/gtpbeihadl.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtdtnkhfoe.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtqneggydt.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtthjscxbf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtazjkmflc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gthscandjz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtdyfvhymk.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtnrxtclxp.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtdvqbmard.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxuanxn.top/gtnldgbces.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtxwbineqt.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtivgmefbf.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtqveivfxn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtzdgbmobf.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtnpodoxfh.html

JS:   #private 字段；其余公开
来源：http://hz.ybcxt.top/gthutzyarz.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtdmylfpak.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigufen.top/gttendeusq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gtxlcooxqx.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtvbxrvwum.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtbgzndeya.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtdslnalux.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtfindyxos.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtnzagqcyy.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtqdzbslnt.html

TS:   get name(): string { return this._name; }
来源：http://hz.hfpthk.cn/gtlgiryzku.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtrzgriomk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtomcccwlx.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtyerpikoy.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtytwwtlyt.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtvyhmmwrw.html

Py:   def __str__(self): return self.name
来源：http://hz.haohaochexian.top/gtfsqvdhgl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtgzmfgpyj.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtdxxodjor.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtdonsxrco.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtijysrvzf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtclzssopp.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtfnuxldjr.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtxyhmznjv.html

[G13] 判断对象类型
来源：http://hz.yj20258888.top/gtyjibpijq.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtcfjhixxy.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtlsezxymq.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtzsuhyafn.html

TS:   u instanceof User
来源：http://hz.shuidangran.top/gtsyzbhfed.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gthmpnitrk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jlsjyb.cn/gtcxuttzia.html

Ruby: u.is_a?(User)
来源：http://hz.fzhhl.top/gtkoavlkng.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtavdglmpg.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtwyyugemz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nwbrower.top/gtnevqopqj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xingfuxueyuan.xyz/gtymldrgnb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtjciolpoc.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtrdhjhiim.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtfonwpnqd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtxumgjidt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtyslwxhhe.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtpnovsmnn.html

[G15] 枚举
来源：http://hz.ivvv.top/gtbrflkihq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtxjtfoacj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtrbgwkatv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtyybawvdu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtgfelanpd.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gttxptxxuq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258888.top/gtgazvtjwq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gzhubu.top/gtuatdgljz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtporclznw.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtrlqgcbmj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtalaahjts.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtahlnragf.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtjfriwsdb.html

TS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtvkwuttkv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gteqblwooy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtkckqywgs.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtbtruqami.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnqzz.top/gtfnwjemic.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtehoepmzk.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtvdxugqht.html

================================================================================
来源：http://hz.zdqjudy.top/gtvdbwqvgl.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtjpwjqjjh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sweek.top/gtijgbrpmc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtunqgmeiz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtxpxlqzta.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtnyyrdglg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtthbnfome.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtrxknkhch.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenzaomai.com/gtilifdrup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gtbpuvxrnx.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtglleoinx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtkyfnquic.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtuxxmluvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtnzsrfndd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtfhjezjzr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtemaunyzy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ybcxt.top/gtjjazmsxz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtqjyszqvp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gtlruxixcf.html

[H03] 主动抛出异常
来源：http://hz.hnxiangtu.top/gtjqzvuyvj.html

Py:   raise ValueError("错误信息")
来源：http://hz.fzhhl.top/gtdqctooeq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtbvjewmug.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtysjtbbtq.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtsczekgqd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtwmuepawc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtdngsbrhz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtwdbcyept.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtubwrzqax.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gthpzkwgte.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtmpdpymqv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtfdqtntdt.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtgctfnnht.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gthzsunagd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtpbkrodhp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtmguqpwhe.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtxpuvexek.html

C#:   class MyException : Exception {}
来源：http://hz.cucudq.cn/gtxobczkcl.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtkkpvuucb.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtsxnbmnui.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtpmorvipc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtsguhidvy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtsaepciqh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtljlixbkm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtgdsdhxwg.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtdxzzlfmv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtxcopdsem.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtpazwqvqw.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gttidiargq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtgqsmgefv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtaugolkvf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtysrocycw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gtxgopjpjy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtkpeznliw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gttnarqxzv.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtmeniykto.html

[H07] 断言
来源：http://hz.zhaomingkeji.xyz/gthgglywro.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtbtgowjya.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtinkbttph.html

JS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gtjedwdqse.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtvisqlrix.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gttzaurzah.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtlbdabmqk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtriqcnxds.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gthruzrjdx.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtvgnradsg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtcmuxkkcw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtphngvtke.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtfuafcsve.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dashuyun.cn/gtfzawndde.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zycfv.cn/gtrcowhpxs.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtiabexlsz.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtwmmalyux.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtiwklvmbv.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtkzdchkep.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtgcxrvmbj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtlqrxodor.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtwvvqcxtf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtmfngcznx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtxdqluhzx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtywfmbfay.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtsobsvkqp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.9152youxi.cn/gtdbilhirv.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtefvuytlb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtwcjnbtfk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtilyegwtb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtdpmdsyqc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtomstpyvc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtbbwkldmj.html

Go:   defer f.Close()
来源：http://hz.jinyuanbaomall.cn/gtasjpygog.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtjcijqflj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtppanbfvl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gttlsgxwzg.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtuclfjgia.html

================================================================================
来源：http://hz.yueranfly.top/gtqirfsius.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtyzpiauld.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtrvpoocvu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gttavtgyfh.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtniovqett.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtjmrzbgcb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtiunekkkg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gtieampnta.html

Ruby: s.match?(/\d+/)
来源：http://hz.c1oappe.top/gtxhltfzty.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtzprzilto.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtrlkpnthy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtdttlrexl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.kuanghao11.cn/gtdtanlmyn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sysykeji.top/gtxtgwbzvk.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtrueevgal.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gtlnwcyxfh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydzc1.top/gtfogltavp.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtndojvcqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtjrktphhn.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtbvcxbobt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtpodmliqd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daxiang520.top/gtyxhtggze.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gtlhzgdmuu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtyetyzwlc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.redwolf501.top/gtamvsgyhr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtkoozfyol.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jiagoushi.top/gtfyvanpfz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtbbeksint.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtgpjlvbpc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtfahobjfl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtpsgocysw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtkfhugvoc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtdrcufwhg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gtfsepfscd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtixjmijid.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.52xcode.cn/gtwwaoqddf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtpxshrjlu.html

[I05] 按正则拆分
来源：http://hz.cheryme.top/gtiosuqcjr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtrzaulrns.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.52xcode.cn/gtkdbclugb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtllxumrmc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtqezynyqk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtihywnjzs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtwyhxzpkb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtmfkveeib.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtzscertts.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gtfdjgsbjy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtbpfohmbx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.bjfxy.top/gtruboadug.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtqypnrbom.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtcffwonwd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtioxkddsv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tianlin.xyz/gtmjmjyfzk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gtvwxqrkil.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtvqlccror.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtmxvpuhmv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gtxgchtqbj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sysykeji.top/gtasuuylfn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gttiwkcnjl.html

TS:   /error/gim
来源：http://hz.shanyushiyangkeji.top/gtioogooch.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtoaxwigua.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yvedp.cn/gtqcsfmmip.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gtmipqwvrt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtecqbvqgo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtxlkdzchr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtyekdtzvp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gtkmpzfacv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtkqrewcti.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtnqmldzbw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtamnarbay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtnahpcuew.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtmnmbqcwh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tian-w.cn/gtpqinxjmq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtitkwhrwf.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtzxgebvgf.html

================================================================================
来源：http://hz.cashguo.top/gtncfhgomw.html

[J01] 获取当前时间
来源：http://hz.svipenyu.cn/gttrvjjsut.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtachpaith.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtcvdeqnyk.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtnyzghzpj.html

TS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtqsetbmsi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtkegblhmk.html

Go:   time.Now()
来源：http://hz.cucudq.cn/gttdbauvap.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtctgmcizs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtiiawqhyv.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtfotcfbow.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtewoalket.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtmqviqlfy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtwcesdkzg.html

TS:   d.toISOString()
来源：http://hz.zhengqikj.top/gtxqcntuwz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gttfmhpdlm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtagjjvvrb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtedmcupuv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.vqdsnc.cn/gtaauawpse.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtasiolaor.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtfcwxzlnt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtiwmxxmrk.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtkvneqqmc.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtejfpcotg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtrqopfskn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtglxyvtpd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gttllhpgxb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtuarkuhik.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtjqmihsjc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtykkheydv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtdmjyhdyt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cheryme.top/gtlqekuxyh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtzpefhjov.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtsqudpuod.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hywenlv.cn/gtwpgkwsnw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtvxcqpjfi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxuanxn.top/gtoxttpcan.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtuchptciw.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtjqvzlpvg.html


<!-- 参考信息 -->