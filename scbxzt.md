代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nunfpiah.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yaypgsff.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fpmxvojd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mqvlrrjz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dqwiviwj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hhbtoapy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vhdeilab.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bekbnzev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vnxnuclv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyypxkms.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbrrajrg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zmschmrl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxkdrmf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nznxletz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jhxklvtx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rtmyfkyj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iwtvpogr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dddzaijl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kbmxkevm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grxeshpe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfwoeykf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bgfjhouk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xgqfcyau.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jjvenmzj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rybduhqs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qgcxeodj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zpsajbxa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjlolca.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpzmuww.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vwvgqqdp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xnbvtrzi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wukzhpcl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kehviknh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rxxwlkda.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3knsixfci.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vjmxblgy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yxxtzoas.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sgmcygpf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zxudaikc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sxgegdfc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3amsbgnbr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3icaqgrgy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xkatobvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hqsmlzpn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3cqqmslwq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kdixdgwg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3knmiopmr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zstaljhr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dushyqwh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3usyeqyyl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zhzagcuj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gezayjsn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rjkmbbmu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3eovifxdx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mbxvnrem.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooqspulf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unwzmzpt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aaxmbokp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ttqvhkkm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eogvffqg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qxotpoiq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dqzsdyhu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cahkrchg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3luglnisb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fjsarzbq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pssegwvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3shstgkiu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bdqqctsg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bmmgzshd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aoutufoj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3luiahayl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvsjchlc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxfzpbya.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nydrryxm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3debqfyom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gcowdsmn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xljunefo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3puatebcd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qcjoxzsn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xsakrqjs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zemfdqvz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtntthlk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upuoavrt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qqfigvio.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ncvsltuj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqggyytj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tqzycfvx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3syqkiiga.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fcydggfi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bceqmwft.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gpjgrzho.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kafakedh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouktmykf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ttocculo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pjuolmrx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vbioqbdu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dzibhwnq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rblffxvb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hlbwxtvk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3innmsukw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uexjmdhm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eqkmftjo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3micvmzsa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3uyvtbycm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fcbpdyyn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sfbirlnh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdwtocwa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vciylilb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yayeiprl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xpjbtwpi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wtpudpey.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ivsqgwop.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dfsahbcn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijewpjlj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vtdubdev.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3groucjcv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hyuayctb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddmdbtlh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hyubxsgb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gfhiswzn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3trgpcsrk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zxuqqywx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3splklvaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjzmjtbm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yogizvvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pogiqweh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rmsqqsit.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3imptpqtv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zitfiysy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ywdqqpsq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3creyulab.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ppfdisfo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wwlojoql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubyiivkl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kerkejiy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zzgjiqyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ddcqlcnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnibuetg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzflbvks.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrijdjqz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kavdabmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3shgpwdkq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3utjahlrp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ziinnssg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3stqnmhok.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kgwgegjq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cwlttmrr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3clyzzjve.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xrvvcpjc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gvjlbgnc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxoxyat.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lzatjldz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kqcbrpmc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3gtxivztp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tvgiwyty.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrqnlyrl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzvsnofx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoxevpix.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ooxcxcqm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vuirhyko.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zinvmoez.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qyuvdldy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpgqzjcl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rdnlvthy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vamnkefe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eolinrde.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulupxcwn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rgzcwvah.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3etrfanie.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ucbvsizl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hvkzrhby.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3acawmrvk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xipuqiqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uzhcqbta.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lcpluoer.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jpcyovhg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lzghcnbs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lcdbjgaa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqsxbte.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fyvwhtbq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gioagzkc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3qpttqarl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uzuokhdq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyxnoyfw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3drybyavj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ciwosuid.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lehhrgmv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ftoafovq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rxchpkyl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ayqouufa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ggbkxbid.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3mgtmcmig.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ciscgidb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ltgjeohe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ejrgkrkm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3skrlwllz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3iagpsaha.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nmpfkicy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3chhywwmt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3eujemdco.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rktrhzrn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rfuigwyt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kyochzzn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jknvkuky.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wcopuhbp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3abjfwjdv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3polyjnjt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3oyzeckrt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ydftqqxt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3puouefzu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qmcmvqzh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rtdrnvae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mrrpihuq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vivqbkcb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kdcufvhk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmphcfut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skngpkro.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gbsvjlmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akyhspbd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wslyfczj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqicwhi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qcttevoq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnurfxvl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xfhtjuqb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3hwmwwapg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvazoai.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lxxfzlhx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ssxknxcg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qwatqgub.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xaciamuu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3anidjbne.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3nqswnwiu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hifguzyu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qpbulnqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnbvnnc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsvypat.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ictuzsrq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vxzxgyfd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvlzsjio.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3iredqoyw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3aiaderdk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3owdwvzia.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ihhuzjhr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tnjkmixv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fubfhgos.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3uqptiquc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nouzoqsq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aeavuast.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lkmojovg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nypwpjza.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xljnyzho.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ogiwxmyh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ffreogux.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ctrjlyrt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3biqhhvkh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bnxfvnsb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmlztrp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ctbezvdx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vawxjdhc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tjtzthjv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3cwxpltby.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rvmtypax.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3adyfnpcf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3dgdmpdia.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pxdjueoe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cuyhgzkn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3vkfpopyu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ztdzaxin.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3okfnqgcy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gkyuvvvw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3pkyuuhas.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3dcdbwpvi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rkjhkrin.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3nadfrnwq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3unfzvlft.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3unyetylq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3zipvweyq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3smvicrry.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gekuimma.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvdupgs.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3znhzfxag.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qkhudpet.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jdkjipzh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3jpzvoyos.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwudswa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gdknwlmt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yspttpbo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3upmmgekl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3qpulazpa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kfbwdzse.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tpvfkhgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwjfesvy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fopaywrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtuejgdi.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3crcfeoyu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgodwmg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwdqvz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mioofwvj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nxqqlcma.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3sxeimvaa.html


<!-- 参考信息 -->