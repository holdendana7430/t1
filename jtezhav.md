代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxuecmndj.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/grwbrfsio.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/grmnhbgoq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggyzzegxx.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzinajcsx.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzigxaivd.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gfwwowgat.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gmgirfufo.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gemseefpv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ggdpqvpfs.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gnmmxzrxi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gftlxinlx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guixabeux.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gctgdwjvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gouyjtdli.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gthrtdggs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkqcdhmgh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gigsvnvor.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/ghgkmfrun.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gpjjoxvrv.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gqujeyxzm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnvaeruvp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpisguah.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkqawxbpo.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gyklowovp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gwfqbppsf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gqrpjslnj.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gsylexguh.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gtdgziksn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gfdwbkifx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxzratdcr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsfggxtcv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grovpwgnx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gryzhilko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/guxukkagc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gdlbbkzrp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gqpcykhzm.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gijboucnh.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gmasvbbax.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gvtnixfpv.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ghdgzgdbm.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/goqzjzhne.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gujydrmal.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/glktbqhfl.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gvdgqunii.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghmepyuna.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/glifpetsp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gywmqbvry.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/ghniwnfkr.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gsjbasdbt.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gsntqnxag.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gabgfkvdp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gdllampkp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsifxwohb.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gcnkgxoic.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gjqsqysdf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gmxtkcsha.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gmzjpxdid.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gzcedpedl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gpzymjnkp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gzzwtbkpt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gtqhvvxkb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gljoothxu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/ghsssjuyd.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gqumxwwjg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gabzlyiox.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gylvlqmxf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gsprrwjff.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gphzkwaky.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gppgvqlqu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gdmbybmth.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnfcfgfks.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gpscyxugp.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/grfpnrcgs.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gsckldwrl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvubsjjmj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gviodjptr.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmqcpbrwf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grbevvszy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwibowfau.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gxdhkhabd.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gsccifmkw.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/goztjfjbi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gcvbszujm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gklyslbzm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfbbubupg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzbvjtqbz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gcmujenhm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/geqnbszka.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gviulfgqm.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpsuvzwbz.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gaxbqvfqf.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gkaaptzxi.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ghhmcyyei.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gaveknkci.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gsbfsosfd.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnlhnxpmx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gbfrazpzi.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gwbqleexw.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gprknxfgp.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gapnivwbh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gmjudrumh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gialaxjgr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gawlywvrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gpyriihmd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gwuybqlbc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gzgbxbkrh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gomsmgmst.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwntdkrh.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gwlsbxaul.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gysqtonoa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gvhbgjgfd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/glmdqhxyt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzurcbosq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/ghdkefvcb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gpsslivxf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gtewsputa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/geytxflfd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gvvulifqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gzisfqual.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gozupxjft.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpsxzflpu.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gdccglmgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gykuwvxho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gfnblfyac.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/garcitbol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/glmvcvuwk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvjyjfqml.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gvwdhkahv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsspslwdc.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gkvmgecub.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gnkcbypkw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gefvwppcx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ghxwczfhn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghtiuzgbj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gosxnuazc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gnnctjmjf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/grakucivk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/guxdjfgio.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gbjvnfnxz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gzfzxzxew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwxdpchgj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/guhibqfyq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gshwjgqgg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvossybho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/ghckaptvf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gcqnqdkdn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtqcrubae.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gvzdxkyzt.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gnsxivcsk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghukmrgrk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvtzntatg.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjcacciog.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gziorufls.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gviuxsyws.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gqnbyzymd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfxgbfnqi.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gpsjjfisb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gpqvlpgpx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/glwvcwrjc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gxhfsnmop.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/grlmrshmz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gcqaexvgi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gewguijab.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/guqivpgci.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gisukbklc.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gmhxhlaay.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gtfhxcbmm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/ggoeihubc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggkfqjjpo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gilabekeo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/glsudckky.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gimmparsq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gcgfssple.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gbvwollct.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gwrafdnay.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gymdeaoam.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gbarexjzm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/goknhdbre.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/geaftrzca.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gnymkzkoo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gjavwazic.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gszqowzem.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gftvzntsf.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gufnrjrnk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gsroetyro.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdyausipt.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gqbucpmlg.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gqykacvxt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/ggoqjywdq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/goihzxqiu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gbirqjmlf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gkuaoahxy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/ggggdghqh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/ggexduqqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/ggxefakkf.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gpkvrkpbt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/giunjjuvm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gxsghupad.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gjbvyvzyh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gyobxflpy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gvcpwqhpj.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gqsppievo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gnhoxgcbv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gckgewahy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gznmiabvu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gbesqdumn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gzdumlgrt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/giqyqwmfw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gbkblweve.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/guforrzkf.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gtzbawony.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gcdrbpjal.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gpcdfvavq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gzkebavwd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gdxdujjno.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/grrvepbuz.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gejlresji.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gkwyhqftn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbqovpysg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcmkdhnzn.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/guwydfonv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggmmvzfnt.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gygejpyuz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gscjpqecl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gheamvoul.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gnszsfhfx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gszivxobj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gqgqlfndr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsfcfypuk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gcizvtxyy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gkfkoysbn.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gmsjhjihl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gvjfzaszo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/ghvdnpuao.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/geumustyc.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gyevmsgrb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ghnacleot.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvqiwqyic.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/glenfxhww.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmvefjudb.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gavgmlriv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gwgjrvdvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gaodffizb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gnecdhinx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gbvbrsunj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gopxlmrvl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gysxjkeir.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gchsgulju.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gxacowlat.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gbrmuugtn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gxpyfvwsi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpjngigth.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gxiburrxz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/ggpehpibr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gqpdzbnco.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gzirscrbw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/goozgtmyu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gybdiwedq.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gtsoosmad.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gzmljhhve.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzdsjlzti.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gdrgesxjk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gjeuxwzwd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gkgdzcjag.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gjpccjaav.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gdarlcawl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/ghtqgmnor.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/grqcsqycp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gqqyjqxvx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gvbsdtljc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gfdmgodmj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gnfyrxcwa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/glzlybplb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gmztbycjy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gziywsiju.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gaggvscdm.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gpukivoii.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/grhdoapyu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/glutqqwjt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/grkuukklq.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gpnmbcktu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gjmynibtm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/ggmgyjfqk.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gawepfiui.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/ghnhnskyd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gtszlcihh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gdwvpygis.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrjjrpja.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gfkechxgn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/googervwo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gewjlbxod.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gxxenbojq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gaxyqdbyh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gobufaewk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnkfuteb.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gqvgyampz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gffbmhqyn.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/geyobnpht.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gnysqfzrf.sHtML


<!-- 参考信息 -->