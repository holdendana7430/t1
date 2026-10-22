代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsrflusz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mlpgvins.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iatvogtz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aydrbgbc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2axmpwqhp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2leunppjv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mnlquhqb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2olllgnsx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ydcmbuai.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2aglznupo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ojidfkjn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wgifvgvf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ohtjdzvc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2immnzklb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aprgdthp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihylmauy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2llnxdzgc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ddeinefa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cvaakqxv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xgzmbavj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dpdffyob.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kaodwwyj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ttakpjhd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztaxxhte.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oabogbpb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nmsvonhh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uojruhzq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bssabnbd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nlrldfur.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2miysibfh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pnwttlbq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycaqnlku.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlpcpqfh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbggzquv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2amixrshg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ktqwikfw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2johkqomy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cgegxvxs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2efgojhlc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2irkywjqu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ugmujdik.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oylccjci.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cogiuctl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2flaohnfb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nbljbagi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cumlpgrr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2czllcufl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gbvycfaw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dtvuscyn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fqhksgdx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ijimpkpk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2utfxzaxk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yhjlmffk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zyfpzitc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzcjbbdq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pabkfece.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cmalmuoo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxmprabc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qtpktmzg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2utvbnhrm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gizfrlqd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sinpjjfx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mdmlziev.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eelmphjk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zasedzst.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wdaedhet.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjgtvrev.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wbxcxsyn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kxsjaqlm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hheticej.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2egasshbb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jhwxcfra.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2beezstqd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uisczzwb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vwbwebyq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfaihuzn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xkjzhdwa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzlvuqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbmcrbdh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aaknjxva.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bctujfbj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2crphjeka.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kumptqjv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yuxdrjum.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uukqnged.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkjbcpsx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfnzyuj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzyinkbz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2swurmwsa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2chcejomg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhldhqeb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2poosdfwc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2adkmhtcq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yrdbstuf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhfxenqy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dynmfzsv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zestkagk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zpltsjwg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bvbdhtxk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2joyccytk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bnimrdzr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rljndlgn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2euxgchix.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rmzilzwg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lmnuqmbv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxasxtii.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zkivftfk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jyjmwqng.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tkqfedzs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2szoijgyq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nowgzlyb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugcqoem.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mabvkbny.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjzgtpe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qhpogxql.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ltrmakgi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qqxynipa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2guyraylk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qwuqamlm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gjscefkb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gyklqxyg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhxjnyyp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gpltbpve.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2byhdwwtf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2eztuzatw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wndijyrd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pzzssuea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpokfaxu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mlohgpuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyzbnckh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2habpbprx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2edsomirx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snsshfmc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bftzyink.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yiebadju.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zytphyjm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ajrdyzzr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vlspmuvz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hezsepmk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ahwfeqlo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uzuioxfw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fplgzwum.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lorvkwzd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tpluttaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kbobqfzn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2uxobaajk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2owbruhqr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkdkzjlm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2judmridu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yogrxrcx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ossefusa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqqeyh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2brnagwim.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mzjiopaq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2adpywqzo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2blvahtcv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aofjyuha.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohrbrcis.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fdaumipv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkunnavk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcxoauhb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cikahqek.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2czfibvgu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fltkistl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tgvyyqrj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nexwjsqz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2edgomgdk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vpunzmcs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jjooeltd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucywwuju.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oynkdywf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2renamsty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2inukwvjx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ffuskbgd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ikhdegef.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mvgrnwvz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dnhgnbgz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvprbcf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2shfbgpdw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bqtrqygr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mbazgnzm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zbocgkis.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2scmmcbbp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pmurmivv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qfvifuya.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zuoazxbs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ripgfxyf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjldtudf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wksqrqdh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ykaihmtq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yqpjlyni.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wtrflsbb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmpndpy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2izqilabf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ysspthpj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qeirmyji.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tnshjipl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2edvsuaxn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wiwtewxk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mifvvsqh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vpwvssra.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ocbdbbgq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2yeiafliz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2kvynfppi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vtstrjca.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfzwmr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbahbafs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cmyxpkqx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2jjddabnr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2cctmqrrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lfkyyjfa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ieuudipe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2juajrlup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wljmmmpn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qvkeiegy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hgceovns.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ukzhnjoh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2blrlynii.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2szovnpjx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpkqxomu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btrxbyug.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vjanuqte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrbpxjci.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fphgrgzq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zpukhuiq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddpxxtll.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqpwxei.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gfvdnxap.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kryautyn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ihnssvcc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zuedbgrn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dzmzbcgw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qsaoboic.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2szuebgiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lculzgsm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ambkgahl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbcteid.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zkgygipk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ulkgugsb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2incjgmik.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aedqgapw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kfilqyla.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wxggdorw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2quftynfb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wcfgtere.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2fplukbpk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fyedphsj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2svphwurl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jemyaiyv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cpgvlbyq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fonoqhru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tzpocwhc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kbnxhbzn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ksshutgx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ocvezjcq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2whglukbl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vvaebqfl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uyascduf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2odyvqyal.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yxomwqiw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbpmicza.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2opgdsufs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmqzsml.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qjwkfgdo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xmhewtoc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecylzhdx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzxfxyn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2cuyiaxnc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zbrmfdvy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kidaifob.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zezachxo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fgpfoolp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2talrxoqc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tawtjrwl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ykpxjimq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jhdwioln.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ocvwybiv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fugswkzn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2fwamomlt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ygcbguss.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vscsgitb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bnfskgda.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ubitbpml.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2geizjwqx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2hnljgtby.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ohijotia.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rqnlibli.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2etxrqqhe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dapisuek.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqrbew.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tfagmomi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pyputheg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2cyutoxpm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hyyzrndi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2trghauey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxaxjowz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2oenkhrhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xodevgzv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2talbssgj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qfpimeej.html


<!-- 参考信息 -->