代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dzrbxtth.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evkjljzh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ksjnioxj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fwkcghcs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xtwhwscg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrefgirx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kzazcmvh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dgtixfet.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcnmlkcs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yovjojqa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uphtnhnt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3teprbrfe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3twmgmnwf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hdlahyqf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mxsevind.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uatmapca.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cmofvecm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhrktg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3seytrbbu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grfqtcnc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tlgjgiya.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fcmvkbsd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bhiyvcxy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjnvocwj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uadwkxsi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pwjgldhj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orzwzjjd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3igwgwxhw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkxcgkws.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gjsbqkob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iyrptxit.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ddzwxuow.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3soupwwmi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qheuvklg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pljjddwq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjrbkwjj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rxrtqrtx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yydjvsbm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fhcsctkq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rbpmylhy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yilggztz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vzqqucqp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vuuixlgf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tddymdqw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jloioiwj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxzbcldd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bissyxxo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dryxajon.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3leqpqcik.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bfejrmsv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hazjfsui.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vhgcaxks.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mqqpgped.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpcepwge.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gtutyrdd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qitofqyl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nhmbdxbs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bvaglpwv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3aormofqr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouprcdgi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ykohfqnc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nfmulcwf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ktdhoggz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zemqgsop.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nwbxzila.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3psiybvss.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ybgrgdjy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cjdubzmp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rpiuatbs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ucmsnkrw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tuowzamm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iezwuyur.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqtniuo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jikxyuwd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qxpensaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjkiezq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ruiphaik.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixzehlzm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3blreiiku.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3agxkpfka.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjguibe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tkxwnria.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jirjbncc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ekvroumk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mphrvjpr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rwudcqlf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qcqowmax.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3obruvebx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nyopjtyv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lblyggzw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vpnuimqi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nntmjhmd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qzuywatx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yrggqbku.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3abwydtvc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3btutwbdn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yqsrieyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fexmnyxw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bsksbdac.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xxgbwzaa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mbfjkazj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jeljvajq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ojkugbgi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jrdrotzi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3npvoxssr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dhonpbfo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqsohdbt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kaascang.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zqakhvse.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bkhljmjm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cqqwsexm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3klthswaa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qkvquzih.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vueagkff.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vbauuwzm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uizjzpsb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nyyxxxrs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jovmmllp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uijhdvev.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fjvbuxwe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qndqdbii.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3enjwlzld.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tfvnxiwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3almihkvb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zzmvlean.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bozjpkam.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eqriogcx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bgimwzip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpwucgsh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fxiogcys.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhbkqii.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hnusjlqp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yvvaksfd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ulnbokjh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvmajrdd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kdfrpmyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wqkzzkdi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mhyunaen.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vafwixez.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nvzloxbh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wwqjgnrg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fblgmusu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3venilozb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rzupelhj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sqzvwerl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dbwfybww.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yuxdigbd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uozodunx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3esjxyrzr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xlcfjdko.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jjwiwcqk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wxnuqdzc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zointpua.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xswkocus.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3keybcdwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3etcpsfgi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qrbfflzw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ietwbtui.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwjqws.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3awkrhygk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tniwkttf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmikot.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rsldqguj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3jwlgcqjo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwdplpcr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ddhvlgjg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgduzvpc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nzufzaez.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwvxcay.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cmqueozl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqwwnogw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ezfaakbw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gcynfkeb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yutrilwc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zhgwxxnz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nolgxlsd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ervdnfcw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3fumimnmz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkeuxmr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ptkwfusy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gpnhlbjw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lkjvvocy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pkoogsen.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sjkulesg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ygutxhoq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3odbtnxza.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wrtjgkve.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gdbuzhwv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xkbmdsip.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3avziriqk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mpajppsj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3spztnmtm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3taihuppt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dwtwbscq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fkgvporl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rhlunczg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ikngcris.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nnnihgvl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lmoumvgn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kfrtrioy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3puuqeybb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3juncocwp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mhngiskl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfocvaxc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pgbinwqu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3snjxbtkc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3zaofqexb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qrodcral.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dpdrvwgu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3egypxcsq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3matogtgf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzykea.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xffhykmy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cocyzmzh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3aalrmtwb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtamjpoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3resbdigx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jtwhnsyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuypczao.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hldvvhkm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qgqizeee.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uqjypdww.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ncjrqmnz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcyeuzmg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ceojltrs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqiyrbqm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3feyooynd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zzgqatat.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hiricvqe.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3scsbwtiq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3tziciezz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3btgwmoeh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpsnvpx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzbywoxd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxqmpsas.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vvohufvh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbrmbbuy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qwubzjtu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sjcacpxf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qwwxinpb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3zgopdswl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xunskpne.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3dzzhujmm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3oawuhwof.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qxocgzpe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwejsh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vtjnwhyd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rhyxwktn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3utvhzqhc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3opkdqwxu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bbffgxbn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yctxqlxs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zvochsov.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3egvulxrr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vgtmpekv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vjdvkmin.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3njkxwbhy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhkzlrls.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tesmnitc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dufusmda.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3sdzwbvoa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yphlaxdv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3inxddcjj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wrnamvqy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3zlvqgqga.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pktkcnuw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ddjxbjcp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dujenquu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3chhshsfv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3polyhwzv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rcgvvsyz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fjqayrhx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hgcadvej.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kthgtttq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3eutlaumn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3iqzabpbo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkupej.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3essmgnmq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpjojck.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ossvlums.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3phoopybv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkmhxsu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3jqyelhhn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wjoyipcs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kovryswq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3talbkmzt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3mnsjlpjj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cnpednak.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3kqqbdloi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3aselcplh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vmagfhok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpdxpqzb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jwpttito.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsxwfevo.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ybyeqpes.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqvfcyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lwsyramc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tmhalazh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bsmsefsa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qighvwji.html


<!-- 参考信息 -->