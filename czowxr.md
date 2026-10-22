代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2brbmrjqw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pihetvxc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mpfjxxgu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2corzidao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgwapkim.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aebwfgpf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jtyedcbp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dobotaap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bjsmbxxi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ktrhugqb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmzngv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pbzbkgap.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nmkqihyf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sjlgpeub.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nvfsazkj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoslebnf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jtkgalqv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zhxmkuri.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dkgecdlc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rmnqpxfw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nszrkdjo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vbahahae.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvnceoab.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdvlsmin.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqpkgpgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zezhjlal.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jlrcugba.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdblyoqy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qmgqbpab.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2uzwvcefq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gsyufxej.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gxxavjub.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cvwgadbg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zvmhtzee.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2utbxuipz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tjblzulw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wijoxlzw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jeccwntw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wxowkqxn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ahmftmco.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyvhlztz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmriprfb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2eryhjquv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2raxfnsys.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2elvcuykz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qvewhhry.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xlruoafn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wstyirwk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zrcvuhxr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2khkctusp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qwzvcinv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrrbcjea.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hpubmwdr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2awonpdjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjfgjydf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vuhedrfu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2josyhbbq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hrsizrgo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iuhuscvc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kqytxlva.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wqaczijp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qnlukqcj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cwxqyuup.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qxuvcbca.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2chqitzho.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vcbdbiaw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hxunpwbg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dohuxkcv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxrrmcci.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nurinplq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxhbhwcr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qwexaier.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vpommrwt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rszeumuc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bxyxdryd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nhvmwjan.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vfmkljbn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2baoiveee.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ecnyhxah.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wmypzgfq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fddnerhw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pvasdpbv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wznvxyrm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2brjqistb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjrvhfh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fdyuqhdq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jfmlijmx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dzupefmv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qkivvovt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wifhmaax.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vwdwhobm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2croularm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2avnotgjo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jdwxtvbn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vtfsiicb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kacbhwqp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2heprwrnq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nfjzshyd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2svempbpb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wtovczws.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2koqozmgc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2eqcsxsez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jewqyuso.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2entemnqd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qgvwsllt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ndsjcgsh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qknzzcjg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxihtdo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bgztlfen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2awhypwdd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tmfhycyd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xppkwymx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wzixsavz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dagppbpi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffwbsdmw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xfbsuwaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2klrxsiwg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wobmmrdz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dfhzqivp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iejpvbuh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hnjgygqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycrwscgs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vusfxrfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lqgwctzp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sahcoazc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxuhzmsg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ehhywglk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lasffpdh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qdklpckr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtwsniyr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxacvlie.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qgsgzojh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2azmlhnvg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qobvchwq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ruafaqhf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zflbcfvl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ckgeqnpo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2glodhzqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2clipuoao.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iutchvqa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fnxikrrq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mcpftsgg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kqeokedc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xihpxlnm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tusttsfb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ujgfdyun.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ygkrjnfd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gmtbjmtb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aqnsdbpm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fqcpvtce.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rxqiqeso.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2alhnniol.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeajgesw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pajflqay.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ithkmekm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2etsmyzqi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgwopelo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkmrtdqq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjiwwllo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zsnpdbks.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xwmsezqi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdbarplu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzhyrhea.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ktwkpogz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ualhdwvl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xevomloi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kfircdqc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ymadmmgc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2iqtqadom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kfgyituc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2czqetuey.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hglpynob.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dichryoh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2etpuhkbj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nuxeuinr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wmdnvksm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rjwidxgf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ouzjxtqq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xdvizxzv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ihzsdotg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2exeottct.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2weranvwv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vagdmzph.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kxohotds.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xygvqwlv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fujnriez.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jhptvnbv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wevbsjlz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2itdqqabs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2eaqezvti.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wdgeqgdi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ipbkeivo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lqtgiltg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ehgyyfnh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ynmqpkhx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wxefzrvu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ygngdrno.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wvyiwrrt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2sfeagnwq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkhziknz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ytsqynzw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2lefapakh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eljggjtq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zuyzyeno.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lplvyekn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2tcqjjmlb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zzpgfgzz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lophiftk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2yhsxfhnk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2akhpvokn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2supbkfph.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iyowngwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhbuzezb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hvhrzfgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehfxrlco.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nbuhxbhx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zbdbmgtk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2unrlelnj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qejxwyyk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwynhvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrzlxr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yqozqvur.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cdnjicky.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dtakquly.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ctcurxrb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jknglbuf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2gveexgvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2onhovqbt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ypuuvdqh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vxqnxscd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsumejsk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lacsjbmq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nlamdqyn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zkpbdrhk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwohuj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2llyincqw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lbzcjqoj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cnytdwkz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pewraglh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2pfqmbgxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2djytwady.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2smahqsju.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nrhvodlb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gxivjtyk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wmxghyzk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qfvfvqsa.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xjpxbehh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dkmhgwfa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rwlzlshl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2jlkbyxaj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ezubxrle.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2eblrnkxx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2bypqcuwx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qcmqosdc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zetzjvww.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nadgbtej.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2imigmwny.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmbwowr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhifjtn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zgpjimkc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2shgwbzxn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tacetsan.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ptydejir.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eudknxmz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2btgrvadl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2aomnvhuf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2opjylswg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2okfowtdk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2seigupuv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ieeghkqt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ujjzntxm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fzmvpwro.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2coijdcyp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kkqzhqvd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwcbjaz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2erxilnbm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxflezr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqwjnmk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ycjdretp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bewibozd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2catcrmei.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ggbxeoag.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvlbdwy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2juoedjih.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zidhtwel.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qishehjl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2suxcncsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlphvbqs.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bopsijgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngsslbsl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2czbscvyf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2kyirffuv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hyjgkewo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dfpkyoyh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mnkcdsbm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jhitwynb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2wtflvkur.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fkwulsdv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2yiyvdoxs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vmnvrmth.html


<!-- 参考信息 -->