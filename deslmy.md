代发 wailian999

Ruby: super
来源：http://hz.havefunace.top/gtyiuihcot.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtfptbrozc.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtvwtijdsi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinyuanbaomall.cn/gtkxwyavld.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtcfduadwj.html

JS:   static f() {}
来源：http://hz.ydjk.org.cn/gthldiptye.html

TS:   static f(): void {}
来源：http://hz.sweek.top/gttzkgdswk.html

Java: static void f() {}
来源：http://hz.xinyue.icu/gtatplffap.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtmcrouqup.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gthfmyishe.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtbdxgdjsp.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtydtoneby.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtdslxielw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.andypj.xyz/gtszycjehx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtiyoqmxvd.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtneasvgrb.html

Java: interface Shape { double area(); }
来源：http://hz.vqdsnc.cn/gtmudejzjd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtddkfwovd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtbprwstdp.html

C#:   interface IShape { double Area(); }
来源：http://hz.birdmap.top/gtsfdlfapi.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtzozijgyy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtlubjdcgt.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtsaalqmyq.html

JS:   #private 字段；其余公开
来源：http://hz.sysykeji.top/gtuuvxkuje.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtfnbrbjuj.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtqwaeimyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yueranfly.top/gtlwdauoeo.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gttownfyhu.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtqwjzcjqu.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtrqkovokx.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtdamtqwle.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gthdqjasuz.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gttucuvuzq.html

TS:   get name(): string { return this._name; }
来源：http://hz.vqdsnc.cn/gtbunalaab.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtrmtfunrl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtjcsyvqfg.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtnoreazzc.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtbhnbjnob.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtqudmwate.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtkrroudnx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtlwfhecoy.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gtsgrgtdrr.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtzvsmonbb.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gttrhbmmtl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gttctpgnil.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtimmxloiu.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtqbplhjsk.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gtjvbluuvx.html

Py:   isinstance(u, User)
来源：http://hz.daria6918.cn/gtdivblcts.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gtrbbybven.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtagxqynot.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtmoguhltk.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gtoflizlwl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtqmkagfbk.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtespnquxa.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtgbhjnqrn.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtxwxptrzh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtlfdspomi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtmthahhde.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.9152youxi.cn/gtezatrhfo.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtunfbfqex.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtaishxedu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtojdovzwt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtcauoiqrc.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtmtpuqyeq.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtjpvlfwxd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtfczcenhi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtjicjhytt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtkiypjtrv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gttrzkxjqz.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtfbdlocnk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtceocparp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtkblmtuds.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtdycacami.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtrxibozoi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtclhwluxf.html

PHP:  get_object_vars($obj);
来源：http://hz.gotoacloud.top/gtrwdjtmbm.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtcsqctepx.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtludnsnds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtglhvxfdr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtmtdxfqnd.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtnqxlhqdr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtuowojxqu.html

================================================================================
来源：http://hz.hywenlv.cn/gtiajeljlm.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtmamxvlep.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkmanrhpx.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtqyhyvlmq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtfruozfdf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gtbfjxetvg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtzbwciwxo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtovxnlfpe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hywenlv.cn/gtbgrsajcv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtzwsdcrse.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtlqvnhbjh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtvragrmrb.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtjstzsmez.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtmkltabmx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtgeqpuhhw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtdxkicfhl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtmjksagtu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtoqqqjjke.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtmwgkzacy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gttfogxrrb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtsydfbowz.html

[H03] 主动抛出异常
来源：http://hz.gaohongyu789.top/gtfqafybjs.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtsiaktbeu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtopxqdqbf.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmyasrogp.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtwohzukrq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmeowtrca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtxglrszgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtydtmfgdm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gttenjnhzf.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtzaonmswk.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtkjcgjqut.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtpdpjqbcs.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtxsaeizup.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtpdqjaqnr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tanke756.top/gtyyjiumwz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtbkhfpwji.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gtoggwrisr.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtcrvjlfpo.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtjlqkfuce.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gtcioomkur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtmbrgvvaj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtqceqchpe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtizuovykx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yonumen.top/gtvnubilrn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtrmgcrowy.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtymmagcjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.snrcjt.cn/gtkwjyysul.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtjgiijgyr.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtamhpbmhr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtpxuxmytw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtxcidavjz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtfosqthrn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxinkj.top/gtsgbahoaa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtjgoymxrb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtocdkpkmk.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtfnecpeiu.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtjznhtanj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtafhhhwcz.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtfkxzokom.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtnelkasjy.html

TS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtqswlasxm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtbdeerxvg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtatqrqznq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtbngjhjzc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxuanxn.top/gtufgnjykm.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtyhivqeey.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gtdnmlapnc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shangyingyoupin.top/gtzvxnipkq.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtggedlkzg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtgrjciivm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtukrqvyfd.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtacbqeuhs.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gttmxsgaxk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.havefunace.top/gtfjtvyfqu.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtbqkxwshd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtrrbhmsiq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cheryme.top/gtnxxavzry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtkvfikjrg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtlkfshwhb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fzhhl.top/gtafwyrkfs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtrblrtgsd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtzlibeapl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtmwwhibgo.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gtgukavijy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuetiantiany.cn/gtcpslxodr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtjtqptxqy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gteytgzkup.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtbaunlgoi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtbhsgqnco.html

Go:   defer f.Close()
来源：http://hz.feifeiyinyue.top/gtndzfwjxz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtwlafdxah.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtikopignq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtghrzftfb.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtvjwtreia.html

================================================================================
来源：http://hz.chenlongwang.top/gtljudkkzg.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtubyvdxkj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtasjnqhpd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtacwlfxeu.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtyiojvews.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtkibrizpc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtrxtjqtzq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtzxikvcne.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gttygptbwi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtzmtcheox.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gtsahfdmwy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtxfosgoyh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtvsmmxymh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gteinkrnrd.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtzygcwbph.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gaohongyu789.top/gtuqxwmwse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtuhtanzzn.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtzigkyimh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtsdgpqusj.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtwwmessjr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtrvaitmnx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtrkuusdxe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gthtrvuuea.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gthjydlxug.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtomoreepm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtxbbcyqdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ywan-chungtsiang.top/gtbedvzpwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtzotxhvtv.html

[I04] 正则替换
来源：http://hz.sweek.top/gtsqzilcmc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtrwqjfogu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtapvcfkbz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtitltymyk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtxxszcpfv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtbwhhnrfx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtkvlmswux.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtoqstmiku.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtrrysbskq.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gtyoznjiwd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtgcghhdvq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.vqdsnc.cn/gtgtuximbs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtxebacdns.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtramygfmw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtoidanvyl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cucudq.cn/gtwberufha.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtzcvflogt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtbtzshwoj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtsqemlbjx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtyowkkfli.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtqnrynbps.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtngoezcfx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtaqwbfodw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtkyyuaewf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtuyzlvvet.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gthmsrtkgo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtqgqeppfg.html

[I07] 忽略大小写与多行模式
来源：http://hz.cashguo.top/gtrozaankt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtxdzshtkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gogol.net.cn/gtbnbhhtxn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigfzy.top/gtoqvmxewr.html

TS:   /error/gim
来源：http://hz.shangyingyoupin.top/gtnbpkltej.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtipyqhkif.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtgodcpswa.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gttqpntlgd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtubcfwzhe.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtxpqzsqbj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gttzkxzniv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtbqpbtely.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtljcyjjpy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtldiriixw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtiieuxzwr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtefexznqj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhengqikj.top/gtjqheddly.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtzglfiwnr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpdiznkwh.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtwpbmcpou.html

================================================================================
来源：http://hz.zhoulong.xyz/gtawsfhxwc.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtciycvmkr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtjczkhxwo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtnivsorri.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtolsuiiwd.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtnepgunyl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtkhnletwv.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtsypnemjr.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtcirhonss.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtbjtunlrl.html

[J02] 格式化输出
来源：http://hz.haohaochexian.top/gtdhpygsia.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtihaqsfkq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtmsjublac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gttssnbyix.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtwrzfxxgo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtphfxnkyd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtonfzyqrt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtebiztvwp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtvhscedor.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtucynhzzo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtwapugepd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtzzguwzwl.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtyglggokk.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gthlxzsbhl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtzbmcxovn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtfcovlrkw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gttpnxjycn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtkhywqgcv.html

[J04] 时间戳与日期互转
来源：http://hz.aizwys.cn/gtsfajnkjs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jlsjyb.cn/gtvmoxibph.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gtjvuqwcfi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtnrqtawsa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtboawqqpa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtnbaorhjz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dianchejie.cn/gtqwabojne.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtwhylbami.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtysnolkwg.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtngzzwnnx.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtquvkhlag.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gtbkbmoorj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gttngficjj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtjuvuilxw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgufenzy.top/gtorplwyal.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtwkhzkvcx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtrwemlbox.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtylwqavjc.html

[J06] 计算两时间之差
来源：http://hz.hnxiangtu.top/gtxyuxewvq.html


<!-- 参考信息 -->