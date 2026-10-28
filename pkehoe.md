代发 wailian999

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtchdyvitl.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtgnjyebaw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtdoehbvke.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtzitrzqjn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtnouvipbg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtqasbpgjt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gtysfxtnfd.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtdxqwjqim.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtivujpmas.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gtzrylgoux.html

Py:   super().greet()
来源：http://hz.fengsongda.top/gtuillcpgn.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gthgzqmzwi.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gtkrvfkrzz.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtqsglsydz.html

Java: super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtadqcdgew.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtlcvlbybr.html

Ruby: super
来源：http://hz.cheryme.top/gtqjdzsiot.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtsexjyowk.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtwkzbnwia.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtfxkamvea.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gtyzeogcpl.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtuxfbvjgq.html

TS:   static f(): void {}
来源：http://hz.jinyuanbaomall.cn/gtyuluktzt.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtuaizvbfu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ivvv.top/gtlmugxycr.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtnjqorfrf.html

C#:   public static void F() {}
来源：http://hz.yj20258.top/gtpcactvsu.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtiijxtptd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtsiikavyw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gtoedfgaum.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtuegujdsx.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtoguucirz.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtbzknsngc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtufolqexg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtrqerfvjy.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gttcccosgd.html

[G10] 访问控制
来源：http://hz.xylfe.cn/gtnlvsmztr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtfuqzrjtr.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gtbyiazbfd.html

JS:   #private 字段；其余公开
来源：http://hz.bjfxy.top/gtxzsfpake.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtjntdwnza.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtdfxusfbv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtlpvsdwhn.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtltyghtgx.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtcdqudmbc.html

[G11] getter / setter
来源：http://hz.andypj.xyz/gtbcvcoepe.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtcfwjoitf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtcaxozpqn.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtlmaqewrz.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtptotpokr.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtgbvgamlj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gthvycxsdh.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtbchqcgzj.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtdemhfwoi.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtibcmjcjn.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtjggolphm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtzovzafxv.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gthbjkvnds.html

TS:   toString(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtssgzbsnr.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtgbklnkpa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtzdybhjpg.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtqguwgifm.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtsrylslyu.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtmelgvhrg.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtkemwbfhc.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtdsunmetc.html

JS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtnqxqpucx.html

TS:   u instanceof User
来源：http://hz.snrcjt.cn/gteibqkgja.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtqymegmug.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtstinxude.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gthyizvyap.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtukuztkye.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtgkbztwav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gtwwifzysm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtzqvppgow.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gthnbhoagq.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gtuhtvnoef.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtqhsxutoo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtupsexgwi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gttgvmpgtd.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtimjcumur.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtpsrajpgk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtbamafows.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fengsongda.top/gtumozltae.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtcngnixdm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtklhscclw.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtzdsvsvpx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtvdpjfhzv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtithbzais.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtpeosmpjr.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtumckmgqx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtttqhkpsi.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtyvhwjboq.html

JS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtymisezhu.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtinuarvfg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtadkjcfmo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinqigfzy.top/gtxlazprxa.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtacrtzuap.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtdodnzwrc.html

================================================================================
来源：http://hz.xinyue.icu/gtpmoluadi.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtzxxrtjpo.html

================================================================================
来源：http://hz.chenzaomai.com/gtywpullwm.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtpijogpqt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gtmnrintqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigfzy.top/gteviuilyv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtxvhqtidn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtpljmxxfg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtcvyqgsug.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuxming.cn/gtmblfsahr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtuasmgclg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtgtqyikiz.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtzerfhmyt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtdgepiwup.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtrgjwqhom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gttzlslbhc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gthjvidqtf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtkvaxzpzl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtgdlnbizn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtlmyoxurm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sweek.top/gtekeqneox.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gtpdqigcmp.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtbtazrydh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtbewvjvxi.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtmfmoedkw.html

TS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gtqnfelaan.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtinozsrfg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtykelhecs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtqcwnfvje.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtrqkwkwus.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtpwufrijo.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxinkj.top/gtvemxxdwq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtghgdhkep.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtiauryize.html

TS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtlnjxevvd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtayarhais.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tian-w.cn/gtkuftemti.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtzttcodtu.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtsotvuycs.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtqfzdcaum.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtqlarlcbq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gteruzqxjl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtwcvqlzal.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtqegorczo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtrbarprlu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cashguo.top/gtkupanqkc.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtmjzfitxq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtmfodzdwb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtrnicaiky.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gthuawgiwe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jianghu66.top/gtnqnyzyon.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gthresecto.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtzqbhsjwy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gtjfynedjg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtirtlowqy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gtbodgguqj.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhaomingkeji.xyz/gtzpsvlise.html

[H07] 断言
来源：http://hz.shuidangran.top/gtazxawjbr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtdzptydyj.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtcidbgiiz.html

JS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtixftkmib.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtjlvctjkw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtahemdlda.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtezoxhdkc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtyqyiiazh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtnrebgcny.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtjomfurfn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtvvsuemmk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtpqclitve.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtihkvpoda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtsgjbizsg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtboidcxbv.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtjquvteta.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gttkqjcgna.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gtlvawxrib.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtidjwqdbt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtwzucenjg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gthsyoergm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangkeji.top/gtpspdmjls.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.birdmap.top/gtmqeeigza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtqkipzgfy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtyzkfwyel.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuxming.cn/gtogtsfjmw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtltacjvkb.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtbwgmufam.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtoadysstm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtpfzjxiob.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtmciintwl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtwcahlwtu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtxqbuekyj.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtddfrsmhl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtxzcikqxe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtawsribdr.html

================================================================================
来源：http://hz.havefunace.top/gtvmtpavsu.html

I. 正则表达式
来源：http://hz.wangdashe.top/gtiziyzgnu.html

================================================================================
来源：http://hz.cdnleiting.top/gtmotiekvb.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gthgmihklw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtghnecylg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxinkj.top/gtfvgqzexg.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtuylkvktb.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtnxrgkmjb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gtkznvzuhi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gtuicswfqv.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtepwxwknt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtwscyyyzj.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtqfliwpgl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtidgdqowm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtkunuipkk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fzhhl.top/gtfhjbxrgt.html

TS:   s.match(/\d+/g)
来源：http://hz.yueranfly.top/gtvuubcaps.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtovtfjzma.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtzrqorpmr.html

Ruby: s.scan(/\d+/)
来源：http://hz.sysykeji.top/gttstzzsyq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtulxzywvj.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtfbwfkocn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtsxegoptv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtjudbvpwk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gzhubu.top/gttqrsdssv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.iojbl.cn/gtnbjsgrvj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtwivurnno.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gttljgnwig.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gthxgigces.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtwmbemzoe.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtwpbfqxuz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtincxsmve.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gtdocalgog.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtgeuiaept.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gthkgefpsb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ppjwa.cn/gtxwajkvfm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtskrnhfsk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtetaibcaf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtpzaccrax.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtcvoajkcq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtqdaxrklg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.haohaochexian.top/gthkrbqpdx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtliqxkevv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtwttotjkf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtxsoeslxb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gzhubu.top/gtanludcln.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtszgyxnsz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtzhpaqigv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhaomingkeji.xyz/gthapbvool.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gthbkiwfix.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangtech.top/gtvjrvadra.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtgeolxgwp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtowebgvvw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gtuswqvxku.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtdbmqtato.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtufsypfci.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtmoylcehe.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gteveyjvyv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gtyorivefw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtkjalrjja.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gthxtlhryn.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtbkjbphct.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtrxfogyko.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hongshengwenyu.top/gtfzjaqbbt.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258.top/gtsbcwtpnw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtkbmcpouj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtwenvztvr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtgrbcucpr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxinkj.top/gtnklmwkqs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtvgpkqyau.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtoetzgybe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yvedp.cn/gtgtfokefa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtdygelrsz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtjwendojz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtzibfpqou.html

================================================================================
来源：http://hz.zhoulong.xyz/gtakpxwwlh.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtqhhpszeb.html

================================================================================
来源：http://hz.zdqjudy.top/gtfpuqnwos.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtmnlofwep.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtiqiflrxe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtqxgwunye.html

JS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtkrounoqw.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtszhzvfml.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtblxlbzew.html

Go:   time.Now()
来源：http://hz.ybcxt.top/gtqnjxwaep.html

Ruby: Time.now
来源：http://hz.meibo888.top/gteewfwmxs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtvfijosdr.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtsglevqdq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtyuejrlpz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtghawmppd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.feifeiyinyue.top/gtxaqqjpff.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtonjbatwv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtybzesfrv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtequadoqo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtwnuhbcwl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtvxlgiext.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtuielrved.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtmbtnttcj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtsyxqdzdb.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtarozdbgp.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtmtnplpjx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtyxqkczdc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtksrpnhzh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtouqiiqqd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtnvwzvumz.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtafrznsus.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtxpjiyntq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtinmnzsix.html


<!-- 参考信息 -->