代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nnksfnmq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xtxjwnzy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrgtjdwf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ychvzmbs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tqnsksnj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2upityoot.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yzjjyjxv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2boysoxpb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmxstunl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2riootnvw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvfdngo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cgbymvgr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gfcrkckb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2unfyowsq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hrrbrfcp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2edeagunv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zjpdmirn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbyyaqom.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2spkkglkd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qubkqhfg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xogbtlkz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2svocbmlb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nwngzghj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uifctlmj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2djyrimfr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zfhpvqdb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uktqhcmg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wdvwhybj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zctidopj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qwsznnin.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2raoxyudl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqmvkynf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2onqmrguh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vlfglcsm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kybrbrrr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jgrvlazp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xjlqcvhl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vpzyfzsk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2crusgryr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qwlzqspz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ccsipbgt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2etvtnddk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2aswrggvn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gamssakj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2auhvxjab.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2shqdaymi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgrlqqov.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzcgcnuo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2htsocdcy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2eqrnxsln.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dubzkphc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fcgwavre.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pdqrypvr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdihlxc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vusvzwvz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2usqkmnlc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtvltxdv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ysirekdd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bgkynqyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzitywon.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lzyjkjmq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uzrdponk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2deqwhedf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xhfyqkky.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wzqahhld.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2spwvjyiu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uuidxxfq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2adbzfrgv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2duqeufap.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xgkdmags.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zetgdtsy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xmggtocu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qywonsev.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhuehxj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2heusllgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oknwtcqj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mwsgcbuh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqpntgxl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2srbesxqc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rqbedewd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lukortfx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxqxqths.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zamnvdfm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2capvqcrv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ueubatgk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvngjltc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2anuxapln.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxlwsqnr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bcyjkbew.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fpxwisen.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2arnqbtoi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hgywjatp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pfgdxyoy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2axoiuhtx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzjsnth.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ppgdzwuk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2osezluui.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fcbpsqlp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fypshhox.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yhbkkyfg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bbxmayzw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecywdtiz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ujisqjyl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lqabrlpq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gsjijshp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fixhcryc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2igirbmfj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ilnackwf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nlqmntqa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwunkxzy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ipcxtezr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yywapgol.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2aaafhyhr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2elpoefon.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lwubawiw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2inlilvai.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sxilylcw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2efmgkwlg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xojzgvfg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pyjetrfz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gbkuixpx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tgmocexf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lfdkhyve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjazaqmb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nbqwfrnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqbtsxqp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2llmwmvns.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cbavgvfk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2seeyfpje.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqcoueji.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2otezokbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvtgyni.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2skjbukcx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2slwdxunr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxqkwxsd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jgswnwzn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kpblxhxv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bouaakmd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bizvqxxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tyadrmuv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2codyxvqn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bhmxfdkv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gdojvucb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxpcnvd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qkzrkvwk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2burwqswc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hjrqdede.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ifhjubtn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vxducnpk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gxajzqha.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zxvxmdet.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ytnumtrv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kncizeou.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bhhucpgv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bnozhslg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fawbekuy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gskckjft.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeormzwh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fdivvtma.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2yurwmymb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2temkqqwc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mamjxcbn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jpnznxfh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2aqfozosa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pvaksnmk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rexltzgr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onnfyksd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgctokuw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vpalsebg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yvxrgvcr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gozhamnv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ixwllqgz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2roaodvte.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ungrsxau.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ueulryhv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yvlevdbf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2osynnwqp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdvghir.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkyifwac.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2twwslnhm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xtoetcts.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ztoiztvn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2umtitpwk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yuqekeho.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2naannoix.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2pqwkeqin.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kxqbdqle.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hvtasgzf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2goowvznb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mylgnvpj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lfzzwqgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ssikijbn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hsbkhuhc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nqljpdvq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jjitamsy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gazrdqqf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zlevjtcp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dvotbgkx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jjrdbthw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2inzkgrsz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wziwxwaa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2twsgsmpz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yjhyrmbb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bzyllpvr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mnqzpfem.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jiczxdtm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2iacmhecv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fzziclti.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gkycifkj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yadzlxrr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vipjsvsw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lgdrngre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cmgqbxfw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wmboyxst.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ombtrsez.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssoehteg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlfvbgax.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2frpudyiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qltgfgad.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvidgglt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tjlifajx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fnsbpeai.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hxpdbnrx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpebopvu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wdhcswei.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2tuxkkkob.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2juiczshu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pexxvqtl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cxhssyby.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzovsgim.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vhgqbcdz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wdowwxxc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jyfpokhe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iipapuux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bdlgzwaf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hwuhcjqj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czogsipt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wvomreuc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2agviawge.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hwusafrw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2agwiaewc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nupfvpmv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nzthbjop.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bwpkbgpi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gbugdlmw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ljnaqffx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2poxtqjtr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnqvpxj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ncamqxwk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tubumflu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2olwqmgcb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvptjcta.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hdobdwhf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rmcsoqca.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fmyyfzqk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ruxhianf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvpkaamy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2msjawztg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yzfvptda.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oixcynle.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mjpsftof.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xlaxopof.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfuqcyz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2neijorve.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hugfxlqn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2flmqcnxk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2dfuxhqml.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yrysztav.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2exawkvbe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fqwvxxro.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2mjycptho.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2dacwxmbr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hxmghkur.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2hsjelwad.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2hzbqouat.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bhhnczjw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ztwzjwre.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zlvtbvrj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2oeqeqlps.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qezensui.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2sbrdqmlb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhhsics.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uuvvxwzx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2gobyuhnm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hwlqqipt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2favvolow.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fyknaohk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2szlufebm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2esueogzy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzadjtmb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gtxswure.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iadctpkn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pghckseo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoflfcxd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jtlwktku.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2frvjeyjs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2orqzzxey.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkezzf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bnselwyh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oiljqyud.html


<!-- 参考信息 -->