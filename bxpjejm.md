代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gdgmbdoun.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/ganikpjjc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwfvada.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcxoncvs.sHtML

Py:   class Admin(User): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gajrkfrie.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwowcbjgj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqqeriuw.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/glzmilozk.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghftiedho.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gothhwlch.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhupzqwz.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqojsjps.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gajoobtal.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/giejrcnyz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopakujfh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guntlekac.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbkkkjsm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdnxlngqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjexivdk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fanxiaobao.xyz/Article/details/gpzaesnug.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdqghrg.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqoresnx.sHtML

Py:   super().greet()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgsehpsu.sHtML

PHP:  parent::greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gafwvctuv.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnglgpjyw.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxvhghnk.sHtML

Java: super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaaqhbbw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gsktyngex.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gssxoyyxf.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhtwteg.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gxskybwmu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gsmoullly.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpdqavwl.sHtML

JS:   static f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbrhpkli.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjcdolwd.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlycmzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumblorzt.sHtML

Ruby: def self.f; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guycjhanj.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggwuslnxy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimidfjgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghegfyxjl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/grhkbsmbu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdhjoqol.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzxsqovl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuhnlaey.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/geotfsvpi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpysmww.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpyawiiu.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/ghmgnrjxb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gitjiwuaw.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gqcfoegih.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fanxiaobao.xyz/Article/details/gqkxaibce.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynrkkylb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkjnabth.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gjkqaxide.sHtML

Ruby: public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrpnekaz.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/geryfyvzd.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/ggiuehnho.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwuiied.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnhykxyzr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcrwzxbz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvolhllat.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkbejgayb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/grsrbuybo.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdirgwu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geuurtbtp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzopoigjv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gqblxclkp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gekjkqpvu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gawdpuotu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gatsfkpzj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedtlazyk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnvfojlz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqgztbgk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gycnfxopz.sHtML

[G13] 判断对象类型
来源：http://blog.fanxiaobao.xyz/Article/details/gydqhsmdb.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gsujsungt.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/glsjdhwjn.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzyawhw.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gczzhscpy.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgldxcs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdrtcwy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxetdobqt.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gtuqquxlc.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gpsaxyrad.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gwoxqsgye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/glehltdoq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmdxpehd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhdooshm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/guhyagbqi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskzshvmy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmncdqlg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxudvpeh.sHtML

[G15] 枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtvgwuvgm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwpueka.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmulqaud.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gmeozrsbf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzofuhn.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmkkbnff.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxeqnue.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gwakcuoku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztmoyvt.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/godppfrls.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gmfzqwrzh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoqdjzno.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgisbssd.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfjsimmh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gqldgvnzw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gcmyjhatt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwnenvja.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gapozixxi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggaigclsy.sHtML

H. 异常与错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjcodrzj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grvfygbtb.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvbndybi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcrpegtz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnlrlaxyn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gejzswlaw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grlohkjid.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwlkmylq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/gpdghwbhb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsjjbuxf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbnpnpuv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glafgfxft.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/gnwqcbhpi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqethpevt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/glaccknly.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeexznos.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtplkykzu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fanxiaobao.xyz/Article/details/gbvrwdylp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gictmbmxs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmsyubbm.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgpkzdzp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gprddbjeu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnaywcxb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyylvxgwv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuomyaii.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/grstwaaye.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxuatmd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gncgmsprq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmlbpclu.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyuahfvhy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gybexxdlu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgbyvozw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquytdciu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhgdkalm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gllqlnvvp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwmwsdca.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdwlrlkr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqdawua.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geurlmyrs.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gxadrvivi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmzwcrmm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqjiwmcp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsrxhjwn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfkujieb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggivqnewq.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gvquegaim.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsbgzbpyr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvdyyzxh.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/ghdslpqty.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmositxsx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gnrgjeoaf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gembmkgav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgvqaeru.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlntyrds.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyuinwtp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtegwrog.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/gobwbpohk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilwengmf.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbgmsjxwq.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizwdfinu.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gejjcaiuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiyufnct.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjpaxrzc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/gbseftngy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwkyvhfu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/gnvbditty.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gszlwiibb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjkobhcp.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/guobmnadi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gfuldtghn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/guccqqsfc.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/gfsvxecce.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gheeqnknk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlfhokb.sHtML

[H09] 带错误码的异常
来源：http://blog.fanxiaobao.xyz/Article/details/grpnizkji.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gqnahvgxm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gvpsleebj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/gkprnvmqb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzfinrv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdfujeni.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkdpkstkj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfbsyfwv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapjaahgb.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gxibpdbyy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/ggmymeevj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghybhsspy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobyyhaka.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxgpdcf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fanxiaobao.xyz/Article/details/gjzgfogvh.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/ggfsyegjk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gffdufinu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gomkczrsy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gypmrizgx.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gshtpqpfp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcebnnqgv.sHtML

[I01] 判断是否匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoqmcnip.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtwjbpch.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqunneywg.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtastixdn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfwahddyi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/gfesooflc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuyjtbfb.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwsdwmtx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gekxvkyop.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxlukgwty.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbsgkpai.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqpjeev.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehebujdz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqiqzclr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gouifpxto.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gemzrktxs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqozmtvwi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gqtomamvh.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxftugopc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezajeimt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvylmztwz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvipvwadz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/goakqpdmn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxlsmanq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjetcgws.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydhbonte.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhfunzz.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/giuuyjafi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykbsizvz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/glzqchjuk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gzplaipnp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gppoevhwe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmnpuzdy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/ghtoebtwl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtntepith.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkmxiijt.sHtML

[I05] 按正则拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gyndcqlkc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkxzoljwh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqkltxbw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/ghecycygb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrxhhgdb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gqxeosakr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxajzobde.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbbtholv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gedkioczk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/gozikcdwr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcecgervm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmglalrl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbpspboq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gqipqsuet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwnagli.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gojfujbkt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkiginoh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gczecduip.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqfhsuc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fanxiaobao.xyz/Article/details/grmubcgyn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpvrtxao.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/gfyaaneky.sHtML

TS:   /error/gim
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoardfmn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqxkcqgx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gextmryyb.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjijusqrt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfzwlaiu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjsmbsqac.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/gwakueepf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gazuwjbgl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtiaqxpo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gdxgvenzv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/ggiplxnxr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/gynghefhf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gzadxatjy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gscbwboqs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gprvmpmro.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gazybdzui.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gojjvwqlm.sHtML

[J01] 获取当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gapxduucp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtfridh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gigdwkaia.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhmgszt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoucgugv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gqzuzcqig.sHtML

Go:   time.Now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaxucobi.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/gmubndfnq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/gqwyywpom.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gehbbeshh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gusgefjpw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwrsvpc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqdccfbt.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gerispwmv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fanxiaobao.xyz/Article/details/gbbvjxmvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gjsxdkfpn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gktxzmhsx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfninehaj.sHtML


<!-- 参考信息 -->