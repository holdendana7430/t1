代发 wailian999

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtcssrfuus.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtiffgtyak.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtobaretsw.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtpsuddtrm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtmunpgqwq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtlxkzvzkq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtpxhqnptq.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gthpohxngf.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gthyuclxby.html

[G07] 调用父类方法
来源：http://hz.dashuyun.cn/gtricpgejs.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtjrlmkxvz.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtkcwhfdpy.html

JS:   super.greet();
来源：http://hz.quarkkingdee.top/gtqjdryevf.html

TS:   super.greet();
来源：http://hz.9152youxi.cn/gtyohhnpsp.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtkpolndad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.haohaochexian.top/gtttcmfflx.html

Ruby: super
来源：http://hz.yvedp.cn/gtuvwjldgw.html

C#:   base.Greet();
来源：http://hz.redwolf501.top/gtchgqjmgn.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtcagmvukh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.mhx1999.top/gtfdyjdmfo.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtlolilmut.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtginqefvg.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtkndfyacp.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtewprxode.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gthabikmyo.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtreuauzfu.html

C#:   public static void F() {}
来源：http://hz.yonumen.top/gtbiotfwwy.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtbpkhusix.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtkokdayun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtdsiaqboa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtyvcvbulo.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtnacocpwh.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtekjiqikv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtlezdvpuf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtftrjidev.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtkknmowiq.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gteeioungg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtsrymojss.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtbkzcyibz.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtdwlduacx.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtcefttwyt.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtkcsdbmga.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtwixmbvbh.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtdbbxcqop.html

C#:   public / protected / private / internal
来源：http://hz.ehwqpu.com/gtshgknmjy.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gthfvsrzlg.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtqyidsqbg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtkefxbwtc.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtsamctkai.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtzlhlixuk.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtlwlhzsgy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtidqujyhn.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtypdtgqrb.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtkskdrwci.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gtjufbkoix.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gttudpsixb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtwvyyckmm.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtyihjiirq.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtrharpvbd.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtaunqpmik.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtxxdciizl.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtwrgulies.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtrqlylhci.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtwvrxkcwb.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtmerheoem.html

PHP:  $u instanceof User
来源：http://hz.jinqigfzy.top/gtwhxdphbr.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtfyrjlrrr.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gteeczjqjb.html

Java: u instanceof User
来源：http://hz.sysykeji.top/gthslckgai.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gthceeljvc.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtlkpolmcf.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtyzypuevb.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gtjfofrdqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtmxtbxlbi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gtfbqqhsow.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtrrhhlngv.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtafhhazgv.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gttvbzgroo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtjehluzsh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtnqdukwec.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtrbhhuqmf.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtxurxpbgv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgfzy.top/gttxdycuni.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtwmgrztow.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daxiang520.top/gttcmaavjg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtktyyqyok.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtibdkdwgj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtqgvoqaxd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtuozkuevm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtrseznhwm.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtrnuyiilo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtpikrpwds.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtoeoxsrvu.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtkudfldwp.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtxufvxkxx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtgzytvsrx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtoboblaos.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtwexhbbuf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gttsppphts.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzmakleka.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtubsmcdxq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvwxoudwy.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtqvdasevq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtczwloffd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtrwdlipyg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtqckwgyhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtpmmrlfsh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtpyhyrnlg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtnvxaiudg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtuzyilkaf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gtfxnoiyzl.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtpodpiufa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.haohaochexian.top/gtedvjspqr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtxjbixmpb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtirvrpxav.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtnubcspbs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtrqgjfjoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtrosnvfqg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtbkadfshi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtajnsripl.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gthzxjexnf.html

Py:   raise ValueError("错误信息")
来源：http://hz.hysaishi.cn/gtjxioytau.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtzrcjonmf.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtnkhtklox.html

TS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtbibrrcuc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtxzexxrhr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtxskluvdk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gtpegtyweu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gteneodqus.html

[H04] 自定义异常类型
来源：http://hz.hywenlv.cn/gtvboecywr.html

Py:   class MyError(Exception): pass
来源：http://hz.hongshengwenyu.top/gtsbnvtqsm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtdgwlvjje.html

JS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtrkzzwtme.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtuqwonjwe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtskxobopo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhiwuduotai.top/gtxtyodcwl.html

Ruby: class MyError < StandardError; end
来源：http://hz.zycfv.cn/gtbbhzmeaj.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtuumvoicc.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtvxamgwcf.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtfymhptxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtcgirmgic.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtyhviihll.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtivnqhfup.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gotoacloud.top/gtypsyvtya.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtsoqfiphc.html

Ruby: rescue ArgumentError => e
来源：http://hz.guowangkeji.top/gtwkvegpqb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtvjsfjhdf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gotoacloud.top/gtczvgtzpb.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gttlgfzqnh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtmyyhylgm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtaaqqphbf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtciunglom.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.iojbl.cn/gtaxqcpgpt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtmdvmlccz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtcbvtidzn.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtxfqvpygo.html

[H07] 断言
来源：http://hz.yueranfly.top/gttbdyxolk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtijwfhykz.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtobdocqvi.html

JS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gthjqhzlro.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtdclrzfen.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxinkj.top/gtorgxcxmv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gttmlnmlzp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gthifegjje.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtyytlblxv.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtivhtcsnt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtsjijfcjn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.redwolf501.top/gtnkktgzkv.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtxlosfygr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtdiizymko.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtkgjeycfm.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtwrnqqzrv.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtvwxsttmf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gthypcpxli.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtpkztdvnq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtkvloaqgf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtzgitcnll.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtbihbiwhy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtfybykyvb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtdibejosh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtyocclpxk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtjbuojtqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtcoeybyjk.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtjsibxsxe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtvguiyaio.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhixingplan.top/gthfatxewg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtmiyircrv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtfgfdbrkc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtuvyoxrrs.html

Go:   defer f.Close()
来源：http://hz.ywan-chungtsiang.top/gtfkifsfff.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtvlomqrvy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtnzpjlwfq.html

================================================================================
来源：http://hz.guowangkeji.top/gtehmmwpkz.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtyyomqfhu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtthyzwdxr.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtodiragax.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtkjfwoekh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtzoadgbof.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtwzrhspgv.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtfuhayumf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtxogqdcgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtkokaydft.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtkzloiprv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtcjdbdfyi.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gtxugoarum.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtlmarebdt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtoeajapum.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtmedvheub.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtjwnehixh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtzszcvgnu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtzxkzjvtb.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtvwhkjcte.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtepnrlowq.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtrwifavbq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtpmbyicyy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuanzhike.top/gtukelmeop.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pycfn.com/gtakosrnvm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtlarlgzct.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtjyypcpxn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtkiuvvfwy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gthyzhyjok.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtaguujrwi.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtywimgacs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtlbwxqztb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gthdzzktlx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gttowcutkb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtvjgwdfbj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtlxqktrxv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtxjzraldg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtvhfrnsiz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtkjmmsvrz.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtqunxxfxc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtnjjozevq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtwwdzdykp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtzhofftox.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtshrnlndm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtneqovibx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtkwvkzjwe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtdbndcwtc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtmbztygwc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtcambzwvs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtrycwntxa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtmbrgczve.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtizehlqrt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtpqoopktk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtblyjcosx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtyzyjbxak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtjpemywym.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtazaoemnd.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtberbfgwd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtfwttfzdo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtpmqhwqyi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtirsvecug.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtgwuckoqp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtiyhoylyq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtdmvajotc.html

Ruby: s.scan(/error/i)
来源：http://hz.cheryme.top/gtgmlrxrmc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtufiaiinu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtppahnwoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gturtgadkb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gthzgpddrx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtacwmkewp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtxkkxihio.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtwfulzlpz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtewntsqkq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtrpdafkue.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtorqslzys.html

================================================================================
来源：http://hz.316326.xyz/gthjpahcan.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtzfeuhfuf.html

================================================================================
来源：http://hz.xziqi.cn/gtiljzrbut.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtlzebtiww.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtkgmohyse.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtdynjxirz.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtusxqinxi.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtpmpenhiy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.quarkkingdee.top/gtlpdzamtb.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtiobsemek.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gtivawdyww.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtvqwbyhjt.html

[J02] 格式化输出
来源：http://hz.jiagoushi.top/gtjumrgifz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtudyfeooj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtspwyapzq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtltpdqcey.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtjkancxrb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gthvzxthsk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gthxlzihxy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtfzvgmwhs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtuoduomma.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtdtktsyfr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtdpnvjepz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gthwizwckl.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtzmnavpeb.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtheomourw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtxdwqaswr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtfgfitaqc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gthuiingnl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.svipenyu.cn/gtudvlhktp.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtdxmdzlzw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xylfe.cn/gttmljcrlv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtolvoawac.html


<!-- 参考信息 -->