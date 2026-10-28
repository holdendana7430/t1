代发 wailian999

[G06] 重写方法
来源：http://hz.yj20258.top/gthaqddnyy.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtlaqkpvqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtncyvttdf.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtpjjndolw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtuafjmcwl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtfhelepfl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtyqtllgwl.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtsetkvnqu.html

C#:   public override string Greet() => "admin";
来源：http://hz.birdmap.top/gtbtozfuqo.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtzdrwhakl.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtyezqekxc.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gtsxffjzwe.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtdcutvrec.html

TS:   super.greet();
来源：http://hz.jinqigfzy.top/gtmsrrwnha.html

Java: super.greet();
来源：http://hz.sweek.top/gtlndpmjhu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhengqikj.top/gtwsclckbx.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtqrbhisos.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtcepgovgk.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gtjwytzvqz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gtqmfevpxe.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtrdktjpbp.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gtwhcrtwlt.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtvqxuazyd.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtnqyfxugj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtswaekcwl.html

Ruby: def self.f; end
来源：http://hz.jinqigfzy.top/gtdskupuot.html

C#:   public static void F() {}
来源：http://hz.daria6918.cn/gtciywdavu.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtejmsxgij.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtybcabmbo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gtjhuizoft.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtudlijqen.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnqzz.top/gtqfikoqit.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtrblrjxiw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtnrwbkfip.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtvopelkeg.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtljqtamrc.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtglrtcdwd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gturfdkxhb.html

PHP:  public / protected / private
来源：http://hz.yj202588.top/gtytueglrc.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtwimfbeex.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtnuqmhhqo.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtpbxtehxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.mhx1999.top/gtgrztugos.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtlkxsdlxa.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtyjodqjnz.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtcshewuvm.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gtwccrgwax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtehcqzfdh.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtzkcslmhm.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gttwpbbydu.html

Java: public String getName() { return name; }
来源：http://hz.ydzc1.top/gtlgsshhwe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tanke756.top/gtgaljswno.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gtnedxclwl.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtlgcuhynb.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtmxasdpdw.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtaclndrty.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtadalvkxo.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gttsbeenjq.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gthuapnobd.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtqxpoelnn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtdoiqhpmv.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtsdjmkmpj.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gttqholckx.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtoduhyjkw.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gthmiimxwd.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtumbfgqws.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtbvblabsc.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtxixibwaa.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtrbgisjbo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtxdemtbbp.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtxchcxueg.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtxndvhyaz.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtchlhrcsj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtwzinkcqr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtskscijig.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtcbglekmg.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtmfuhwxen.html

Java: record User(String name, int age) {}
来源：http://hz.tanke756.top/gtflgdccin.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtiocllzzn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.haohaochexian.top/gtuzyaqabm.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtvjejnnoc.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtlovjrsaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtjdwtmghs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtumvmrrff.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtwsfzvnof.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtagahsgwg.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtacjydekm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtnxgaklyz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtehxvqqix.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtovlmqnok.html

[G16] 对象转数组 / 字典
来源：http://hz.redwolf501.top/gtpatydwmw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtwmggrhpe.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtgmjtcijw.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtghxjfzsl.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtspkhidcn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtchmlmmwx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtyibwxqnn.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gtdqbaeazy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtddcsfvby.html

================================================================================
来源：http://hz.jiagoushi.top/gtfeeagdob.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtxbnvklhq.html

================================================================================
来源：http://hz.yj202588.top/gtztzqiemd.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtmrjpzzjz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtnigcihzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangdashe.top/gtiagfcala.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtfthdtvky.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtwuntiegb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtzotzdwvh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtahyyiiwy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.meibo888.top/gtlhxiueoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gtuatemeuk.html

[H02] finally / ensure 收尾
来源：http://hz.jinghuilouyu.cn/gtbcgxyygp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydjk.org.cn/gtdguntugg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtqwhdlllm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtdmrygnrd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtwtqieitn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtzmmrgkdz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtnkvaqmbx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhengqikj.top/gtdomaqkhh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gttefwedzc.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtbwuaryxc.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtrkralkag.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtrgyltvkn.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtqpruqnjg.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtzydppvsu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtmtlleydx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtkjidcvzi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangdashe.top/gtmmkqdrnf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtwplrohqs.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangkeji.top/gttbdsrtcp.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtyxxyflkb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtrnhtsgns.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtxxoqywln.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtiredkale.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gtsbozmhdv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtlpkxmyil.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtfwbklhwk.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gterchqwur.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtmrmtumdh.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtedsubhya.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhaomingkeji.xyz/gtzpjsromp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtzmqkkrod.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtrdsvbaif.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtrrapgtrt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenzaomai.com/gtodzwxzpu.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gttxajufai.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtcqmqwqfa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtvboarkzb.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gtppbaflke.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtbaanwyzw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtvvljuowp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtffyjgqzt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shuidangran.top/gtptzigxcn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtzyngtlfq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtybbozqhv.html

C#:   obj?.A?.B ?? default
来源：http://hz.zdqjudy.top/gtyrsamspo.html

[H07] 断言
来源：http://hz.xinyue.icu/gtfbgctdpj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtqnlelwde.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtdgjtgxuj.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtfhyvqrda.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtztgkstss.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gtbklfubuy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtxizijqtr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gtffbhncgk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtueufctis.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gtgvvitytd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daria6918.cn/gtawggwero.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtpzhbypnd.html

JS:   e.message;  e.stack
来源：http://hz.ydjk.org.cn/gtwsrczgvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtejdxohjj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gturixtyuw.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtascazzld.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtnpnoswwo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yueranfly.top/gtfrycyrdu.html

[H09] 带错误码的异常
来源：http://hz.hfpthk.cn/gtdatftsoi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guannengcc.top/gtvafqszgi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gtquvkrxio.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gthzoyzics.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtraafafho.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtylpxdqvw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuetiantiany.cn/gtksaqfpwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtyzhcfelp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtemqkplxc.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtlzgzfvib.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtzqcsyouw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtxyngwtac.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtjnysqsvp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtcscoqokw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cashguo.top/gtgntgkaiw.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gttfjowfpt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtrpyexxci.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtreraelnx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkjzewxqp.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtglrqdfpb.html

================================================================================
来源：http://hz.316326.xyz/gtqgnfzpcd.html

[I01] 判断是否匹配
来源：http://hz.xuanzx.com/gtfewzzjtt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtwqejfcef.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtopidxctc.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtuubpbbmd.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtbwveahsc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtaczipuqo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtiscutcsk.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtqjfqbudj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtgckhujvr.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtvmnunrew.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gtorejwzfn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtytdtrssa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.iojbl.cn/gtzegbndzl.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtiqsywulr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.bjfxy.top/gtkdknasan.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtrdybtyja.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtcrqdobgr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gtslqhgcad.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtvrxvnntt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gthidmqozv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtqcswzciz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tianlin.xyz/gtajfovmbs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtuhybvhyw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gtxpduszxl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.bjfxy.top/gtdyirmdjh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigfzy.top/gtrroqvpyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtaohbctad.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtqdfggydc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtificywei.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtqvjzkxhn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtqajpubeo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gttlcrsmtd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtpdwcqiwx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtphypqrkp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtkkllpqng.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtfufsbqqq.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtsjiitota.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jyoumei.cn/gtnmoyqlsf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinyuanbaomall.cn/gtmgfytsvj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtqbxgupzj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtpvdcimqe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtidecvqwg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtztuxfzfe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtbxidcroa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gttimqcgpd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtuuyiunqu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtmprmpvms.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gtaylyctbx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtuqzctfuo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtvtkrrwnx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtfskbdlwh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtwbtuchnk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtbpecqxrf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtvgxxbzmp.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtcfwhtpbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtahksnrhc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gteolzfngc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gogol.net.cn/gtrljsxdrc.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtmzhhfigd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtrspfcvic.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtfzokcntq.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtmazpvxwe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtrsjzwdmq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtqeliiuwf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gthfkbqgap.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtrzscanju.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtfkyunavg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtbgaoylsk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtqlgjtdbd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangkeji.top/gtdevwskdl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtqgpuxigb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gtcozwpkpd.html

================================================================================
来源：http://hz.meibo888.top/gtvkwhzzje.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gthxxzucea.html

================================================================================
来源：http://hz.daxiang520.top/gtvshjdurk.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtywdipeea.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtckvjigdf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtivzyfadp.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtafnnrnys.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtbgowyiay.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hysaishi.cn/gtltrzseqh.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtodhnwhbv.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtajawheak.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtbupawvxb.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtirxivtke.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtcrjxjfoq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtfgsnixyf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtvgabuigv.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtgynxfrjr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtofgkbwes.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtgxirnzwm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtpioatafy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtavmeyyjc.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtnjaduedj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtmkutyihz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gttnodbujg.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtnzcqzlul.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtyfhvrrru.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtkxdppiyb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydjk.org.cn/gtlgslksrc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtbdzkzxdx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gttiijziqk.html

[J04] 时间戳与日期互转
来源：http://hz.nanxinkj.top/gthlithxsa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtqfgxhqln.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtnskaolhh.html


<!-- 参考信息 -->