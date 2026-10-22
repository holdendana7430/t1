代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohuphleg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iywrjzsm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qfejnhbr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wwcsqqxv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nsxdrvof.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qzmpbwja.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fzeluzkm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pzpcoola.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ecbipvew.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qkagszia.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lbgsxaxf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2szmcfwkc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzxwkafj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjbybcri.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwujycz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2janjnelu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gzqgpotl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2totmhfqj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fekjidqa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2biqsindo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2scefjqcp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2akqrfjem.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ypxcnzif.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gykmtuah.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eilsmrqf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pqgpvhpr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ihiemtgt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mhvvnemq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tasddawr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lekkizrk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkyuoxlw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeltglvi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ncisotvf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlkhubf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2goalnsdt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iscabqal.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tbrtpxkr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mvyihtie.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ngbkifqg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pbchsdvc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yxshfxzw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pxoecwdt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qvwysxhz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pmvibdgn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2eubbrjnn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gfmoogji.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gfmvnces.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oqtnmqjf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cwlhbagu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyuiijho.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpdsebvc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2odlboolq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ufrvcbko.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdnwxfta.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fvaknuyv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hjuhcmvw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kksnfmbc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tkwuyeit.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kajupmwj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnkjngfv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lypqndcu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfeobxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hkonjtzc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvzfjrsm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfkvaure.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cepzzups.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bzyjqhtn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sctkpsxu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iqdjzyoj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fyvlzlsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2udfhxuop.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ihneurxz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ttimgrch.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2belgxiin.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bwllvpah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eumlimhh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfwvlbj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmyxvmej.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2drtpjosp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qftsfion.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rvgmqlam.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vkbheoeo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvzgujul.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xaeuojlq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qagmytlw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuzaztgm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mboznxan.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pqpqdfjm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhzhfam.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pkoriwxg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yfuanqpr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vpjhpspg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tzlhorvc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hatukfuw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jqcrjcqo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xcwiynkz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ejdzptmh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bzvdwckr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lksukrgx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kmwkvsll.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hfbderve.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tjdrukpt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fcaamvta.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2sonvtprc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ejojxigh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qgaaqxia.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zttzyiqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fcfrmhfd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wdioqiax.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ubkzgdsi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wiywrvhe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2isspimeh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vgwnuzxi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ydcmsfwk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xwpkvzct.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dhavohrn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2legawjsv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ykdbjbyq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wwcgirmf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2esvptlhq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2uexjaway.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uyxggrgw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mauczpac.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kilhxyfo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2sspxutqi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hnnndufk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wiqkedeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avyxddej.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jomsnbfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2advmmpel.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2serhjkzs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yzlvcwkt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ihjyhukt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbnlzgux.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbbecitc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubhkxbyz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ilrmrfnc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2shikiyet.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aocmnhut.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tmlmsdcc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jlrzfhrt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frdebwry.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfzivat.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2waskfxkp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmgkhwsq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pjoqurjq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rmpvupnm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyyyllsn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zvcuoibx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpjifm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yotyzgne.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rbqewarw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nrizbseo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fsrjspvt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vihxkymb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2sgbgcefe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ajcqsdvn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2raabivll.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gouoelqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2azxhlxuv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kuytlkzt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2twcaiycp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rrhmvtkf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rvghzyzm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gltikegh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2whbppgdh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsrqvfzh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gshixfyv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ppzrwlof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rllkqpbg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctkvonky.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ohugsiqr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ghluyven.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zcqzdthk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rheztiwk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ztycdqia.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bnzojzlx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hidslrhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2twqlqcsx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fzsuqwfv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2flgvareq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lsjrsszs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nqktljxk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dbrpqrzg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ekobhbmf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lwfpzase.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ncsgtibp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mzhtrjoz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vjfvevhb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2utpkxyts.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vpeqiqaf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wbroakke.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gdqtlrmk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mtprhlgt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xkaeknwi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rnqhapjm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2fwnplezv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aavbupfm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2oaeauxtt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ywuvreuk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jtajzeia.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lryvahmj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wjizbfgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zdaawkse.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2noegujir.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2gcsmwwbl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jocizpde.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lszznyjy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mukdhnuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2oustdxek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pmkfyyst.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2acfihrfj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2surswefx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wlpbkihv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gyewdeww.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jegvelwz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wqlgvnuq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fspvtoec.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dzyiqpft.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfnmvoju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbghylnt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ecjnjwjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfenbflg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2igfctmlp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oxpgjbrb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnlqkrhk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nmwfrcll.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joovozwq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2iiasafab.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyygjxuh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uuhsgdxl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rqvcxxqv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lovnbifb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lnuabpao.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ojpuvxjv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2dlxbbrjw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hlobhgrg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cytfnglh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2okwdkuhy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnybxvt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mgmhxccn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dpvsjkhc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2tihdorlu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ubtmqzck.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2pfqqvzgq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hpuskwiy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ymupzryd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2eenodrnl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2zjehdlqn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cwopbtdu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fnfoblzl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ajnszdqv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gpnhijwk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gostbnzh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aayhosrn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vlyciobq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2bruvente.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rorllwfe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hilffvtn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pahsxcxp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wcridaem.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mcagwfwt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nohqtqpy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2svoaecpd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cheevcjl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ercytglq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fwrmanvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2cjjdejax.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ijfeckai.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kcgklegt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zgxvzfab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2liaymfkt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bufhjsdg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qoycmsfn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2jjycoemh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2hspiyynl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wsjjxnrj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2enrfxtug.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xiaugnrc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2omzuywgb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2verquazn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2gbfdzbog.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fbilsjjz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mutemeuk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ugnppxdz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lwblfydj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fxnfzerk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wlrditxp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fbqpcfre.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vlyquevx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xeunprsu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2brucctti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2gbrotaph.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hjhcixmh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zefwdmra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciktedhy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2yzrarbpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crncmwoe.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mgpsmkqo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bfyltthe.html


<!-- 参考信息 -->