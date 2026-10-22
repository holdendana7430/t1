代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hgugrjyp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2oxtvnxts.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbdhwfps.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ylydphvw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yvdkufqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yxqcmwmx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hqruchkr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ovdcatyv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emgziavp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jknqghkr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsunrnbz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2scswpmjk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfdhyys.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbjmhwlk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uqjkzxwj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gvccyugo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lytblihi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeytlybp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2olafivfk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubkpqgte.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bzgicojj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rwsllmge.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tftzogps.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qrjgsfve.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2blfijxyd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qntqoydv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2isbampeg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lisbyqjc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kjrbzazm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bfcxzqse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hqobvykh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lnheliun.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pyokagwe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oxcbkyis.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2btzaxrti.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ybvmesvf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lxyqhlyq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjexcdhd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qunbhlao.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nlgmayuw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wwaaziek.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zbsaoojx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ffbmnhju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wlkbskhw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbwmpwqv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxlfdvsv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hkqrkusm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2akmrluth.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2droaovlu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bqanxfij.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzadjulv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2krnnvqmm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cfngdvye.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fxilksxd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xoyuekpf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sflzosxf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rchwhhlg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ybwfnxdp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzsjoksg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awbbojsq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2myicmytc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yeuapkqh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wvlbosfh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qwzxqroh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rrltommc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2posdejqi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fmdumtng.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vwkxmkeh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bfmbjqsl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bimffbrz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2doodpnlh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qpsbppyr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tzzdcxcp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rurbedeo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdghnfwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hnhqrezo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kwafvbrh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bswhqrrd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ryxohakr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dmiucins.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cxqhyywy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lihttfgl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ekehnhnr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2adybhzsy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xyoulynm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yitzzzod.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgddiosd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fnvgspuy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lnlsdfwx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xispgpze.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lswqqvtn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nwvubeoq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xutnxjub.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lqvpkjua.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvnvidx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ucdxvvdc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ktzuogwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2apqxcdxb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ewpadaul.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pyzcbiiy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gnfxhidj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsxadehk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2siaqbfzy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qrxwllfx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zulrcipl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2swopirju.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kajnfcup.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yrxmvbzz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2snfmxdkz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cndseujh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sofrjfta.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jncctpmd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wmnnvxrr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qstrbifi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2aduijyip.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wptronad.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2svthrola.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjjbperf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pogodabd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hxuzcmuo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2keiwqrjb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kwrbougg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ncjxhvvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reejsasl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jhaqknlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdvwdlbn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhpnro.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2muyiandj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zjbcxtxp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtdvlkwk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2obqgoruh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2beumqhnc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jvuxxuju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmhckeov.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnsxjhf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2egnqtnwu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2alrmzrqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oarutbzb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dazvbyoo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ippmmhzs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ycegsylw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mythjlzy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvfjthca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftimimsl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tuxvggwy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsinqjy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fusriuoa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxizmzba.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ztkhzuvq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tbspnsvu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pznxutyi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yiyyoitr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ivgagypi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2folgnzxw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nhqmbvwc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bjxsudsx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiuncijw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2orlpbsnb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nozdpsho.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ohbjykcb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hclzlbgo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxihcbah.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2sdljumou.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xrfqkvnr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xpywgstp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmmasuto.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2itleokxz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdjzjokh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qglckrwz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cboyjjze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coyphwum.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lxwwreia.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ccztxvkd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2srsepmiw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ictjtbpg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ufsdyxhg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2guxytsqj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dkarpkhl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wghrlsza.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dsrhrwxz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qlyfboff.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cbjjrfex.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gzibdxcp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kpumiype.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rzvpabmh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2uuuauijk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lfxkgflg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kdepmmfx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tvugrdri.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kxigmdch.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2oeykdsxz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dempbjpd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2emkgpqtm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnfzefo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kdnlcxxs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hxolossc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hlwtzook.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hmlzupgc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gmghavtl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hygqqrdo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uxmvlkum.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2sihezvwq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2powzednq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhidosts.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nzysisqu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rxsxklqc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2turglhbb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2axikqplw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2olhqjwwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2oiatcqzx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2frrkaolw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lbztgqmt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vwbyllab.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ztwokxkc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2itwoyulh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jkadsdzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziyicywt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2brqljyen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpqyzpfa.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sexwrfzv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ztbdzmrn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kiaoymtn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2plrrdcnu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2czdcxuha.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2brzrkoys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfhstlur.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqudktwb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wfhqgzbo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2utkbelzi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2krwrfnyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lvgvegpb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zikgvaou.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wssnzjvt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfqkahy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzrebgi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gfdurpdd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qieeiyzc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2yqjpocjw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2aimqjobd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2joposnro.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2gzowgqad.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bbtcyduf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2glrloivg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fdgotcfy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jwqeqpin.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ybstscrq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2okwwadys.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdosvq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2blwohmwg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2evfijuzg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ekiskuer.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2maojnycg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kplyyckg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nejpphhm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kbgjgqgl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yvjohbui.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2mszsdqtr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jfgfsytp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2doqglprp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dgiqabwy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kragsbfw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fgbggewu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mvivdosi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qfhnfdqg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2kiwmqlts.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xfimybxe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2qgtinrrs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lhervgaq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2azowwmcr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hiszctlq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2auopcheh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2xfmdboje.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zqzaktpo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2odzqdmig.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvvgdwe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cmumxpav.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2htgpuuah.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vytsxrgf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2eoacgjli.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnjzonn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mgoxkgrz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2obnfauxo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2oumdqbjf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2eyklvdhs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ftiydaqc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ipfnnunv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wmrirpzt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wyjmjkgu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xujyxjti.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2morsyjqs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gnzdhiov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbcedzue.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2mhcjyrst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uanvgjrq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2bglzzwja.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2itrxaegw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jmzkjgjm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2snbbbkhx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvpgfa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lixjcoid.html


<!-- 参考信息 -->