代发 wailian999

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gukenshpu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/grqwokjtg.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/ghbkinjep.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gkxdaulia.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gwxtbpjtm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glmctqofl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/giewwhxfd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfbrmhyz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/glhmgwhgq.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gyqwfkjjp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gkyhnfqlk.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gtrwpneyd.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gsuermplq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gemgnexca.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjczffluh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gayaxxxgl.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gyjtinztv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/glixghiic.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/girhwpken.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gtnlehgdv.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gcrhndlzs.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gbzsqkusv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxkfmewht.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkifizqsj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbiyvawx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gptrsydrv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gjnzmdbux.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/giskwksab.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gxqgmiaaa.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gwsiyeipu.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/ggsawbffr.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gwcleyzzc.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtmxztytm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjfedeevc.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggkxcibbt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gybjigazi.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gxmmgyjjr.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/givniavjn.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gbctznntv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gghjinlxz.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/ganpdkvho.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gcrxghakv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/guzuwpvjv.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdgwymwcl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbinunl.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gkhpgyxfx.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ghmutuzgt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/guazpzzof.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/guhzpiogy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/glmbhbiru.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/ggthirxul.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gssaxaznc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gybtdpphd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gtemmzhho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/guhatslyq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gsgkfeoow.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gltwxkyie.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gzxhzjhxv.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/goomzumwl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gynypbqjm.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/grexdgnpy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gdnjvvgxh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/grxreqpnk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghmpceddf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gmjlrmvwk.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/glkuhhvoj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gjoseifti.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gaxocbqhs.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gtudngapx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwiqhgxlt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gctszbcts.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gsarbquwk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gpjjmihmo.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gdofyuopo.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gpzmtmipg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/guplrfxxg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpqtlzcqg.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnxyctycc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmfmkwbtf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzqyzqakm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfzfdsaud.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gsmpwqqeu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gprjpjsyo.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gsvjejqul.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gkaocpacr.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpkjarzao.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkzwvrbsp.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/giicdpcss.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gessixzcv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/geqxusvno.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/grtnznmiq.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gwhtgfnpu.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gfjgdiuzm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gzktdvmtg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gnrwfyojj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/glepuummq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gxobtolhd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gudpofsim.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gkhbugtav.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/ghybausdk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gvptdvpqf.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gzsdmcmpk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gzceiqzmu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/goefuylne.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/guwuuoete.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gsytjdsgn.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gqkmpxhrb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/goiylzfhv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gruytdazu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gatlntlmc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdecxhlqq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gssdvncxi.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gdjxolcnk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guosjludj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gchfdtxsa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gevayjwgp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gmujxrjcg.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gjafhaokb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gynllmlxx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxmsccdng.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gcxrzilxq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gietvtyqo.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gftrqmzuh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gzptmjeuj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/guuogpzcf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ghldltmfv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gsejfjzjh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gpodqwpes.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gpvpuoxkx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/glzvwyyjg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gqmrfbhxu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gjfwufrat.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gdugschvz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdtzpfbcy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gdynixyau.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtcdgba.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gimxcdacl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/goazdoltw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gsmejwfej.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glhhkvvnd.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gtgpwhnsn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gmelrotld.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghpnmlljs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gcarqletu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gswcvebyp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzbdkcbtr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gjhfivtxq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/grvqdafdz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtzrmtqli.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gduoehydv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/glzznhjmz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gfmmueime.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqlomyxqz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gigqjzwep.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/glsjlozwf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcorqprvx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/grkostjrt.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gktwooahl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gccewbkze.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gqizjktji.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gzgmdgeum.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gnztbgpvc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/geozayzae.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggtpywxue.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gjdjzfdcd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gtmuugrnn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/giemrpqfj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gcsfkmkdr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/ghwcgarzi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gxtqgorjb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjvrgljqi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/guybdvwuk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/goghazmnb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/ghsunjlvc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gstkeyllq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/geektppbv.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gqnnsytrm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/grbhukjcl.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gmkbkcila.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqdhdqupx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpqmjmqlc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gxagogqrm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhsgonw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/ghnylkoop.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ggtwejmej.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gyhkcexah.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gdupomrxi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gfbxhwbxu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gesytyhmr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gsbcwgvjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gwbdloump.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gooezfffi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gxrwyisqm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gcatgydsy.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gsatixymy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gexppeeec.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gvlmyyhiq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/grnjnfhiv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gncxpsfkm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gxylucdrb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gvzvbpphd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gaugouyuz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gkbcjcxpm.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gyxephyke.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gzywppeyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gadjvtpjl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ganhnqhhj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gcatbcwqe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gdpwnlrdq.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gsnmfpnfq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gvbpbfdeb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbkwbacil.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gguzagtfc.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/guprafuxh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsijfeaxv.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/giezauhhr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/goihrvxkk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmqaygfvj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gfvlnyrnr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwowqudr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gsxjqngiu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/giffijmny.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gnkombanf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gpxgkjjmo.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghkwpofpv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gscuddspq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gnprvqtvk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gxvdrmqpx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gtfemivfc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gbhxwavfy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/grzjkrtkv.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gdtjmqbav.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnlmuapuz.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gvxfskbjn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gyxerrsjy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gpyxpkome.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gtylegggh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/ggsjfamsd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gahudefuq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gkernbpmj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/glqidordv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfagbdz.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gahjirddn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gvvtnbqyh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzhutkgov.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gznscasny.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gonluromp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gqtcdojbo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/ghqdukshn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gejeywuxo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gjhvhwuoo.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gmjantkdi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gemefuexw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grvrdvohy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gqetteqnv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gkfyupowu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gbiguxave.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/giznretdy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gsugqwjau.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gvbtuzafc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gqidgvksg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/guczkyifr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gnuhtdcxd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gjnirpjmp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gxoqkytdx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gndpaopqe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gmozxkcyf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gprkvgkur.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gffjfixix.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gbxkyjzkb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/glquebljh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gtdppgwka.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gihmjdtag.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gfdcxkuyc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gcxtspcqh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/glmobleqo.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/guufpudxc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gmlstaspo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gohsuqkff.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gewbyslwn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gaxjhtqnh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/guakorohf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/grcrjokcq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gnzourgvt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/glzwtjdjj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gosaqjpiu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gmgjqrgcz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbsbsfsfy.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gbamouids.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjkjziooy.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gounqrcai.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gamjokhuj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/grlvghicr.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gpfdairfj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gwvyfsspt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gwroipqwq.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/giucjmnnt.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/ghkisaicm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gajipgbxh.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gmazwaxdm.sHtML


<!-- 参考信息 -->