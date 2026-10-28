代发 wailian999

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtyqcyjjpy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtymtbehxh.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtxgjztbhe.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gtpcoadyow.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtbotmkhku.html

JS:   greet() { return this.name; }
来源：http://hz.hnqzz.top/gtzgbhlltc.html

TS:   greet(): string { return this.name; }
来源：http://hz.xylfe.cn/gtnxoigdyr.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtcbtafcgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gticmlbjcz.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtfmmlcyuk.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtsrmsidos.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtfdtbvmco.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtytcjrxrz.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gteekmxecj.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtahanxetd.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtxbbpclqx.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtsdyntkfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sysykeji.top/gtfmgxkeby.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtqfmeiejg.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtjmppaxxn.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gttgvcvzrc.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtgrrnlsgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtwjhyehny.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtxwcrkiav.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtmozoopto.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtjneubvkr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtfcwhztyq.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtagzkkmrg.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtqndggdjj.html

[G07] 调用父类方法
来源：http://hz.ydzc1.top/gtffilvret.html

Py:   super().greet()
来源：http://hz.ivvv.top/gtxammrogz.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtantmfkhp.html

JS:   super.greet();
来源：http://hz.yanxiufei.cn/gtodoxyvou.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gtfcojnppi.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtzohgoccb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gttsyyqlef.html

Ruby: super
来源：http://hz.gotoacloud.top/gtswmtwsna.html

C#:   base.Greet();
来源：http://hz.gzhubu.top/gtbouawyxh.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtlmwfurcu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gtlbuvamxd.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtehnjjnij.html

JS:   static f() {}
来源：http://hz.bjfxy.top/gttigslapv.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtsdjjhfae.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtnbynszfy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtskuiduxv.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtmvjwabuv.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtxokktdee.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gtuvqcfpwq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtdyskotjz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtapkuzxmf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtevccahaq.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gttiwqycjo.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtayuclles.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtsctrpibh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtzsjukvac.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtkdojxtxu.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gtmkjvwuns.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtulvxhpqd.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtjbgzkdyd.html

JS:   #private 字段；其余公开
来源：http://hz.nwbrower.top/gtjemjlwcc.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtlscqrjzh.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gttvofsvoj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gthqrpglur.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtirhkyqbu.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtstvkjgyh.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtofpnwdcj.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtezafobkz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtbrkrhkrg.html

JS:   get name() { return this._name; }
来源：http://hz.feifeiyinyue.top/gtxqawgyhu.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhixingplan.top/gtvgywlfac.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtanrxnbyj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtfsknsvrd.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtazaxirye.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtlmuxdurc.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtyhlcodma.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gttxucubup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtnivhiaem.html

JS:   toString() { return this.name; }
来源：http://hz.yanxiufei.cn/gtwvhftfmt.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtzigmpbzo.html

Java: @Override public String toString() { return name; }
来源：http://hz.jyoumei.cn/gtqlhgwlpj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtnsewbmfa.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtzyalnmta.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtrqvaujty.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gtbuebnyye.html

Py:   isinstance(u, User)
来源：http://hz.pycfn.com/gtrjyufadv.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtixppxhis.html

JS:   u instanceof User
来源：http://hz.yueranfly.top/gtggzeiedi.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtgselimac.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtxsodgkua.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtpieknhbf.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gtwvpdelgg.html

C#:   u is User
来源：http://hz.hongshengwenyu.top/gttjehwfks.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtcqtjdkpu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtukxgdlga.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.feifeiyinyue.top/gtvcoebqci.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtzpatgazz.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtbyxxzply.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtipqxixyp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtvpxpeuef.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtnnjrooee.html

C#:   record User(string Name, int Age);
来源：http://hz.gzhubu.top/gtorvlwiof.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtestgkjgp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtbjwsejok.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtmzijbabp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtefxoijdh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtfmlwcsma.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtgswthxcl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtfhknkdpp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtegvbikir.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtnydcanmi.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtbdtcriwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gtihpbgtin.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtiotjjhcl.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvqzfalnj.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gthjujxxiy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gthorptbou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtetiqpzdv.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtcphxkyea.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtqqpfmxnz.html

================================================================================
来源：http://hz.gotoacloud.top/gtvaibfmnr.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtarrsevly.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvpryivpw.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtcusugubk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtceduxygp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtapeecton.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtsyvskzkv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtsyctzfnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guannengcc.top/gtdjwsyzdc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gttpdovkbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shzxlz.cn/gtvufllgnv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtqxmqqclf.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gtxdxtgunk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtuncoaqch.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtylmyjznz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtdwbjhega.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gttjsyddot.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtkuucuhmh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtboylcgcp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtlstcgzbd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtuznutblq.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtloxpvhxn.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtmdpdbddi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtybjqbaga.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtxhvenbib.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtrjamoilq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtegjyjkqv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtprghjyat.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtsjjzimeg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtjbjtcymp.html

[H04] 自定义异常类型
来源：http://hz.gaohongyu789.top/gtwrkpcekq.html

Py:   class MyError(Exception): pass
来源：http://hz.ydjk.org.cn/gtnvqoagmf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtfxzdoxgo.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtspxeyfqk.html

TS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gteqvzxlzd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtyldtfzqx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtvjkkxqjn.html

Ruby: class MyError < StandardError; end
来源：http://hz.daxiang520.top/gtohfjpkna.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtpqbfpowq.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtixevplog.html

Py:   except ValueError as e:
来源：http://hz.snrcjt.cn/gtspprpfgn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gtvofgqyfh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtpqjcigvr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtpmvdsrnv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gthiwwqnpq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtpudbhpli.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtxtalhcvk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtxzeiefvn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtvcspdhmk.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtwidawgfn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtounkxojz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtlzqshall.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtbtofuspt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.haohaochexian.top/gtplhigqjg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtpzhuftlz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tanke756.top/gtrsmlpuuh.html

C#:   obj?.A?.B ?? default
来源：http://hz.quarkkingdee.top/gtxvvupznj.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtdeumarly.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtnpvikjqy.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtnmmqtwrr.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtmtojfeyw.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtugxowoba.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gttbhfjvhw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtveiygrfh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtmiwsksyj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtemjnzlsc.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtlyazyavl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtpuysktvp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gttjzbhdhe.html

JS:   e.message;  e.stack
来源：http://hz.cucudq.cn/gtpqffdlax.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtuvkgmruf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.redwolf501.top/gtjyrelovo.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtlgxknrvl.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhaomingkeji.xyz/gtnnqjorks.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ppjwa.cn/gthyfwcfoo.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtdqctikvy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gthdgmxiwy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtfplxoxjt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gttmjjfprs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258888.top/gtdmflhzfu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gterrtzwee.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtwjjdclzl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtgjdzogvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtebucvoqa.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gtpwyupumu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtxeyaxprj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtlqyucrzo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtkhgfcfho.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtjroceige.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtfaitolds.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtcdtaqkgy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtvfobwcca.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gttjyqaeqr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtznacpllo.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gthrucimfs.html

================================================================================
来源：http://hz.sxryk.cn/gtxnocqbtq.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtvknyopag.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gthxenqvif.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtxkoopgly.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtqxppwluf.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtfemucjwp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtckelsynt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtrnofqpkx.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtsynfrvep.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtiwyrautx.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtzrootdxd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtpmhdnjmf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtcolriueh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtmoopbxaf.html

TS:   s.match(/\d+/g)
来源：http://hz.yuanzhike.top/gtdzxmhkva.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gttivioqwu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtvgndpzal.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtqdofxrnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.feifeiyinyue.top/gtjfjhgvuy.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gtqtqvguud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gtygtgzome.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtjjtmfemy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtosxttywj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gttyjezsul.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtjjrbvipe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gtbmatssav.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ppjwa.cn/gtodufqsut.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.0kj1m.cn/gtbhzgsetm.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtvbefhmpr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtvphurpjq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtvntjxkcd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtndjmezzt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtfifcysng.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtsaojmogi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.mhx1999.top/gtmpipkylb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtbwpfamfg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtvzmaxemf.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtsmednrds.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hongshengwenyu.top/gtfjrisjwg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gtahqcfvdd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gttgiauihu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtxwuioqjm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtlweskwuj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtrnobvkia.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gthwwwpoyl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yongpay.top/gtdodchdzk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gttbugcovk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtbcddydue.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gtprqoighf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtbvevabsh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtuvazqrkh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gttmvmvjrv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtaqkjjhhv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtavlfftjk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtcwcdhmpb.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtiimdwdhw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gttnbfzczk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jlsjyb.cn/gtzisuumjb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtzmywurpv.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtvybwfyxa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtuqtzlngo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtwoincffl.html

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtksjeiqrd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtbgbqmbsk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gthhbhdlhl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtcftrmgti.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtfmnrsmfa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtypmdwcgz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtfettkgij.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtedbwzmms.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtwttqqsdx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.9152youxi.cn/gtfgkhmagd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtecetuudb.html

================================================================================
来源：http://hz.gzhubu.top/gtzxbnmnwq.html

J. 日期与时间
来源：http://hz.aizwys.cn/gttrefkzkf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttzzhytqk.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtztnxtdwa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtfhadnpsh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtgrmemogp.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtqxoherps.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtxsiwbkfe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yangfankeji.com/gtvebrivwr.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtggetbxmp.html

Ruby: Time.now
来源：http://hz.jqgfzy.top/gtejcnhtjn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtrbyxqjpu.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gttiruwjds.html


<!-- 参考信息 -->