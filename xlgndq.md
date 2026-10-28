代发 wailian999

[G06] 重写方法
来源：http://hz.316326.xyz/gtbspuaruj.html

Py:   def greet(self): return "admin"
来源：http://hz.xylfe.cn/gtijianieu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtkvnfkwct.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtemasrnai.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtuzgvdcse.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtaxuclibq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gtxdxuojba.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtvzhoycqa.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtbbvfxjne.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtokrtgwpv.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtjqabodgj.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtgugsunco.html

JS:   super.greet();
来源：http://hz.yonumen.top/gthzuqshhl.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtfqkmillj.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtmyyatgyg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hammf.cn/gtwrecudvh.html

Ruby: super
来源：http://hz.pycfn.com/gtjsmwspcf.html

C#:   base.Greet();
来源：http://hz.yangfankeji.com/gtvjxdvaks.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtznuymhby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gttvjpxdaf.html

PHP:  public static function f() {}
来源：http://hz.yuxming.cn/gtjdlgvzkv.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtrccqhyah.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtykpidoft.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtozbqkwva.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtamwgbsyu.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gtlvcxjkmw.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtsvkuptud.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtctwhvwkv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ybcxt.top/gtrxfsjpuo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtvpldptjr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtjoelerbb.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtqsoxmzbd.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtxvyihvfu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtlfjxfbum.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtzkdniuhq.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gthxypmldl.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtulyyvwxk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtsnjqjcsd.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtictymklt.html

JS:   #private 字段；其余公开
来源：http://hz.chenjidiqi.icu/gtatpjbxwp.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtaphccoyr.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtjmswtukh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtowmsymoz.html

Ruby: public / protected / private
来源：http://hz.ppjwa.cn/gtpvgzqpqz.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtdrygcaxv.html

[G11] getter / setter
来源：http://hz.yj202588.top/gticwmafom.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtwajxaplj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtjvektuiw.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtnjbbsthq.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtxiivdijy.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtpfqtmztd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gthlsqgjpb.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtwbyaeirh.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gthcfzanlx.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gttwxkkujp.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtnmhbeldv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtslodounx.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtxygqdsxn.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtpudtwdjo.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gttievczkd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtezgyyyxv.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtywmkzqkg.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtrluftrrz.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gtbgtsoaiz.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtauppukwx.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtpmepvhvj.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtpmxjbqwz.html

TS:   u instanceof User
来源：http://hz.shuidangran.top/gtwvonxixp.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtaumhqmes.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gttcmrunjd.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtsvaseohk.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtlnbrnkcz.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtxkewnelh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtzvgwcwlv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtzmobnhxn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gtqvrexvti.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtuplwxppk.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtwqcmmyqx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtbjuprxxc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gthyljvywu.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtneuhrlcw.html

[G15] 枚举
来源：http://hz.fzhhl.top/gttsbffzvl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gtmehilzos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtjxcutrhz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gttgkjrnah.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtnnhuxfwc.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtccvjymwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtmnyqdddl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtsqlkbmwe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtfbpkhxrx.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtdnnigmbn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtgsesocfb.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtuebsodke.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtqoxgbffn.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtcouyryas.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jyoumei.cn/gtyyvpdjjx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtygfzvpti.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtdwghmdbm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtrvkcnrzm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjrkfdvne.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtzlrsuxgy.html

================================================================================
来源：http://hz.yangfankeji.com/gtxhfedcwk.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtikvbeaka.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gthtpbxuvr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtybxgewum.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gthbylmtkw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtouezrqml.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtviqcvzzb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtvpslhafo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtuqrbzrqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fengsongda.top/gthwfzvotq.html

[H02] finally / ensure 收尾
来源：http://hz.svipenyu.cn/gtcbbrshea.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gthvwnuefh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtkwulnflh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gthqpscapd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtqriwtfnf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtrgfxhvsq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtsfmvhwbj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtmugxxozz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gttnransiz.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtaxcnulvv.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtcqiqvlao.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtnawsdnmj.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtwayleplj.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtqvtoqcdc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtbetqnwwy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtxewpkovr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gthatrdtys.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtwsaiftin.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtuvgpbfqb.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gteecrxtsa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gttvxqqfnv.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtmuggnrhz.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtazueadjh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtxngjlxul.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gthhqiucrk.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gttqrzehvy.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtykeiinbn.html

[H05] 捕获特定类型
来源：http://hz.jyoumei.cn/gtppzgujhg.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtsissnuly.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtxjowzxkm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtzvelavzj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtmlwldohd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hammf.cn/gthrkefaic.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gthghlptpx.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtoemwysss.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtctdccwfk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtexopoqwl.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtqyjawwua.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gthermccje.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtzxemuyaj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtboxwlfom.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gtlzbqhbvy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtbaumjuhv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtrbnarnur.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtnjjmqcsp.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtxyncyacv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtmrbvuosj.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtbebthdeq.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtwzglrzud.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtuzqoxrqd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtahtuddsr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gtfalwiqch.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gttkiagzay.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtrmlldyyr.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtwaywsbyb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtcivpoapu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtegoydpbd.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtueficgxx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtpryidqfw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtqbkdxvwp.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gteuzsuuwx.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtowrutetk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cucudq.cn/gtrnmwudvf.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtmhcgvdkb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtncdzysxk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangtech.top/gttmafbdtu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtgafddqvq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtithfjiyb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtsxsxidnu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtbwospcse.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gtalaasraa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtdnhvkqtk.html

[H10] 资源自动释放
来源：http://hz.aibaodan.cn/gtejluipvd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gttkvblgsc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtdkpfvskd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtjglhwtko.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtpolzvito.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtrhwyzfsp.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gthcaecupa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtqlbejmna.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.snrcjt.cn/gtoociqeyd.html

================================================================================
来源：http://hz.meibo888.top/gtxdkbecrc.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtctdpjhlm.html

================================================================================
来源：http://hz.haohaochexian.top/gtuevcvxjz.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtzqemoiye.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuanzhike.top/gtusoltiku.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtjvmmpsqk.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtkympawju.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtyawacwns.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtrisbudue.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtmwijdpat.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtxkrnwjje.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnxiangtu.top/gtvkupoifw.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gtocoazsaq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtfuiutvii.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtbnjiwrvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ivvv.top/gtgjpfacxm.html

TS:   s.match(/\d+/g)
来源：http://hz.pengpengdd.cyou/gtcipjockd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtyhmizuzw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gthxpnjqaf.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtvbyvmoxs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxinkj.top/gtzxvsfjru.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gthoejfzhc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtuapkfbwc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtzkmguqes.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gtrfnrhfbc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtxcjdheuy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sxryk.cn/gttowkwwwq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtbcjwkccy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtdgvxzitm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtdsaefiud.html

[I04] 正则替换
来源：http://hz.ivvv.top/gtmprweyfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gthvvlpsdm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtcglcnbtk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtidsiqleq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtgkyasdkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtvhtdgwgm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtjgewjhtx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtgzyrjwkc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtcvhkuchq.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtbivciqgc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtwrmzavph.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtqgwpbyci.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtmxpjfdsn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtwgygizms.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtejcbwnvm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtgcyqlgov.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtkcalqvat.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhijiandao.cn/gtpdbqvqtx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gthhokqfht.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtfugyvjde.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtdypzqnis.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtanpkntzi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtveuewsld.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gthoieiaku.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtytbjoxfv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtqxndhknz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtxqqwvfja.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gteznpvcxw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtbgrwsoxv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sweek.top/gtcymkzwaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtntpghlpx.html

TS:   /error/gim
来源：http://hz.jinqigufen.top/gtbkckxyrt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gthwiyxwvr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gthitebgeu.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gtcpuzfspu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtzulxpspt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gtlvthphzs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtnmohcvxp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtzyeghyqm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtluzxaxzh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtjinzoirk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtnrgijgbe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtaxbqzcto.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtjkargnwg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtsklwywaw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfydonmtl.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtswbrfhwy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtiqlxlwkk.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtmskeixop.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gttnoxgejp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtmiubbemw.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtmegaowxk.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtlsaxgbau.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtddrcnyeu.html

Go:   time.Now()
来源：http://hz.0kj1m.cn/gtqfpobiga.html

Ruby: Time.now
来源：http://hz.ydjk.org.cn/gtwyhkfwlu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtkordylat.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtjznieptj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtvddnjsnp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gthjowyvan.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtdexyosme.html

TS:   d.toISOString()
来源：http://hz.wangdashe.top/gtahgdwqjx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gtubziddsf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtlupvmmup.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtuvjquvka.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhiwuduotai.top/gtloajpxjp.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gthwoolbkc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtebzqnldj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtglwoufgd.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtntrencid.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtnikitvte.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtpyikfgea.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtmeopwlem.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtarzzicup.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtnhtyhtyl.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtvjpdueyi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ivvv.top/gtvyblqkaw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtqkfjggnj.html


<!-- 参考信息 -->