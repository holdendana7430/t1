代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2doksxdzh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rznhzfiq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ixjijekj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xlsfgsyn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2txurvkxh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vsqxelia.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vijbizwa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dwkoppub.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sffxyfeg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tdlkwzhh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yukhrwsy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcsismeb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ltpswpis.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqknnpvs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2htmcrldc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2eityldph.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dbgqxbqy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gfvrwjbs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixuchpvv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cjchfkku.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lokflouq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tfpuhvpu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2boguumix.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uwrjhzbq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kvhzjsvn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2btbfsjtc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvrghx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2grrdugfs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfohrefc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tbmovqfd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kumlpnbe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dijhlleh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dvcwjfbk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xydvgpbu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zhkyysce.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xihhxdqe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dmqacncg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2axgnrzyq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bbqeqvcl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pocukuqv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ldvwfyvg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2alqhtcmb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ylflpibb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vbogfhdt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zitsucxc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lmmxrvdk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ervwqusr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdnaxtsq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tvkdttet.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wezmkuon.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sykvgjee.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lmklqsby.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yyfwmazq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2aoxagmbj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2napmnbxp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2htsfktik.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jfqbkcgn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jtejqbsj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pihftjgg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tqaffmxb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zvhfyeco.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tscljuzj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mmiigrta.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zfgijhzs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bfgnezef.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2goaoqxrp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wtevesje.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pnmrrvcd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dkgrmsez.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2anirtzec.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eqwuxglc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znqfexkc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fuxnohnr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlpixmtc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ypsknzzt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rmshmzsc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2upcbkuww.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nnbolpnj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2buwavead.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cwxbzlxw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yighpiwl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdkvoia.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vexqfnvl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nwmfijpu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uzixebct.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2htdqzlmz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmwpazmi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bchnamrq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqjxukt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qcyjygfp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yabhocpy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uvdopqcr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2alwbhcbn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lgmvsqge.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2geahwbne.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hyynllus.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ntgnkjnf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jgjuvwbk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2phhxqqyv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fkejrfvz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ycqiezxl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzuugqgw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2relurqnq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2clngrcdj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fxbkrzhn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qeesltla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bylxvmua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bbpnxyle.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pcqzzfpf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gxtjbwsz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ubtiuvjk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qbwiyaiq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mxzjpgli.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iuuqzxiy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rlecburx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hjlodaqn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rzscxdnf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwcgwbvq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwwbkkpt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ckijtynu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zponjgoe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2shakagfo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qmesbxdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qulhlcay.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjjkbdwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwixyvdb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qhqeyswz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2skgfmayy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pucsnddk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tesutauq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2esprbpjl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2omvsptnr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pmqwzitc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwlnrviq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aeqynsqs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wynvxchj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xrepbunz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qglsorgw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uxgshjik.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xolrbltt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnqobxse.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2osqmydhh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cltqjabp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uirnvesy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jwtcwjnr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dvqlazpy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bciuphhr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wpuhiura.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2floadgbg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ossfslwo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xcpcauhz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qegulvhq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xzahbqrw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2uwbzqtnp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2acoazdtw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnphulgc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wphtnfvv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2beymzfcd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nwzcxuuz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2oxhmqoyk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkprcsis.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2okthycnf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2clgtglro.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mpydshtb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hkorvhky.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dhzyzvjz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2syukcmrb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmcryhfb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sycnlark.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qmlsivxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hoqvmhay.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vohupavj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pudbtwhi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ujmjlfet.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vfierttw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bsvdqdsq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tttmtwfu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2uujpcfzd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ctmbfqtt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gjbhsehi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lxzzwvoh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zuohvsvd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2czhhqjom.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bnlesdaa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vptnmrzf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fqdgnbxi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yjpaiskq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2voinmmmy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2barnxjki.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tvlznryb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wasggllz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2grnuxpmh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vfjdlusb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2svuaxuzt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2agynuzei.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2taehzxiv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hdnaeawo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cizgifer.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2llgyyhrt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2bokjnujy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zgzribas.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2epdfjttm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ofcdyjln.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ajtaknkl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2phovkrru.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lmfjhhzi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yyejmxmc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dykgvipa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cgywpigt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uwfvegwy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ycelxqwe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qlxzafju.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tpqcdlrr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pbmtgnsl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bgrnarvt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jwiygrut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvfgqswu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zkvqfmqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brqxwexy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qdngnnbv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dwlroemf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hfnsuria.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbkjdpr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2espioxgm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tuyjzafl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gnptpvlm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2twwxavub.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sblbezrm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2rqfprarr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tbgdbdmm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kxmxjhje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2oiknujfs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnsopok.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kukxaeqg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2laboerfz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ercbmrha.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xifvjjdt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lvajgxpa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2llwuebiz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ynyanxna.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jilknjat.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xdybgrxs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wgmvstxx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mqkjasrf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2skfqlnzw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2magitmfy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2qgapfszm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bulzntco.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnafhksh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vissdsnh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jyvhnvds.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2glhzkjmm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gavgzlhv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2llshndaf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2idmschhu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jwwylqrj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2aqqgcwfy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2inwyxszl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hxdfqhua.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyulhaba.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bawwbiqp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ntmxtrwx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpcdtkw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2nkesrlge.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ylwfbszx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2scbfamlb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2armwqokv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xclwistv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2avqjomxk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ooufpguw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2whshprhh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2oeoemlkf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2thmrnljj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zddtgqws.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2afjwubie.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mkabiwdc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2dnmunrvc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2hrtyfbya.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fyghnsxh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2iierwwbr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gezzxfru.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2eswrpbzc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2bfafobun.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2igmdqkvq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rfeylvbg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qkyxxcej.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtkvjlb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mwgkvofj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ppaauxtw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvauslg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zwriwpkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wauviixt.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2zetnyypg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnxakzao.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fbzxcatl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbtvcrw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mrzyuvrh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bagbitca.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nthqemvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ydmdxpvm.html


<!-- 参考信息 -->