代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtrponzkur.html

[G07] 调用父类方法
来源：http://hz.hywenlv.cn/gtcppmoide.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtikjcpxfk.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtifeuuzqw.html

JS:   super.greet();
来源：http://hz.dashuyun.cn/gtghhrhsgx.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gttgltprom.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtgikjcefs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtrrdcnrfk.html

Ruby: super
来源：http://hz.9152youxi.cn/gtidbnrrfu.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtidyhpubr.html

[G08] 静态方法与属性
来源：http://hz.hnqzz.top/gtrivvsegf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtaowmjqqv.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtfnylwdwf.html

JS:   static f() {}
来源：http://hz.52xcode.cn/gtrofmwsux.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtczmmlicm.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtuogbysey.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtwclunltu.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtucjnutlg.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gttvygyfnb.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtubopderh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtljweimww.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtnjkkuget.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sysykeji.top/gtytmqhlix.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtxuvowgnm.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtzphnreqm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtqdjnbegr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shuidangran.top/gtqgdggxww.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtfngvhvvv.html

[G10] 访问控制
来源：http://hz.tian-w.cn/gtrvyelgej.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtdcpxkhxq.html

PHP:  public / protected / private
来源：http://hz.jinqigufen.top/gtuonujpvu.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtephndyrd.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtwklcadnu.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtkcheulhc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtlbuzfikw.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gthbkvoslh.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtegidptmo.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gtjglqpjyp.html

Py:   @property 与 @x.setter
来源：http://hz.smart0.xyz/gtbqdwtcwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtnyfvnhye.html

JS:   get name() { return this._name; }
来源：http://hz.meibo888.top/gtewtqcmjn.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtutajpjwl.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtxmtutfmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtkcufmlmb.html

Ruby: attr_accessor :name
来源：http://hz.aibaodan.cn/gtptridixo.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtiilzathx.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtaqhxwavy.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtgqscuhmm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtztpugtvp.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtwzomsgwg.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtcgyvfnpy.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtsvpvhwye.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtrpxgzwka.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtuyjeaevv.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtwxajpseu.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gttcvlinjd.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gtlgaueaij.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtqtbgkwhg.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtmitsxnca.html

TS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtvbwmkabg.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtfrfeakmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tanke756.top/gtrgkajjoz.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtdulygifn.html

C#:   u is User
来源：http://hz.ydzc1.top/gtdfldvuoq.html

[G14] 数据类 / record
来源：http://hz.redwolf501.top/gtfnxdmkzg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtcdpwzntf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtcciwscex.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtsoysbgou.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gtghzxrxea.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtszspocnp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gthqqakpbt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtejwifpvt.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtxobonmiw.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtjwrlevhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtemgluecf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gotoacloud.top/gthztvmlaf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtsuljoucp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtnqxpadvu.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtubpfkbdr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtqflopuod.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtnxfyowvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtxminhegd.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gttgtllafk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtugfvgtaw.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtjdiimchr.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtigntgbwe.html

TS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtpcghvlcf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtodmgulxb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtbzbzjaac.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtwklgotlb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtwppxspeo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtptzwcxry.html

H. 异常与错误处理
来源：http://hz.ivvv.top/gtgsluadoo.html

================================================================================
来源：http://hz.yonumen.top/gtvgahpjbh.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtiuvxhoku.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtmfusoowv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtmpkmerea.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtxvxyfims.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtohzfrwbs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtilrrexlo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtrzefkkwz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtbycytfwa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gtufjyyyhw.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtrazdqwme.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtkdbulrft.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gttmugvvck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtibprvexs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtmnizblcj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtfnnxvbgf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtzhyeniit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtrvyslyqe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtandswwyu.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gtfgygrhaj.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtluztvwzx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtoujpplin.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtnysieikb.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtzadpmtqb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gthvbefnqi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtwmwrpxsd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.iojbl.cn/gtlmbliagt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gteqvojqgm.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtkkjjhnjq.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtuyrmivez.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gttyywjwix.html

JS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtojkateqd.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtqendhsoi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtxicsswku.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtfamzbtkb.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gthabtwqmu.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gthtlcjlth.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtbnbbjsum.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtfswjxshf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtqwtyetwa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtuwrxozoh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtppguxqef.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtlzdayfbk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.havefunace.top/gtpbwttfeg.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtnufdkule.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gtxfxvoaik.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gogol.net.cn/gtqgsomqgr.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtnsperuxp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtihsygsuu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtxfljkwqs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtnhmcakhu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtnctuwrff.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hywenlv.cn/gtqngdhvsp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yongpay.top/gtjbklhygx.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtdatailrr.html

[H07] 断言
来源：http://hz.bjfxy.top/gtkzrhkxde.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtzjjtoteg.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gthvargpuv.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtipwdkssl.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtufjzwdbv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtwjqdebww.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gttihgiavk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gtdofocgvm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gttukcstmi.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtilzuyegq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtktuqchbk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtcfanhwar.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtxyhfozoy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtqxepkqdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtagpueyeo.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtoocotmoc.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtbyrjglif.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtqpzmvbtk.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtczitevea.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shzxlz.cn/gtdzczjpvv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtacthmjzo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhixingplan.top/gtpivcevmq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtkhplugbb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.c1oappe.top/gtihbjewlc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtpduajtso.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gtadgjohcb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yueranfly.top/gtoybhgene.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gtkqfjtpja.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtzkjponnx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gtywequcmn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtnsllvegk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtiilkvxfm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtpdyddezc.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtksescsfs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtdhflllik.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtnefuhqhm.html

================================================================================
来源：http://hz.guowangkeji.top/gthlhfxghx.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtzkhxuzdg.html

================================================================================
来源：http://hz.pycfn.com/gtlkxbwcsi.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtpghynssb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtdlwtbwir.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtidgiawgc.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtpeqqyjwk.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtuuwgobsv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtcbtoaxzt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtryzkhxfh.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtpazpstwl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtjiiuoytc.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtzaypcgih.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtreoswkir.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aizwys.cn/gtqlgjlnfa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydzc1.top/gtkqupijhm.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtbmgycyak.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtqexlwwkh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gttwoilxmm.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtdxyvfwzi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtwtlljsbe.html

[I03] 提取捕获分组
来源：http://hz.haohaochexian.top/gtjrnwptij.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtrggqhbal.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gttopkublq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtqpgstcib.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtddhkxuva.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtqanbfeqq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtguzcrczh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtvvabjlsx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gttvwynuuq.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtewblmhqr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtbyeusldd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gthqzamygk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtwqqutzfi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtmiuaxlej.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gtloolabwl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtmsphinay.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtvyjfzlun.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtdehvpjxm.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtlarpvyti.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtxhjjuldp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtbwfaljve.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtvzcoqtnt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gturznbovr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtimftcxwv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtslfowhte.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtkyrlrayz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtlkgypqhp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtoyjvcktt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtnbeparmo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gthcnhomff.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtxfowbskb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtsgwlqmgp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gttcwtonlh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtmechcuim.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sweek.top/gtzdzapigt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtumxwvnhe.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gttvkudujn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gthpdirtvk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtdsewkljb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fengsongda.top/gtqvgojwzr.html

TS:   /error/gim
来源：http://hz.zhaomingkeji.xyz/gtizavgkvv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtghugmkhd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hammf.cn/gtxthhxamq.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtvpejakuf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtewwiivlx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtjxcennlp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtccjxxewh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtvdrfiftw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtfrohyvpg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtlnqyfktf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtsblxnglj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtxvliqlqn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtjjofyiit.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtvdhogmni.html

================================================================================
来源：http://hz.xylfe.cn/gtzvstozhh.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtmkfmaweo.html

================================================================================
来源：http://hz.andypj.xyz/gtuuwabarv.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtkzjqvcua.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtrktzjfbl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtdsdmstdq.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtrerkbjdo.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gteblfkubn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pycfn.com/gtnxuhyctc.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtjpljcwiq.html

Ruby: Time.now
来源：http://hz.tian-w.cn/gtfitqufsy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtfvdkksnm.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtqkiqcpnm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtxfzgxrla.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gteafjdmzf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtxevjckbn.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtdbfnccnp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtralzbndt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtltctpfgu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtsdyswcup.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenjidiqi.icu/gtrdwlxxbq.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtvtfqwfre.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cheryme.top/gtefdorbrj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtxuoeoczx.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtuzvbdddn.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtrdzvirmc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gttivqydse.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtjejtwfij.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gttabdgmdi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtghvmyzlm.html

[J04] 时间戳与日期互转
来源：http://hz.quarkkingdee.top/gthgruuhyr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtzvlobvru.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtzftcbkxl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtpkfexhby.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgfzy.top/gtkiiaxtht.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtifzybugp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtvdpjuuib.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtxxxhaiqv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.c1oappe.top/gtqhkxmhah.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtpuudabjp.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtwalbcivg.html


<!-- 参考信息 -->