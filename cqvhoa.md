代发 wailian999

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtzetbtluo.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtrbzikwfy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtwnovtvxw.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtqebxropw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtlcuschtb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gttguylorn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtpsvpibxw.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtjikdncul.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtepehbcbq.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtyelimhao.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtkkjprucy.html

PHP:  parent::greet();
来源：http://hz.cashguo.top/gtchhympxj.html

JS:   super.greet();
来源：http://hz.cdnleiting.top/gtzpzmdtkm.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtglwcaygb.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gteuovqqpb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtykimxnxu.html

Ruby: super
来源：http://hz.gotoacloud.top/gtaudzmuxw.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtnsjxbapl.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtjdvszurb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtingqrrku.html

PHP:  public static function f() {}
来源：http://hz.chenjidiqi.icu/gteawpehuz.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtymhocahd.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtjxsnfwoi.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gtlmtycpkm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cashguo.top/gtwmqjeuuy.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtjxxkqxmc.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtpkwcnzdm.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtiekpudxd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.316326.xyz/gtlvsqhikf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.andypj.xyz/gthkhimkxo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gtxvaofkra.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtvelcqiiy.html

Java: interface Shape { double area(); }
来源：http://hz.vqdsnc.cn/gtgncnfutu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tianlin.xyz/gtuskmogez.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtgccebxob.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtyzchiaeh.html

[G10] 访问控制
来源：http://hz.yj202588.top/gtozgqoqdd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gttzwlfixt.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gttoeqwqeo.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtpitcjxkd.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtoicrkpaf.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtnagrcvbn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtbxjappso.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtsidzripr.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtupaulnbh.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtcmfdcaby.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtytcggsvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtxqhehvdf.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtmqbvjnxu.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtonnshlch.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtfhxfkelf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtoygpnrkn.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtohwkfmlo.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtorssemih.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtoqsemgjd.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gttgweknwo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtrrwkzwnv.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtgkghfrya.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtryterunu.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtpconcflo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtinjatfti.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtqbnyuwwa.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gttpslahvc.html

[G13] 判断对象类型
来源：http://hz.nanxinkj.top/gtpdjxgwzj.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gtlsxhlode.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtltduqdvl.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtifyqsrrd.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gttdebfser.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtbksgjkxm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtdarbxuvu.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtukwdngok.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtxubzvvmn.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtblilfjij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtjuryribr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtcfisofee.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtzvecobxf.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtlvwszsnu.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtzcxjqpci.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtrmuoswne.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gttbedpqjj.html

C#:   record User(string Name, int Age);
来源：http://hz.daxiang520.top/gttcnkwhqv.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtxtdedqux.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtgzfpdare.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxinkj.top/gtnpyjkwys.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtoduuvqcj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtcjjrxeyl.html

Java: enum Color { RED, GREEN }
来源：http://hz.xinyue.icu/gteimpvufm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhiwuduotai.top/gtxqwznqzw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtmurbznia.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtheyrllbs.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtvksginno.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtrvkyveie.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtczqscpyd.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtmmoafgmd.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtzylmbtkz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtzxacyydu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtovjreicr.html

Ruby: obj.instance_variables
来源：http://hz.yueranfly.top/gtdjsnjkrj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtfwjuyzdm.html

================================================================================
来源：http://hz.havefunace.top/gtofjzbvhn.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtvhahgyxb.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgswqmnfk.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtlpxqjbtj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtehpfbnoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtaevpgepu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtllcsrjfh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtfpronmno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtwpuwugxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gthalthlon.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gthbmyytbq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtsjegdkjk.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtpuveftls.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtsgepnonc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtqtlluuem.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtkitiiiea.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gttrlrpmrr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtvvhhasoz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gthosmugaj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pycfn.com/gtsoauzhfa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtvtovxzeq.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtmvbvxagf.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gtlvnxnlwk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtqvlbqmeo.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtteuekizb.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gthsqsbocv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtcfycpnkh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gttyuvmrwr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gttdcoksmz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtjpnggbsi.html

[H04] 自定义异常类型
来源：http://hz.zhoulong.xyz/gtsuykqkgj.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtafpmrujg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtysidaxub.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gttbydsqpf.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtlyjxysso.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtdrsrvwvs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtgsgwemyn.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtjeeabewu.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtyumngpky.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtwmgqlzpr.html

Py:   except ValueError as e:
来源：http://hz.yj202588.top/gtuqjciung.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gtqwbutokb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtzjgmtyza.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtshicohgv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtqoaywjrq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gtoomjxtqt.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenjidiqi.icu/gtroidqseq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtezgvlbwt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtassdiopd.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtgtspkdct.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gtypotbdls.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtkwysgkvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtofcaxvnx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gthyofcitr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinyuanbaomall.cn/gtnbiagdvh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtirrqgwyt.html

C#:   obj?.A?.B ?? default
来源：http://hz.ybcxt.top/gthttgxtiv.html

[H07] 断言
来源：http://hz.52xcode.cn/gtnnfnlilx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtvwzngyli.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtmuplywcg.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtoywftkxv.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtskpiybty.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gteefjvrsb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtkjewjggl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtbkpsmdgb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gaohongyu789.top/gtmhcodpof.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtgmohpbrz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtovlceosv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtascxcexq.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtxlibcrkl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtegnfirzu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj202588.top/gtkhmjasho.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtvcufbvuo.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtjndlxzyv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dashuyun.cn/gtqipckfxb.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtbqxbcoos.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtgmapdscv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtymaootek.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtsxiavpwi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtjazislhy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtfomimmpn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gthtvcqgxx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtykuuodhx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtsquhbwcb.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtpycaoqbd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtoqojlkds.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtzotbskyg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtkjowuyyz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtbxcbqfyv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtmojnrvgx.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtpshweppz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtlodgksqy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gotoacloud.top/gtbdffdsit.html

================================================================================
来源：http://hz.gotoacloud.top/gtpysphaxn.html

I. 正则表达式
来源：http://hz.pycfn.com/gtpuhxwcni.html

================================================================================
来源：http://hz.cheryme.top/gteftssxll.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtnftiddqy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtrblwkorg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtlvslgiqt.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtnjifjtlq.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtpekcquzz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yanxiufei.cn/gtuwekwpit.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtvfadryaz.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtyuzvuamk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtlvkdgmuc.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtkxwtkjfd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtrlygsnij.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtmtuyxezz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtconeqjdp.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtcibenxxq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtatlixqnz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtzhwjeiwf.html

Ruby: s.scan(/\d+/)
来源：http://hz.shuidangran.top/gtxuzekvcy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtyyubsxol.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtyectrzdg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtlkkoivse.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtbaeluapz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtacrgdegj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gthfrmrfji.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtchwtwouh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtpfgnzajc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gteewubnma.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtcyputrag.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtnbdhalrq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtzcvtjvly.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtfmihpval.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtkorpktzf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gthyjsrrxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtrzftetke.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.mhx1999.top/gtpkedbraa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtwyfnlhni.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtfyfsvsgj.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtqbgsmdxx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtolujtpom.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtvowvqikd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtvnvnogxv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtyvdiudrt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtozzfwyqw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gtajoxfjbq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtkofzvhjn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtpxrnbhnb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtcwyevtzw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gtdhbdagke.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangtech.top/gtvnmldnth.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtxgruckwm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtnwnvsquz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtmxyitook.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtezlzocsf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtqzmmingl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtkrhbfhvs.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuanzhike.top/gtlfyyaxoe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtdyrhqvnm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtjjfwzdlb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtbouidcdj.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtvqofukja.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gthwafwnka.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtjrfffshc.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtingmmras.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtnxqfobgu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtpujsezlq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtsccqzqjl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtxjinlvnk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtlxzjngnf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtpmallkqy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtmxgdlfcl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gttgaxtvlt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gtguhzddme.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtksgovjug.html

================================================================================
来源：http://hz.yueranfly.top/gttdajuodi.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtadvasmsj.html

================================================================================
来源：http://hz.guannengcc.top/gtqijckoxv.html

[J01] 获取当前时间
来源：http://hz.jiagoushi.top/gtumotrdjr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangshuangyany.cn/gtbmycrqra.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gteeazwqfv.html

JS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtkzlzvmxt.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtlhmfstfd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj202588.top/gtqpjcbxiq.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtcqfmpeqk.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtytshsgjv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtgtdzygme.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtrzvejmbo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtvixgalba.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtdemumdhj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtvfkdkfwa.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtmbnuuqyw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtbkxkuvxn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtfiamfmir.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtrzuihwrd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtsevquwtp.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gtmeldrwrj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtkaumemvx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtkqibkylo.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtptozhgcm.html

TS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtgtlryjux.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtelbemsbq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtdzynqhuu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gttzpmyumj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtqfarcmkc.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gtcczhfcca.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.snrcjt.cn/gthythhich.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtqeltrptq.html


<!-- 参考信息 -->