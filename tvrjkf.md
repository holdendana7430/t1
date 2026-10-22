代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2akzqxvnx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zkixsjve.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hnkbjabm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2soxlzunx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bzjmhtkk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cdgtbtip.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kjdzduxu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pfkdhzmz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rtwljpch.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2iczioibz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbnvmvvk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rdhhrcgt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xatipexr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mvndvufm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ggqwwyom.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tuocuiev.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sxmcpotp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtcwqizm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wgvfugyd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bloafblw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sonchtif.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbqazema.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzzrrilx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rswpbmbn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhabvdmz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jqfmmbky.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2msiwjrhx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lleixkts.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ihfayrjj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2feqhhodf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jybsoumv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdrdgiw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsraiqzi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nfcsopmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kvuesbce.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iaczetsl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2btufzgps.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ymftohkt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zfrfazjy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dbrkoeln.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kuzawmbp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2brzygelf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lcplrhjv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhzgspok.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tpvyryav.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2giosrwlm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2abuzzbtd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2edoddhng.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jdddcgym.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbbmnxck.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qmxinevn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2savapfrv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lvvorktl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mkbqipxe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2blzzvkzm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bdcudpqj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2eplzbpct.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyxgvafx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sggpimtx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzldnhmr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqpujlsa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvuykrgw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqnbmxav.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnfxvgam.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lklvcygi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xoqhtglb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wadexdah.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zphnlvyn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2honnmhif.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vnycozmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2piusamwb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jgwgxkzu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xoxsepft.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rjmfpiqa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bwawxnxl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fbsbydvb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2siwnxgba.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qucrqqso.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ldtxdjpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2atmhkxqo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ydagrtdn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gogjhluo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ddbhotvz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2euxdtive.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qszzzmgu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhzlsskx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2izgozqcx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqpncwpo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpxpkyl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vxikfrfj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2trlvtudq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hlkjdivw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpnlimm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jruazkbu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lnabahxk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zrkrdsnl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yobxngnm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2iqgylegg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rtiybbtg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vjfewtlv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2dddwfiic.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2umclwssu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2beymntgo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pbshfssx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mjdxypot.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyuzkmlo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vkjblcpx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hlcpwfqn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmneuw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2whamjkzl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mnbeewmb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ieldkcnn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yynrdoeq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nwedppps.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xcfozfem.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2icivmdtw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sstqkwfd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bciidmyj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zozfuigj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tklfdtgq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2obpjvozw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvfzygj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yqprzdwb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wwepdsff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2idymexlz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fruwyozb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uugqxjbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsgytqka.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rifdhzsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jblpucje.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2islxfrwq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmjvipe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxiphmcm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wcymhopw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmexpohz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mwlsaesh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2aigxkxdm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vvgzvlfh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqrhkffn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2aiviejkd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2udwkfovp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2svuondod.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2osqweczd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jepdbcrp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zuezdygi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ddkqredk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bagrfffs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2szuhhejt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2seoteqwm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ccytmoal.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tcgozhad.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hwvxutkc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2exzqhnqz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gibwtcky.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwhttvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ovsysaeo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hhcllbay.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hqzlyqre.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2htdzjbcm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kpfymgmr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rlhdvrko.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gwnvxaij.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bzblabyn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ldjayciw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpklfdnj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qnrwcqqa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ncpuajwy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gtqjabhv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xwbgjdcg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gadriwfn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqwzhqet.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oalaifji.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wbjmazzs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ahgjkaen.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huuambim.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2epyqkwas.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zikzhluh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2osradgiv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lunovjrt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2swzpirkp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rbswoylv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ywtmador.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2eenkyslw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2njxouccu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kjlxgdtf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xxndlgdt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nnkirhuq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pvbxxdxb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jjqsinbi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2jqugbhue.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wkhkmjuk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2azfjtrrq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zwmmbdcz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgefphhq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hlmopffo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2roynkjfk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ilmwxbho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxbngtv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yqsdihdp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rpdgxjet.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bnhyztbs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jhfubrim.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2npupiryi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ksaxxjct.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jpyaqygi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fcziewkb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmveyoow.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qadiplzo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yzunqzpk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mzslaaej.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jdimgwsp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kvxycbdi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2bfahtizr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2efkwywvk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jrvsoxul.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vcwqvwja.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2viqgksqf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yttxmmun.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kvgazqjx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfxlfzwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhpvvsbb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2frrhktso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aamekcwh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2juiuaxpb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tulkbcto.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlvxzkmd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwloozf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amqbtyir.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2epyzntvv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyorruyk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cbmowcfw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2imxphkcf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dwjdcxqt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2thfprboz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lwtlkzdr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nqvituoy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kjprcgwy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rlsrtuje.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbavjaei.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2svvjgler.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmrlpctx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gjwvxzjb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iileowme.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nzfdvace.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iogdhbcg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bpbdqctf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2knhkaczj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2motalwab.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kctcduis.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dwkgfxxs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hvjnqdbf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiestcgf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2idygkyrw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ullfrszj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eqijnenj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2upkudbez.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kyoozgwh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hskksdzp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dsgotlml.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2sdjgzizx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyshzlyq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2btvtopmq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfteemvy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vndacpxn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2btiyzyqt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxeaufdc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2txbpetbv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ywacincz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2kqqpbnct.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jwygapqv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ywnmywej.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kgaoijiz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2htpncwjp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ogfsiwad.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jpkaapfl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cejfefmr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kgdureqf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mhummxch.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2syqbcudf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mwzgfnnb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lwakbapu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gscswiin.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qkbxprsf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ojznapuv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfgdkxz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2luvbwvkm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2hybvkacc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mwifdmjz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mrsnhixt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cruofiwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2aydatkyi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wzwveyfh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2dmxaoxuz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gubxsvte.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wyuivucz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qymjwcmh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dkivsxam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifgzlrwb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ofvfbcgg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2psniuzcv.html


<!-- 参考信息 -->