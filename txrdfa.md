代发 wailian999

Ruby: super
来源：http://hz.hammf.cn/gtnjsyczfz.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gttamwstgq.html

[G08] 静态方法与属性
来源：http://hz.yuanzhike.top/gtwavatpvp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtklrgillw.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtsymcamlx.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtmsxydftp.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtmjibmnuj.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtpdtmontv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gtjzcmeqdp.html

Ruby: def self.f; end
来源：http://hz.jqgfzy.top/gtzlnxokez.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gtwkfvsrvg.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtwrgnwfvi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtpyvjflfq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtbwgmtwyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258888.top/gtpniboqpz.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtisgdrddq.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtaxdddpsd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtjomurgxp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtrfrdvbzj.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtgxsowdrg.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtorrlrujr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258888.top/gtdnjnpjbm.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtlacnxjfi.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtwrqjyamy.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtwepauuqa.html

Java: public / protected / private / 默认包级
来源：http://hz.xingfuxueyuan.xyz/gtxnedpzas.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuanzx.com/gtsypehigg.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtdabpmock.html

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gttdjltchx.html

[G11] getter / setter
来源：http://hz.gotoacloud.top/gtspeftagl.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtujgxlsae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtrzgiixxk.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtqnrixmyk.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtwmfznnce.html

Java: public String getName() { return name; }
来源：http://hz.jiagoushi.top/gtxchfvzce.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtqbfarveg.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtmbqkdsdg.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtmcyjjlnx.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtuckejcbh.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtpnroaayp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtvkjsgodf.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gthztfhqey.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtmgkqrmba.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtvbajjtew.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtzikqiuvj.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtrtllknss.html

C#:   public override string ToString() => Name;
来源：http://hz.shangyingyoupin.top/gtrqdrjetb.html

[G13] 判断对象类型
来源：http://hz.meibo888.top/gtnwolpmem.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gttqldhavf.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtxjdekwux.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtxgxiwimr.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtmkwbeocu.html

Java: u instanceof User
来源：http://hz.gogol.net.cn/gtxhxsmiin.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gtvjylljmx.html

Ruby: u.is_a?(User)
来源：http://hz.cucudq.cn/gtnfbjzqhc.html

C#:   u is User
来源：http://hz.yvedp.cn/gtziuvoepe.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtshfiqaep.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtbwdqkglh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtgljxzhqh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258888.top/gttktyongx.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtlqvbwttf.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtyaaewjox.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtoejecykr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtibskkhda.html

C#:   record User(string Name, int Age);
来源：http://hz.yongpay.top/gtcdsixvvb.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtlxzjfyha.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtntxrclji.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtbdpwbvba.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gtbcqmucyj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtumsvhqyc.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtkyadobmv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtppegbsla.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtsouyuazm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtwkapkbme.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtoqmfinho.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gttzlppwnb.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtsmvhjglz.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtaqquwxhs.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtvarreyvz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtkwfbzfqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtlvxipyoa.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtasgowclq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtmwqojnhs.html

================================================================================
来源：http://hz.ehwqpu.com/gtgmerunxq.html

H. 异常与错误处理
来源：http://hz.52xcode.cn/gtvjuirojl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gttrogyuys.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtprsrhfrh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtwoxlywom.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtmudignjv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtuomwqiap.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtvjfmpylf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fzhhl.top/gtmsgseufg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtxavrijff.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtahyihzkl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtilkakarb.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtrqhtzjai.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtckwzcgxu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtrypqanrc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtysqbpmfh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtlxlpbujx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtejmqnlgg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtxpisgggm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtwisccqec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.316326.xyz/gtgwmvfebf.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtbfdrvfgl.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtextyuhdi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtiprkujef.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtpgwhpkgj.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtvixznagr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gturaoouqm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtpovxjarf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtqqxskson.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtlkhnufrc.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtjkoefkni.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gthwqibtpg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtuikcxmzb.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtjkreeyiw.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtwxvwnbix.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gteivjbdde.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yvedp.cn/gthxpjvadh.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtbmhehgev.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtetdqjncc.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtidfxvpzf.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtjddztwgb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.bjfxy.top/gtnuafvkor.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtisumxtdz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtqinzufjj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtdsuasnwt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtrsruzslk.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtxddyguis.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtxyefequv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydzc1.top/gteqlxdqtg.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtfpxmudzz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cheryme.top/gtpoisddjc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtdmzyqyqp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtnjapofdy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtfjcgjqwn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtdwrvoylb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtpxnejdrn.html

C#:   obj?.A?.B ?? default
来源：http://hz.fengsongda.top/gtsbdzwtzd.html

[H07] 断言
来源：http://hz.nwbrower.top/gtpoigevep.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtilejmtdp.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtjdserzka.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtyrdovvax.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtxukyfkqp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtdmvwukne.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtnuuwqdzj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtddqybmif.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hywenlv.cn/gtervregul.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gtnqlhxwbi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtgzuthwmy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hysaishi.cn/gtuigdwwnh.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gteqtwxrld.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhoulong.xyz/gtrwninrhy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtucppdsoa.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtzsacxfqo.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtktpunwgx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xinyue.icu/gtemgizidw.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtbbhoepbx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gteaiipvwg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtwaxhmbva.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtdehbkxbz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtnacbbbhx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtlignhdpr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtrpujdaro.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.pycfn.com/gtpaigqkbk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtwsebubgw.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtbwkewcll.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtqcupkvkv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shzxlz.cn/gttibyjetz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtoiajknxl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtwqhrhvad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cashguo.top/gttnnhidcd.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtlvlwwwsb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gthjcjjsfy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuanzhike.top/gtlchgjegz.html

================================================================================
来源：http://hz.gotoacloud.top/gtxfgarbjz.html

I. 正则表达式
来源：http://hz.zhijiandao.cn/gteanrflmg.html

================================================================================
来源：http://hz.xuanzx.com/gtgoiyyhke.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtqdfizcju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtfzvprgvt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gtfnfpvhmc.html

JS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtvekstarn.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtytlnneij.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtgzwdqhoe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtvnuhxvbo.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gttucfjuav.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtzeuoxblq.html

[I02] 提取所有匹配
来源：http://hz.hammf.cn/gtuiphccux.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtstaygtwr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtbdciehto.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtdwdffipe.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtgscmqmhb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtfaxgaufd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtjuuoqely.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtkiubagzg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtyuvxeqty.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtyykevpsh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aibaodan.cn/gtytjwmwtv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtvjubicta.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtlqrpgvxa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtxnharofn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtlkbnpmdu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtjovqbedo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtotrcutqm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gttsgegeon.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtjcsdfqzq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtcrhucyzz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtcpjbawij.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtwcrdqcde.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtnancigcq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtyknctsld.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtorjwxhcf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtonjwlmcw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtkslvgogn.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gthzjamrhg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtpxzvcnii.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtxzaupjbc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtsbbizsvj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtrijxhvph.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtrioubmgi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ehwqpu.com/gtdbwovnoa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtguvccpxi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtugjuhzqb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtrmrdgcha.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtugwkrcwu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gtrzedmkfp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtadhtjmfw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gttembtxsf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtdswutcrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtygfinobp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gttfifcsml.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtwqbmjdws.html

[I07] 忽略大小写与多行模式
来源：http://hz.yongpay.top/gtxqcivuoi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtnsiflesk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtntccixux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtmjbmriqm.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtikepdyzf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gteheycdhy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fzhhl.top/gtfrgoshbx.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgufenzy.top/gtwzdsszhu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuxming.cn/gttgxxijhc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtmfevgrvf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gttiesffkq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtqsaizjxn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtfadloubw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtkhlkrwgf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtymqirgay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtosbfrgcs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtabhuwtxu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gttjjrfjis.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtfrzyihvk.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtkcffvwgn.html

================================================================================
来源：http://hz.ppjwa.cn/gtuzweyzgj.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtxxlomilv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtquzcgfan.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtbbrgvqfs.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtovbhgvhm.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gttexfuwux.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.52xcode.cn/gthpillepu.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtxpvbkhli.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtbjjtnjby.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtcfxwvnjw.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtkqztmrpl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtyohkvgey.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtubooqkqd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtbbyjagrn.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtpuhbpmth.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ivvv.top/gtxsgerqvu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtjallxbsk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtfthegylg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtcalbedps.html

[J03] 字符串解析为日期
来源：http://hz.zhongyouzk.top/gtynpalwoe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtllepphzo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daxiang520.top/gtuvbsxhbb.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtbxukshek.html

TS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtmesslsnv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtupiomoqe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jyoumei.cn/gtskcrdaky.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtunihgihc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtgklcoiib.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtexpgkvxx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtkmkrhtqk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj202588.top/gtpkujatxa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtzmhzluno.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtkengeuha.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtvzhheepq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gthkgvxkqk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgfzy.top/gtyefzvgou.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cdnleiting.top/gtsmvrxozw.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtefmexkyr.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtjwloddvj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gtbyrtkodl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtznqwlvsb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtljcngcqv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dianchejie.cn/gtiphkffqh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gtpsrstgrm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.birdmap.top/gtiuykuwpt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtgdyiyyym.html

[J06] 计算两时间之差
来源：http://hz.ehwqpu.com/gtneywcnwp.html


<!-- 参考信息 -->