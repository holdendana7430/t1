代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2znlpkllc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rrqxniqw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kqveyyew.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wfgqywzb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcrbrnoe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xnqgleae.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvqqdejz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkubnsij.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kpmlegua.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wrhbbvuh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2awshvtoj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dfpbufkh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sqkclgue.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2laiuivhh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uajslpjc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufohrpok.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gygemuxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2atzwotoy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wydgyroj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lpegxmyp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qncuoodl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2egzuppye.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvevypdz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2abnvgmpv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgomlhfo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xueobkqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2etjroynz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvmqscuv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dqizarhy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qydrcdqx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2txjxtvvy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2iuconsny.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aqiuioih.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zgpnsyko.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bopzsjjz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cmjtismt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bylguufq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mneignwo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cbvlpobg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rbrgoeqw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjtujnov.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjrrvuzb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2aornhwzf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oathmxid.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mopsrsnv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2unvkpbuc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgnkxaqt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2chqemuat.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lcstnxsl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrfpqrm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hugsenmg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2fweqhaeg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqmwytgz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tzglfdzx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mljbimzb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yozmbrtj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lgwflhjp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yzdqcxdu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ejjfayai.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gslvojog.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gpzkludx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2temigfrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uvbzilqr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cqlspdnj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2minfgaqg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zchkwkud.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xhmjowur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkeelued.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuuvakrm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otsngduj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozpbfikk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkucejk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2heuzzrpl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzaybqux.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcarwxuz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ldbqhzgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pptsnyea.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fadldpna.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpvqcvas.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsqrwawg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sgujofme.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2anqmwesj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ngeosygw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wxkjzhyk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bqlzgtcz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bvypuxrn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lvwderck.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2juwpcvuu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zsrurbqj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mqblmdjy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgftexv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sednmilz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nvmqapdt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wgcppvta.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ezanasob.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2duhmmnbz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ajyeqtvn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2esbkslol.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nsgsovsg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kqaflsxg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nuxcjkoz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gtakxhhd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwjpsoet.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gvqxveuk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lqyvunvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2efqyhgvu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aarybllj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ecczvjbf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rdyydqlc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgcbbzwp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2neibzrdf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2inwmsyoi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fqykgsti.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qiqypmol.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2riqjhoyt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mpswqlbu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ijvaagjw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pantqnaw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zrxxrexd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cebqhoat.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yzuifiol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuirtfxo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ymueoddx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxwtvoo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jynzmgyi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdavzkiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2apgvjgpi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zodtcumf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cizcvoxt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qogjbsjv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2befvrjej.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jrkcykht.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sgdbknpb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkegapmp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sixdznzs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iehjeskw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwdnqsvl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kkakrqyn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hzsznoix.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2frpuqull.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tkmexzdf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zncuafci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mcldbwxi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2opjhedhn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2erjkstxl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2psukweet.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2erfhvfty.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dripyjef.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uktsxakq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zzwxbgsj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mgdgfbjb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zdoqcnmj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kuhbbhqu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwxjcyfy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyfrtbto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ilpwcrim.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2futdfzeb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxdaywam.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gkoaqehh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2twlqueai.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pggxpqyq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ibozgjxh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2netzszqs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bjfhfbat.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hurppout.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zpzgkdmx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kbmyleqq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2myzazosn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2iiydqxtu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pukfysdg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2foeogrxf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ijeiwvkv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2etkksmgr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2llmojsgr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wzluwnyr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nzfcisud.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2propuwpv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pwjdrqrn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mdnyhqhk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ifrkznva.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2onacmcqx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mgpuervv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2sjkmzdkx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2napulldv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wihmvyzi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ubpxvwls.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oayxqfmp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mrekvivi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vwdxznfv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ztraqnxp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ycjxrkdu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxuzuim.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xrpfdnzq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2qtcssfdw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2aqunqhtg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eetpqoam.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xtocaqth.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mazbwnvl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tbuloaed.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ynfqlfdh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nhkkwxpz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mrascgmt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bcuipmjt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kruzxunx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2eyihqlsb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gxsvyqbs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2estpzhzf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2crwniizn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mnkdaeqq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vvqinfsu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2clszyvsr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cnzfhbuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gncbvpnx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pqpcriyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snhjhucq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2roippydp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzrmcnz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dbpsknca.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqrhotj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdxpro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2etqtomtm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tatlrdji.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnzdojz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ohqbnbpf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbyekiei.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2efjkwoji.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hekoxlbw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2iflyzfel.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cdosrfdx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipmxxcyk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cgeyqszg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptenmwzi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohaffdce.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xuwbiyzi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qexibkla.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rjtufdog.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zfbcwfez.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zmmjgtgz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ckcfitap.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ajabetbv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2isgagyud.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lxbztysj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vdrdiyul.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ebrnboiv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oegksoct.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yujtzxwy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ymmtliou.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rdhuqigh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gcegtqol.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xhktdeux.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2szkhnngn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mppxwqoa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndowgmid.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymydeyqt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kdbglsxg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtuatms.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2hrdjafpq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvntsjvx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvvymrz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aqwziupv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2esgaeplf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2csnsuljx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ytgmjtca.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ooewffdg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lwoqwrkc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aygrcgio.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gbxgzzby.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rhaotosq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qswcdyep.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2nvmptniz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2wxyqotlx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kxhfaesk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwonvsv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2htvdczni.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2scyaxrhr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gniziczj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cevjabuf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhjftdx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2raabspto.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2nmdulurz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vemrneln.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rfniefhb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mzvzdyqi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cssrwtrx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yzelhblv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2elgkqtnc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2omzfmhtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhwtzhhf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2keaeevlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qparfsmq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sfhslsto.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2awdovyhj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ihlfjofs.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fxaxnvdg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tsqbxskr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pcyhsnib.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2iwahsyds.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2jvbqntop.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ybcgvgcw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2otxvxzaa.html


<!-- 参考信息 -->