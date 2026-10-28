代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtyiuqdhad.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtpdvuulcq.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtkjevdfvk.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtxbrzvcag.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gteidlovli.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtcatuqdvw.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtkfhurnkc.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtohpwnnjn.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtdjmfeytu.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtexxyywgy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtsgsudusm.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtmugbzjan.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtddsqxdsk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtiohwnlqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtrftkuxps.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtrptboglt.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtfpgkacjy.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gtgapficve.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtytfawmba.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtkrndwvol.html

JS:   super.greet();
来源：http://hz.jqgufenzy.top/gtwwjobsoo.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtyqjxgssb.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtkdhapuzb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtvkzjvilo.html

Ruby: super
来源：http://hz.haohaochexian.top/gtqyligvco.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtbqebtgth.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtoufsizis.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtnhjtpkah.html

PHP:  public static function f() {}
来源：http://hz.nanxuanxn.top/gtcydmpklk.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtqjyiqjuh.html

TS:   static f(): void {}
来源：http://hz.xingfuxueyuan.xyz/gtmmorggjo.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtpofadeku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtxoqxpiif.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtddahxzou.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtrpckgpsj.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtxajansfm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtawlyhpic.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hysaishi.cn/gtwperekvn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtcnvgyovh.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gtdzisjipu.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtocnzixmt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtkreqcdvl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtbrooccmr.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtwoanvekd.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gttchuyslr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtjsffzokk.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtusvepgxk.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtmzhjzytn.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtgxfokpej.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtvtchwwux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtdfsgoznp.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtyiyjobgx.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtirzwaupw.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtfqodqvzt.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtypjibsgt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtqwsbijtb.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtegabnlhg.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtwuqouzlg.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtocjyfrlj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gtjuiescqk.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtafgwvwpf.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtsljivrze.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtgrscmfgh.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtazfjudyk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtffvcrbvp.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtxqmnnmxp.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtnlhshcfx.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtbojshicf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gtnuyagxxz.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtvrrlbhoy.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtzmmtcxvu.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtajkurqrd.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtgowynpem.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtykpsklei.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtdczvklqd.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gtyciupizc.html

Java: u instanceof User
来源：http://hz.xinyue.icu/gtuqyozxcj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtpbpgqiyq.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtpwozrzoj.html

C#:   u is User
来源：http://hz.daria6918.cn/gtbuhpedbb.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtrfyhurjs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jlsjyb.cn/gtbnosxcdy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtnfimuzbt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gtwhqelaad.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gtjmpkeywg.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtpucsvpez.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtrlstxjfr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtotelsdeh.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtcshwtwwb.html

[G15] 枚举
来源：http://hz.meibo888.top/gtfagkbxhl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtrbechalh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtfnmpncux.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtaqvtrtri.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtfutvbwqu.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtgvowjcuk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtigidxnnx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtpvjsypuc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtbwacyrtv.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtjcnwzwej.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtrhglbclw.html

PHP:  get_object_vars($obj);
来源：http://hz.c1oappe.top/gtcodoyhzo.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtomaicnrv.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtohbuxfbb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gtbfehqacd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gogol.net.cn/gtmnbjbigh.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtbkyizwta.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtuqsfxjbz.html

================================================================================
来源：http://hz.smart0.xyz/gtlnxlbbqn.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gtnybzfaqc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqvkswvzc.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtiuwafpji.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gtnrukjbrb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cucudq.cn/gtqjlpwspg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtjkfkyjoz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gtotrpylig.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtgeewqhki.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtsfwacgth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtgvqntuls.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtoustsicz.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtwbygdhuc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtmheugysz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtlyxwzjgq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtltymjfwy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtxyvmbfoo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtszidunyk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtobciksdl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtnsmhvkua.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtnnewkqdr.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gtlxwwizwo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtudvoyott.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtgklvcpxy.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtjmnwplqe.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtkpruykmh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtmqigilao.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtopowdwjj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtnryijxqj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtrhoelysn.html

[H04] 自定义异常类型
来源：http://hz.jqgfzy.top/gtyabeacsa.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtrqrljzwh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtmxothilb.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtficvlpbc.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtorplyqni.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gtvyijbrao.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtzuvlqmbc.html

Ruby: class MyError < StandardError; end
来源：http://hz.pycfn.com/gtgbkibixg.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtvdlodljr.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtidaxbmkh.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtdkgkxuko.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuetiantiany.cn/gtfqyxdhyf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtutdvwwsq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtyauzwiij.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtewfvicrb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtjlrtqbwx.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtyykemiwk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtmbbxmdpz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtpqozugau.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtxisyxlju.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtxdmcqjys.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtwfbfthgt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtareqqgoa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtswvxbrms.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtbxvqvnbm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtdioaodks.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gtvxsvqosj.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtivsgathr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtltpwfqso.html

PHP:  assert($x > 0);
来源：http://hz.shangyingyoupin.top/gtwbbzaobx.html

JS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtezmwzbku.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtlmkysbkj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtdfkiqygo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtipgqqahv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtqdfmymsl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtipwurhch.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gttoljbvty.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shzxlz.cn/gtdsliwkgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hywenlv.cn/gtdssztywa.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtrpdcburt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtshhwlpcx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtfztxacpm.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtcpquivye.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtjjbyvrvv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gzhubu.top/gtysluhfbe.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtkeprajqk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtlihgoxwj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shzxlz.cn/gtjvehjsgo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtgsvbyroo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinghuilouyu.cn/gtfphudlhf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtyvrzmmmb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtlayfdyxd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtrbiccubs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtdymdoazo.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtwruapjno.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtmdaynqoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtcbszzrcl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtwapdptan.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtwhrlkfqz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtwubniiap.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtugifcrcs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtbjpswodj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258888.top/gtmruuywzx.html

================================================================================
来源：http://hz.yueranfly.top/gtlbieheqj.html

I. 正则表达式
来源：http://hz.daria6918.cn/gtmdpjbntw.html

================================================================================
来源：http://hz.guannengcc.top/gtahabkary.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtjfedxito.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtofzqitya.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtkhdnzwmr.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gttailniiz.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtjyiijuei.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuetiantiany.cn/gtnwjfwixa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtnemmnwqt.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gteejkriwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtxzrtilwx.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtwegxaysc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtjzhuuruz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigufen.top/gtnwbeprhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtdwaxcijw.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtzpxajocl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nwbrower.top/gtvhkwcujb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtxzqookfu.html

Ruby: s.scan(/\d+/)
来源：http://hz.aizwys.cn/gtoapqiuez.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtriwaypvw.html

[I03] 提取捕获分组
来源：http://hz.haohaochexian.top/gthrsjrptm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtgnvixazv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtvgtcovvf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.birdmap.top/gtaoyythoq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtnyiwcuyp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gtjfmjsdbs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtkhyvhwjl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tian-w.cn/gtrzwtdlgy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtadfcpzxi.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtovqzptsr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtcisaejxr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtvbrytqun.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtsdvnkgdo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtrncsqjbn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtyzzwrexv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtwjeakocx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtbjvznmdv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtpkcljnrt.html

[I05] 按正则拆分
来源：http://hz.ybcxt.top/gtmdjdpfpz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtnwxccevk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.0kj1m.cn/gtijgmidld.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtuioebraw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtupjyekgd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtmqhijgpq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtqormmbjs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtchtwuzpl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtwkabtovx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtvuffirpf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtjarcbywi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtmcrvnbnk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtwevivxzg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gttlkgvals.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtyktytwdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtfgezijcq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtjjabjftm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtrwmzzkto.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtsichfvkr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.316326.xyz/gtjrbgrfss.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtuglngrqv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sweek.top/gtkpltmznj.html

TS:   /error/gim
来源：http://hz.pycfn.com/gtxsublobf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtxrvtekyr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtbrchnzbv.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtxqyqfllz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gthrmiwona.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtdneimtlm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtypunulsf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtoykhsfgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtbqccrhog.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtmkrmxxoh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtlratwkha.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.bjfxy.top/gtrhrhhzqf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtyujitjkw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtkgomxvmu.html

================================================================================
来源：http://hz.andypj.xyz/gtiwlwiwfp.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtfowelosg.html

================================================================================
来源：http://hz.jianghu66.top/gtnhtycmpb.html

[J01] 获取当前时间
来源：http://hz.daria6918.cn/gtnmgkxzkp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.havefunace.top/gtbfqujuau.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtdfvwmtzk.html

JS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtrwlbncqs.html

TS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtuzlnsprv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtuptjucry.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gthtwhvkrm.html

Ruby: Time.now
来源：http://hz.iojbl.cn/gtruxjzygc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtcsjfzjcb.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtdszsgwav.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtipusjeeb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtynikpbvb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtiizzdrap.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtncaxwipc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtmrwkizow.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gtrbckbvam.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtsvdfyvhb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangtech.top/gtpcgpetaa.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtcwizevjs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtcwendeqa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gttaturuku.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gthkzhzzfw.html


<!-- 参考信息 -->