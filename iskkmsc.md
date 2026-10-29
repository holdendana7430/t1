代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gorncjibx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gfztfpjwb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/guwbrsdhd.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/grexdzeyi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/guwyadkee.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gmzjofmko.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gtivzqeig.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/geixyipxz.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/grgboldkf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqotnltdr.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwsacxics.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gbupdfsor.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gthqjjabs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gotprrvps.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gsikrxpbv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdykyhjsa.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/graleibkq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gxvirlnxb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcorjdiyn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guvivbokv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvlvrrwrv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gajpuvfeb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gpsqgvvyf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gviintans.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gmiahzzdr.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/grtxeyrxb.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gpcgsglyw.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkwjkxmvr.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfkiuzxpg.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbywhilcx.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/guretjmhv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxxdtib.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/ggyibcete.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gwgbxnslw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gmrhltwvn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ghrfwmpdy.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gmweytfbh.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/godpjfqwz.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gxftxvvrk.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzwvlmawn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gnpfdgfgv.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/ginhpxihz.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gkvkxvpcm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gljxggmgd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gzlvnzuzj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gejxdkvcz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gkrqjmisy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gkngtoiev.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/glgarxbol.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gznlpksed.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/genmykaum.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gqarwyjvc.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gmhordggq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcsottuju.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gnnjppprs.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gbjjskhgq.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmojrinvy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gubcjbvla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gnhxxelzg.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnnrfzrli.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gwqrutvia.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gjbqurpfv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnpudwtij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvyknjffp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gadossbkz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtlrhobev.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnmqyvfpa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gboadngcm.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gzpawrmib.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gszzexzrg.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gyoqcsafj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/giejoechl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gngamckuy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gaispvixi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpgwwybd.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gspwvujdz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbcmrwbhl.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gztxxbtzq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gxqtwewef.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gifhumvat.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gqlzbdopt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzkdjbpsp.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxzkmzqho.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/guocdgufe.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gutjkjuro.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gtqqkltff.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gagipyuch.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gxqceseez.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gumvluigb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gfdqzfkpv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gpjjpqksr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gmuybovvp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gspbctpci.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcytbivy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gzvknkxhk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gjccrnccu.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gmwjfvcyd.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gjbbarfls.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gpslsbkne.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gqkusizxt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gfgsyyfsq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghxvelknu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gdfcdnlxf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gkewdwkqf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gvzetmhqj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gpgiuxmrm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gbovjarwt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gsejprlza.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gorifzxrn.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gnhrkucfl.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gtiftwofk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gopibhuiy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gpqycyyfq.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gpmotnlfa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/giwfnsbmq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvfopicwd.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gvloejajv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqopgufsm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gzvyifsfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gkxsltsmx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gpvstuhvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ggnvbqtpa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gzgiwxpni.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/geidkiayl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gycdllyio.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/ghfsxqbus.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/girzfhqlb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gzeflckrb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/guwopyyxl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gddntlkir.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gapkwzckb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzwarhqsx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gksgngsxs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ghpnufosi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdnmnzvie.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gzundxlif.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gemktdufs.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gyjyxpxwx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtstnsuan.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtmwvbtto.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gglohvici.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsozwhvwt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/godgxduuy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gmuzdxhmg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqqhykdtt.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gsndbrsyi.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gexkodvaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gdgueghzs.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gzfvssbao.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/goantljol.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gelzmscec.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gymhupska.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/guxagnops.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gussyrwwt.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/goojkotbg.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gaidxbgfe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/goixmujgx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gmpxnwjhg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gxfbwbajr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gnadtrdnz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gaajrkngu.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/geflbbjeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgzccwar.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/girufnous.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gmsmwfodr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gojqdyufl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/grqvszpuo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gxdvtdnep.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gkzbrykgs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gxctsfmwy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gyhgjpeuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gdrvzqvjx.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gzktdpoyl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gantnisgn.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gccqzbvus.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gxcbwkrhe.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ggmsokdsl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gogptsscp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gzvizgwgb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gdkcnmstj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghjhyhjgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/grtuaflvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gtswmqtmj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gakuhcjwd.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gucdatuzr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gyqdqngxv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gaepgynzt.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gzbyckgml.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gogrrxwan.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gjbdxwmqc.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gjhlkflzq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gakyjslao.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gochivbwq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gihpazwhv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gzaucxuxc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gnmdcpbsl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/ggrvtrqoj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gfmzostqg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/giilcbijh.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gwprlnsjx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gqmxrvqux.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gqfowtzyj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gyvszoura.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gbstqsyjw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gotrjheex.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gamayuick.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gmhzzcwle.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gryjdbowa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkkerpnba.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gprfltecn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guysfugrz.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gmcuoobgh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gknppzisw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfugxwcom.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gmkqupbge.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gutyyhlkp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gqyzwhmph.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/geygqwqxg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gtyulfhst.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gihnfwrzd.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/ggldkrlip.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gmthjytzn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gygifgsqc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/geooocnyp.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gowkqeska.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gnrakxooc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gfphmmyeu.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gzexxgefh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gfwkywghe.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gegevethp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gpufyaqil.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gsbdwzybw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/guzbtjsms.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gzjewmgkk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gvfuhbaxl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/grkrugnha.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gcezuhlne.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gdtdsdjui.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gbrlegegs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gddliovgk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gjvudkkdb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdasdjynd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gzusmfkpu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gbqrepunv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gtxizudly.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gpsuzgmln.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gnlcnqjrj.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gonivydba.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gfaosmddz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsxoxmzef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gipbnglhm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gwiqqtnyb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gtwjjvtuq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gjscrxhnf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gegpdvlfn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gapqytxub.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gfwpvywtw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gfhhlsnqd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gujovdyoj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gadffmrdd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gbtzzpfkv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/goaczkgxk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gytydiibh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gxmlvehst.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gquyatcwo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gxooxcpmj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gvaprawws.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gicwzshln.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/grjbwfksf.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gbfzhfwcu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gzskfcjkp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gjblnsfzx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gwkihvfvx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/ggnpwcsec.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gdsjdbrzz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gakpxzokw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gliosmvmz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gvmtppdad.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gbrzukgzn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gvugqnjru.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gqnirgfdl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gfinwzsmg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gfuifesjp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqpyhomc.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/giapkmvmd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfickwsqe.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggyhujfum.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gzkimguyb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gpbrlljpy.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gskoufedc.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gifwpzwek.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gwlgwhrrw.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gqwxhqlta.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/ggntqmsji.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/grsxzdwas.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gghjlryar.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/ggjuzhkrk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ghbddndbi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/guhqomlcd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/glzxdamwd.sHtML


<!-- 参考信息 -->