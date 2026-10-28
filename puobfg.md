代发 wailian999

Ruby: super
来源：http://hz.jiagoushi.top/gtpyyszsva.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gttsikxwvh.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtcucyaabq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtpothwwmt.html

PHP:  public static function f() {}
来源：http://hz.zhiwuduotai.top/gtjgpjarcu.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtydtcvywf.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtchprksro.html

Java: static void f() {}
来源：http://hz.xziqi.cn/gtuoyhrkxa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtscfketnd.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtccnlipzj.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtuqmqdlka.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gtwexzgvfh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yvedp.cn/gtktlbulci.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yvedp.cn/gthwhunfgr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gtgigfadgn.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtshrngyqt.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtybyhbdja.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gzhubu.top/gttihxplct.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gthwqhozbv.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gthztvmkjf.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtahzvbzox.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gtxcqiucut.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtqgnowlqw.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtisufwxfl.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gttmfjvjqc.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtuxmnitbl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gturrgxzfx.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtdefhwqwn.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtskxekjdk.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtgrxgaqko.html

Py:   @property 与 @x.setter
来源：http://hz.xuetiantiany.cn/gtlcheuryp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtyjzmlinx.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtfobxjern.html

TS:   get name(): string { return this._name; }
来源：http://hz.svipenyu.cn/gtscizaqsw.html

Java: public String getName() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtezhvpwhn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtjrhprspo.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtrvxywqtk.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtccbredgu.html

[G12] 对象转字符串
来源：http://hz.ivvv.top/gtfdwqoejq.html

Py:   def __str__(self): return self.name
来源：http://hz.pycfn.com/gtbqibkfti.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtqkpezqke.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gtujsvwvjb.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtviawfplx.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtxbsiqrgu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtrskakjnc.html

Ruby: def to_s; @name; end
来源：http://hz.daria6918.cn/gtddvmceuu.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gtctrscsek.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gttgmqwpcg.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtqwxqxsca.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtjsqxipvu.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtqbmwfcgo.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtmmoodtfk.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtlnkqkgxu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jiagoushi.top/gtttxxgfwf.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gtmffgjxwy.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtezfzjiok.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtevbgnkku.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtoblqhksi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtyfxyzptp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtcitfoszx.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtntjnzvyb.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gthyljzzde.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gtoftagkhm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gthpebvbih.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtrslzkdud.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtkcyvreev.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtlircwfxq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtawdbguid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtpsgtbdwp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtbwgeuhtj.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gtagvhcsfi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtprznguuq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gthmblxpup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtlmiiidrt.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtximfnqrr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtsaoekgue.html

PHP:  get_object_vars($obj);
来源：http://hz.jiagoushi.top/gtfhuifupj.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtrdnienti.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gthzplvjln.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtxeewwtof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.0kj1m.cn/gttozjwhwx.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtgmhrmqez.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sxryk.cn/gthtcbwtdb.html

================================================================================
来源：http://hz.yvedp.cn/gtmuxisksr.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtjyvcxaml.html

================================================================================
来源：http://hz.mhx1999.top/gtsfzuwwft.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtmlyotdck.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gaohongyu789.top/gtlequbezb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangshuangyany.cn/gtiqqtmzpi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtzhyivoyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtahjysapf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gogol.net.cn/gtfqsctork.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtfyxshpga.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtgbafsjid.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtbjbjpcna.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtfbrgtcpu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydjk.org.cn/gtkjcrlfxj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtrfcjtfxx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtcggtjhko.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtfpaqyzsb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtwqjizyyf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtyttdgfhe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.quarkkingdee.top/gtqwbslvlj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtppcxbwuf.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtzkawtzbu.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gtaxfsvbxw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtaejvdnuh.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtywmnakyn.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtfhzqsuam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gttwzvsmds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtaahlqulf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydjk.org.cn/gthgyjsatn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtvxrtpnpj.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gteltpccrs.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtdpsfmuun.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtrhozwodq.html

JS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtxhkxjuty.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtvdjmkekx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtjfkhodaj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtoslwlgmy.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gtskrituyx.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigufen.top/gtyuwpjvsk.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gthfhicgem.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtrfpuvsdj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinghuilouyu.cn/gtvyiuwval.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtksoealyq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtdzqzugjo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtysgpbaul.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtyjaugueb.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtgscyvdnl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtphuiqtvh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tanke756.top/gtdyuvrqfy.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtxqumbrqx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtibymezgt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtuoaocpyq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtpvthfcvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sweek.top/gtyupmjyhi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtjlmtttam.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gthhjfajrz.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtdxaqaijr.html

[H07] 断言
来源：http://hz.shuidangran.top/gtpsjdkgwx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jiagoushi.top/gtzjhfcypa.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtruhwqurh.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtgmhaiyuw.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtiqkjucee.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtjbtkaktq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cashguo.top/gthnndgkqr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtdrvgljkx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gtrgoawsmg.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gtwgalxhxv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtvnuirdkq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtqisjqcbs.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtrmrgptco.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtvnjprffv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtksxxkssh.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtrencwjcq.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtjhvquvei.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgufenzy.top/gtxdevdimb.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtfkcwdoao.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtnstkyzbe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.smart0.xyz/gtghcocrjt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtisytwoyg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtjhwtwctp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gtpkbjljae.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtpodecinm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtoxpgvwwo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtsjaihfob.html

[H10] 资源自动释放
来源：http://hz.tian-w.cn/gtccnomvwf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtvbkzeqar.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yvedp.cn/gttmsypiqy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtxgnhgemp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtveucimgr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtzvbfgvcq.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtzqdsecdx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtxfgcpbjl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtkzrvrkxf.html

================================================================================
来源：http://hz.hywenlv.cn/gtuhlvlezu.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtevcyktlm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrixxepya.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtivgdkark.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gtiwevqjwx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gtkhmikoad.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtiesibnwa.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtwloldmey.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtblirdfvk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtfxqiinzx.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtokzfknwy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtxsnuaqsi.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtyelnxkee.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtcepoqhkp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtbidhkljr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtffoeyhwj.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtdiqytqjv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zycfv.cn/gthvhfzcpc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydjk.org.cn/gtawsrspal.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gtyzvypisq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gttuasvywf.html

[I03] 提取捕获分组
来源：http://hz.shzxlz.cn/gtbdxfjhka.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtoxbkgasb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cheryme.top/gtchhaieie.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gttsohtdpq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gterhdqinw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gttheztwsg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gtdnocjbzi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.vqdsnc.cn/gtfjzobdoh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtemkpvdrs.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtzjjrlegy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtfgjkefcz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtyejqycnr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtupiddaur.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtipbfauni.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtpnjxhivt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtgspgxkjt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtjpnptrsw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtypftwabp.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gteqjmfdzz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daxiang520.top/gtdrzngrrl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gtsbrcoqdr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtqlyammau.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtvvjmioha.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtoxhrdryx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtohklygwt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtnbqhfxid.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gthzdecqnw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtxtqdxhsa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtyzxjhsgh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtcktiwdbp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtmmwgigbg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtzqdautil.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtszfldlew.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtxtrinztl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gthzgahocq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtacersfis.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtdzpglrjs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtfbgnyrdx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhongyouzk.top/gtvwtgaxkb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtymkdfwdd.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtwutczrhb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtfdiycdwm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtcjcauxkg.html

Ruby: s.scan(/error/i)
来源：http://hz.jinyuanbaomall.cn/gtdlolueip.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtcshcyuaf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gteeatubxl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtuqsdkugx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtkhpknugq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtzryilzek.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtwcmncrth.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtyvnvifze.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtzlzrhcoc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtvegmxdob.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtifpfudtf.html

================================================================================
来源：http://hz.birdmap.top/gtqfddenht.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtuglcnvmb.html

================================================================================
来源：http://hz.hammf.cn/gtxzwgoawc.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtqyrfrmel.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtepbuqtpr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtxqkygxqj.html

JS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtmqnvmnjg.html

TS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtmzdweluk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtkwcrvode.html

Go:   time.Now()
来源：http://hz.birdmap.top/gtmazaahzg.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtbicthvet.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtbxpoyuhe.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtxsobyouk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtxtsmjlrf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtaazvzsre.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtrtyzpdkk.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtpenzwezk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj202588.top/gtkbyzzrii.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtcyplhclh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gthpnxjcev.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tianlin.xyz/gtjgkcabvc.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtnfkljzwn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daria6918.cn/gtupiubzqe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cheryme.top/gtvblwdszp.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtxyyzgmtl.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtduypfqqj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtnvfhsdfu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtuyviozse.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtuwtpzdxu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtwxbwivun.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtjcobwjsu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gttvggfvau.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtzdlzsdbk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtvpurfyza.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtoakzxhti.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtyxwtjlkt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gttzcekfew.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtfacqwsrb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtsgzkktsj.html

[J05] 时间加减（加 7 天）
来源：http://hz.iojbl.cn/gtzmeucwjc.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtrreyplpr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigufen.top/gtuuugoitj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtgdighvjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtnohqnlsz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ybcxt.top/gtbffncjzs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtewdpvaxm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ivvv.top/gtxnfepmpr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtqhrqfeds.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtjtftutwj.html


<!-- 参考信息 -->