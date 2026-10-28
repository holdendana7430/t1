代发 wailian999

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtssnrtzpw.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtxjjntmek.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtsawzposi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtwvqdhgxr.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gthleslrug.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtbvgaokbu.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gtviwjihne.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtciivwjmb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtfijtehab.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtwzevgfsp.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtgywjnzap.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtcuqcvnsh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtpflqyyrd.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gthrwxgokx.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtzwuyshsj.html

[G05] 继承
来源：http://hz.hnqzz.top/gtlohbpwxu.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gtcynkahal.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtqsubjywn.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtbgcpfrrq.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtedpxtnnk.html

Java: class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcrxpocls.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtjdeuesvn.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtlphomlcq.html

C#:   class Admin : User {}
来源：http://hz.gaohongyu789.top/gteewgxkzn.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtrqatqswt.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtvzedrctd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtiqudbyxr.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtklidqezo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtfvmmhdht.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtztecveed.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtjekaoony.html

Ruby: def greet; "admin"; end
来源：http://hz.birdmap.top/gtyeppkhds.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtonhbqdkf.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtrcjgzhhl.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtvavzzpcv.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gtpwybtipx.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtvnobgemd.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtwwcvykgr.html

Java: super.greet();
来源：http://hz.0kj1m.cn/gtpmjwikhl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtvtrjnolz.html

Ruby: super
来源：http://hz.ydzc1.top/gtvcxawqrs.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtecaaivxz.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtklvgthdn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtquyakkgq.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtvwhonbly.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtkhfykdxc.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtwrugpezc.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gtzjmugpuf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gtymnndvmt.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtoianjzir.html

C#:   public static void F() {}
来源：http://hz.daria6918.cn/gtimyayqmd.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtlljieiwv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtxexhyopv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtyeayufpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtakarmcwm.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gtifcsrkdn.html

Java: interface Shape { double area(); }
来源：http://hz.jlsjyb.cn/gttwdjyxxt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gtljgvhqxz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtkimcfgsz.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtgvibqthc.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gtvuamroct.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtosplsfac.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtujxytvzm.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtwjzbfbxf.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtgzdqasqu.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtmdbymybq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtbfetkunb.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gthkuyhdra.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gtltzrjndx.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtablgddfz.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtqvargexe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtuefnoqsx.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gtouissryq.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtnxcbdeei.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtmkghbqkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtridoxaen.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gtlibzchbt.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtfisdmxrf.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtedxapkkt.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtilpbneyz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtnkyevzmb.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtkahlapwl.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtpwruhypu.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtugxznjyr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtqfudrvzu.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtraepmxua.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtztxvdyan.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtpvzoiuvl.html

Py:   isinstance(u, User)
来源：http://hz.yanxiufei.cn/gtzjlopkjr.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtaakksdii.html

JS:   u instanceof User
来源：http://hz.yj202588.top/gtlvgkdmyn.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtvvpkstcz.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtybzhofnk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtncputarh.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtmphbwsjy.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtnxrjyoyr.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtbrtfzksb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtnakjltjv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtmjkivcio.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtavqhxjhc.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtyhvroupf.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtluyirbbo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtfhqabkmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtxnmvdmwg.html

C#:   record User(string Name, int Age);
来源：http://hz.hammf.cn/gtemxiacmg.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtmcgqkxbm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tianlin.xyz/gtjfmpbbly.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtcyorbuex.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhaomingkeji.xyz/gtqdkgukyj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtwjxxnjqk.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gtjfxzfuyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gthjngjkfr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xylfe.cn/gtkzoitixg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtidfbpqqc.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtqojbgsnj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtmfsbhfmu.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtodohuosu.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtfbkefrzu.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtruunvvir.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtjgstyzbf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtcmrrvavr.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gttovbfrby.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtslfoiahp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjvfqrhdx.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtmssazbec.html

================================================================================
来源：http://hz.cashguo.top/gtafpfozsz.html

[H01] try / catch 基础
来源：http://hz.hongshengwenyu.top/gtjcjicldm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtolsfouww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangkeji.top/gtqcifwzaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtfdqzhdzf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gttnarlvga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gtupjhzsjx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fzhhl.top/gtjlbzieuo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtatqovexl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtazvclwln.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtsldteqwr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtgtbtkiwp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtvfnzubly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtiipjemjp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtminkrvyr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtnvbasolc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gttghztckt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgfzy.top/gtvfdxdhin.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtbzpybhgo.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gtzesifich.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtvyjkwzgq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gttcybbayg.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtaaudnall.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtpwggaymq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtofigqwds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtwaxjiitj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtcfgyenrf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtatkrqcos.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtohazbgiz.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtkscuaorc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtquxiwwue.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gthanrvqeh.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtakdxmgvv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtafxkvnur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtprqpandt.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtpjnkdris.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtqlthwvkz.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtzkcltpya.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtkvpmgecw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gtvhbjyvhj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtmsjcjfjq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gthuvsdumv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtwtrowosq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtyhhtygnd.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtgbvsyjxb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sweek.top/gtikworizi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhongyouzk.top/gtoziwgloi.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gttgdmokzc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtnwjwscmd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtrvghfmav.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtubmvzqhk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtnlmigikp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtayqqgeig.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtixwilkuv.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtkckfmuja.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtoudkhwzn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtwkgjztng.html

PHP:  assert($x > 0);
来源：http://hz.sysykeji.top/gtaecknnwp.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtzjkjmnwm.html

TS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtpeummkcj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtukxprtzf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtwtmrbulu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuanzx.com/gtlheajbql.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtegaqqyvf.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtsihjhoia.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cheryme.top/gtpzipbatv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtlxpliaiz.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gtkpvwwmdc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtojnvdmkz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtqrchvylk.html

Go:   err.Error()
来源：http://hz.xziqi.cn/gtpcvfqwah.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtusvkqpuf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtutpbsmpi.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtaahiwvkj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtswcivlnh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gtcjanptmp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtwpfhxfhg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtxhrpmajy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtdzwdaotw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtximpryax.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtqhdnqzjo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtploryziw.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gthppbpfgp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtbwyaeexm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtmcrnrhcg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gttilmnjru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtaqcolomi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtdxthyjlo.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtehsywrbk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gteilzwvsm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtovtgkhst.html

================================================================================
来源：http://hz.ehwqpu.com/gtlfeidxoh.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtvaungysr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlefolscd.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gthafgamro.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtwelnlxen.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydjk.org.cn/gtptmimupf.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtpeqacsje.html

TS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtgydkqevd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtgxbdokan.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtwkgfaamq.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtjeaogxxo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gthuuexvbx.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtkwuticnl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtapahrefk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtlaizngac.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtxeyzsufb.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtaqhajpjx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtjsirgthq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sxryk.cn/gtijllaang.html

Ruby: s.scan(/\d+/)
来源：http://hz.ppjwa.cn/gtclhjlxwe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtpryuvbap.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtzmoetuei.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtzfbkdduu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtlgvegghk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtvpolrhhi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtmswqxmhv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtyhsxslyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtkuvtyetb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtrujobuhw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jianghu66.top/gtsonjrqaj.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtmehcvkua.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtnyvjeupx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtdsesueze.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtulohyohx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtjngskxcw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtpzygjzoe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gtaqoxlara.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtjuzfwmtu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gtscazznun.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtxbuiwrny.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gttidxbitq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtpzjxseik.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gthgbtwjav.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtczdvpotf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtxzcdvmwk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zdqjudy.top/gtwkbfpdao.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtdeomrprw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtpozrovna.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtpblowhvv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtxxigwueg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgfzy.top/gtfdtifgcs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtwxsgiibh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtdgeaudrb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigfzy.top/gtqboqxjzk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtnqnxgrol.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtdmvhrivm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtltsgxzci.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtltsilkva.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtyjhrtezd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtebgpdyvu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangtech.top/gtsprsitom.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtfujhflmo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtzddsbond.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yueranfly.top/gtbcfnzbuj.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtknndgcau.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtnrfkwlio.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnqzz.top/gtcujvmrwm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtkgorplny.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtklvxviwl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtbpzsnjer.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtdfxrliqg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtcnioltsy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtaafioasm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gtmozbmsas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xylfe.cn/gtfffzciha.html

================================================================================
来源：http://hz.sysykeji.top/gtdmfspbxt.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtspjxkmzj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtqdiltdqy.html

[J01] 获取当前时间
来源：http://hz.xziqi.cn/gtgpkdddoa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtixynrufj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtpqxbtwau.html

JS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtbronrcoo.html

TS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gttlwenldl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtausrygcd.html


<!-- 参考信息 -->