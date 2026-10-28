代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtksspnril.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtkqmhzjcg.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtwaaetygf.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtqgnrcqiw.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtzpeppjwz.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtsziwfjoj.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtudgpztfu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangkeji.top/gtgrkhbssz.html

Ruby: super
来源：http://hz.nwbrower.top/gtrayhcvai.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtwbsybtqe.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtuyyivtvh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtoamzsuls.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtbshpuogd.html

JS:   static f() {}
来源：http://hz.sysykeji.top/gtnyhspjsw.html

TS:   static f(): void {}
来源：http://hz.tianlin.xyz/gtezwdhvkl.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gtgcbglhzz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ywan-chungtsiang.top/gtlaldqgob.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtackxrugs.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gttgkqipho.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtacnefawy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtojarhoui.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtopqlixyu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gzhubu.top/gtuhafgcvn.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtlzwndatm.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtjbvxmtat.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtgmejkceq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gtodxryxor.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtcduxvlmv.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtxzrthgdr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtqudqutfr.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gtnunrwoxd.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtjgcowefv.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtsasyiqct.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtcxynypzu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtecuusfer.html

Ruby: public / protected / private
来源：http://hz.gaohongyu789.top/gtkpmenile.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtmsbvfkbg.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtuigfyozv.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtwddyhpvv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtytgdjpcg.html

JS:   get name() { return this._name; }
来源：http://hz.svipenyu.cn/gtxoofpvtb.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtnipxaput.html

Java: public String getName() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtdjxinpti.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtdxmqsvys.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtoqfwdqhh.html

C#:   public string Name { get; set; }
来源：http://hz.mhx1999.top/gtdsjrlxgi.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtkqvycyqd.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtmizgqcoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gteddkevbf.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtropewaif.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtbuhbknbv.html

Java: @Override public String toString() { return name; }
来源：http://hz.aibaodan.cn/gtjaddnngm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtpyuuywmv.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtxmieygmz.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gteftpkjdq.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtoolkzrxr.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtpfdpwmww.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gtbsewrxre.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtopvaxdje.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtwrpfjgyr.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gtznnuxsmp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtwnysihjw.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtbsohlawz.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtjqqgwcvt.html

[G14] 数据类 / record
来源：http://hz.yongpay.top/gtkawyravd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtdeeroahz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtewlhgjxl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtuiefnotx.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtodmddcbs.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtunxuttmk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtpcqedzbd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtrlyorvvf.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtqlyrxloz.html

[G15] 枚举
来源：http://hz.tanke756.top/gtdzldhaol.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtvlvepfdw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtmttcwegu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxuanxn.top/gtneuuwsfe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtkuqzgjdm.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtjgmipyuy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtbuxrconq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gttcufjukq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtfnnghwld.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtjkmctxzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtyxnoggpe.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtbkgvkelf.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtxpishvtu.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtvgmadylm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtxpwkteow.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtnnkmzimd.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtzfetiaib.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtpumrkvty.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzgpygtpm.html

H. 异常与错误处理
来源：http://hz.xylfe.cn/gtvuzmgdvh.html

================================================================================
来源：http://hz.chenlongwang.top/gtqfnbxaqj.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtdehfwyqr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtpyvxamyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtubddnwcu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtepshlggf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gotoacloud.top/gtxetexuii.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gthuoiqajt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtfvjmgqrt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gthnyuziee.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.feifeiyinyue.top/gtndccotzo.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtnalsmsui.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gthbunrtom.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtcoltvglv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtggmstape.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtifegjura.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtwzauowfh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gttbwcqjin.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtiazmripn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtdlekmdfs.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtvrbtktbf.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtxyzjjfci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtcyzdbsmr.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtpqknezjz.html

TS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtrdoynjgf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtfembokkg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gthqojzmzg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cheryme.top/gtpscanldy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtelhjlnzo.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtrtyycaag.html

Py:   class MyError(Exception): pass
来源：http://hz.yuanzhike.top/gtxvabhchz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtqtrqkekx.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtvwdecaot.html

TS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gttevkrluz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtivheqfys.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gttfxvyrse.html

Ruby: class MyError < StandardError; end
来源：http://hz.jiagoushi.top/gttnbkhzqu.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtxpaqhblb.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtdqesnelj.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtbzwhpxlm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yvedp.cn/gtumpjiurs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtmfhvjrvl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtkhqtfwad.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtjxsqnsgt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtdoqslxae.html

Ruby: rescue ArgumentError => e
来源：http://hz.jyoumei.cn/gtdalmgovc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cheryme.top/gtnklelxxi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtzcleqhrf.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtkbsegcxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gturzavaey.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtebjrzlhf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gteknlkzls.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtwequtixe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yangfankeji.com/gteoqamozq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dashuyun.cn/gtflarknel.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtjfhrngco.html

[H07] 断言
来源：http://hz.sweek.top/gttocjamef.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtshcxlvqy.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtfagknjqx.html

JS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtrlpjgvcq.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtxysrtzvi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtvjnncuds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtszrskirt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gtpnzeissv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtaaufppve.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtznrwhkfm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtvtetecck.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtckweqgdw.html

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtoqivosqu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yangfankeji.com/gtrjlzavmc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtmokvtalz.html

Go:   err.Error()
来源：http://hz.cdnleiting.top/gtbhvzwikg.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtmacdeigg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtajngujuo.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtdirddqun.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gthceptoyq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtijkkirli.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gthjlginca.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtqwuwtecm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtlbwzxyfj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinghuilouyu.cn/gtuowfrsco.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtxifbmwxx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gtiedggzvo.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtqohixmil.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtadmpccsx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtyxrxzwmw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gthzytmowi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gteyzixdgi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtcooagghs.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtnlpuvoqm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtslyxrerl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtvggbuntf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtucfoerhn.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtdqrcwcte.html

================================================================================
来源：http://hz.jinqigufen.top/gtysqzvspy.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtbqzqtygb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtdsjmngas.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtqfwjqycy.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtyyzxshaf.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtkvhumifd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtyprgyctk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtmuuaalle.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtzojbtwky.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guannengcc.top/gtamkqzpvf.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtpjsxhzop.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtaftmoeij.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtdwlbuceo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtcdpugqlr.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtauccwrkj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtnegxvyee.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtjompldmg.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtxabsxwon.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gtkngqloqp.html

[I03] 提取捕获分组
来源：http://hz.yuxming.cn/gtdyhvawrd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtyuptfruw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gtksclfjui.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gtllzikvlf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtoxenozyb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtinvpkivp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtmqwbiscd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnxiangtu.top/gtmxlgvcko.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtqgfpklgv.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gtbwtgwgmf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtvkyxfdxx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtnygtjinu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtdlidwvql.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtvzmfmtut.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtibdeotul.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtzwpzpnee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtprqggbbv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtivppuadi.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtesibjthx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenzaomai.com/gttebhpied.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gtvdxxeegs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtagtrpdat.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtenzrgolh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtuqrntnzk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhoulong.xyz/gtzqyffdhu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtbnxigjab.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtyfvrbkve.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtmljumipl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gttpbvjwmf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtkmfwtcya.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtxncxqjza.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtsknqwvsj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtcbdzjzld.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtcbvyglde.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtldmmojuq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtbsxtnctx.html

[I07] 忽略大小写与多行模式
来源：http://hz.andypj.xyz/gtbrekeovz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtkpikqioi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydzc1.top/gtvudsfufb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtbbetcifj.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtzmylmiku.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gthrncfakf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtdiysypaf.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gthijpfafp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gtsocrzxbr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtqulryruo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gthksbsmht.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtlnnvnlyg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtcawyazfc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtsazbexbs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtzmzzjypl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtxfkbqbur.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtmtlklzbl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtypyfpnzn.html

================================================================================
来源：http://hz.gogol.net.cn/gtctkjljct.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtptsolifs.html

================================================================================
来源：http://hz.shzxlz.cn/gtbiignubq.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtltblwtyv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtxkoamzyi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtgehqdlzz.html

JS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtwumqnxci.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtnndcqrjq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtbxocemlm.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtvipbuhpt.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtbzqwayus.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtsyfujjgx.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtuqlbcxbp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtfkyqtpkd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtntrrngiy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtceczteri.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtkqbhywah.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj202588.top/gtayyllzzf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gtwkwvmukq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtpontpzqf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtdyvjdqft.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtkszzjkdp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtcxtvoldj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtafhbtpqw.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtadutbzia.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtqtylkmft.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtxcybtkgi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtjesktyoa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtvqubdmgb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gaohongyu789.top/gtoponxtfo.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtjauxadoe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gtpzlrhrvd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtqcpjtyxg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gtffezajne.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtxmezplgx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtijkgmpxh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.birdmap.top/gtqyhdkhpy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangkeji.top/gthnelajeb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gthjchoxgo.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtmtthmpcz.html

Py:   now + timedelta(days=7)
来源：http://hz.zhongyouzk.top/gttycaxpcm.html


<!-- 参考信息 -->