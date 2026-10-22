代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lexusrqo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xgzpyuny.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2otjptdwd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nqdypfav.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nltagvje.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkawzsci.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mcjoumsh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bhiagjrl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yfaqaukh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cqqategb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vjrxfgdu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wigehgft.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sauohazw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqqxdlan.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvdtxrom.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qptkswdm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuurxcsx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2blhktjne.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucxegmxv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2awhbstxq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fqwbjnjs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fmxclhjg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fccnyjnx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaggyxhi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2podhlyxq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmjjlhli.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zuajfcgw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiahmfwd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yxnfpsbp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lgpygzfk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pymyxaam.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xouhbjzd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jspgdmct.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cboqawog.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wyghsnul.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pxzmxxls.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oqgojafd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cvsmvfio.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yrsqoiwd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wuhmmamf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxjltqtg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvzbsjcj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hpqqmeli.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zapuenlk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mstcdaqf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2izaysygf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2sweiiwmw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mgobxxfh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2siynltem.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qzthpddu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ghbbgvty.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ouxixlzs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chiyqadb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2opafeprt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdwkvsya.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jijricff.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ebyvtphb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yjowbzef.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qinkcahw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cpcywsvs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mybhypca.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ztztoeow.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2khwojqoi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lyayqigg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2aqexfocc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dotrlcza.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lsydgxvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ooaguemn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lzjmnhsr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwsgdnvv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2knmdujdm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmbenwf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kkcmsoji.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bublefot.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pxvzzicx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bxtcqtuh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxottchd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcgxzmn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqlgnxb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqqobhmq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hegjnrvi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2feosfyqv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zsukmpsp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bncthyrw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ecogcsdl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aqiwjqjr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2afgbfjol.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tgqhizsu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kcprbxrp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mhsiazqb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kwbswraj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mdmbfjpm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ndesftgk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lpnhhdxb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2elmcxbst.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2baltbyaj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uaawoamr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2luymxpfa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqqxyin.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nbuunidm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ojbtktce.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gqfeqpcs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cnlhpxwo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2beygtfgz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wvoynscw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwqkqvh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yahjoote.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nnxwwfoc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vjapccev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bpieioaa.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ubsnbkkf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pufxeenc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pdfobsgd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lupbdxvd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qgyschvb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2aoklgxkv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dzqimafn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nmiaaxoj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bkgercvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmgrlgjq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tomwwdbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxmvxfkk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zxmqahhx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxrivlk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsvqcoo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyetsqgh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ozwoyvbx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zdfaovcv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mmachwfs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mldeoswe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jbfejeyb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hppaycvn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2txmvjkfv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zgtxbfen.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wtqedrqm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyjpyasz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uksdajvk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lntgofmk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wgdvvcuy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jeykmrfz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aahiytje.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mcnwfbqf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lipyfcol.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fuuvibkc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vsvwhaci.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gzxiquxh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2olyyqygl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nzcbikvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ypuumsbl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ihyzcygu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yxrlijyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kynuapyn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uugjvcia.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gexevlgi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bcgqntbu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rdflcxgn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vfgxgxhb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtsekbrw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fhnnteow.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xlnrjdbl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2niparcmf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lppjgrqw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hdmipwfu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzptkhxq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2stfrqxrh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ezmnmlcm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tpirwdqn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2emmudlma.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zsyybohi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fdlcrghh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rkmucdio.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2sehkjphh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hqobuftr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2eimdjmhk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdeitju.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jhzagnik.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2emdmqohl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tyxshgko.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ywomyiip.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eniffdkp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kfnpmnto.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wytwsvuj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2talujvrh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vztxzvws.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvaqrwir.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pfxpnbxm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2puefjybi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rxunqhxc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nsfuvlho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vfzaubjy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gjlmlbuv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wfptbcml.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2pocwwksu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ockcjfez.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vzxcfdbh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cxzlkmyk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2otsgpxan.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pdqbkdnt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fglqetcs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vdfvjgin.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lfjsopei.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ckyedlpa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2nyamomgj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2efydfslz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lvbzjvtm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vozicdfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2maeuwzhe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jgpomyyb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mvdrygwq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2snejhbqi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mcpykwcm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jzhbauwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snfavrdh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ibklrrps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqyejnvm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2uuqvsdvg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cpqiwddt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mewlmteb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zqfhwdre.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ihcribrc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2pnldyvdy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ojdeugte.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wccimnqp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2redpvuns.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mgnzesmy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vselfxel.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2uyrdsbau.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2znakidbe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gdzcukld.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ocbdbhau.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrueuacw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuqsjgg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jvpjrntl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2phraygkg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gezwqmxz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jeeoxljc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kebkgazs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ymjwugow.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nceuuxod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fayiakvk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qlbjevyx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2elkdrtpl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2snfchbxb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wxmaghlq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xvpehzzs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rpkhetxp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ppmnoela.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mxehrtgd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wbnfzxqp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xzjyflkj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uiutijnn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ngopxtog.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qupuowyl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uefidkvz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xqztzgtb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lmayxzag.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lrpmofcv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbxgjom.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2imvkfxeu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqazase.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lzanvlly.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zlgznyeg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dodaolpe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hyxalbqz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2guleypbw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zqtxltdy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2luplflgf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zjinashv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qgudymzf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ymorbibf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zxlpgrcw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qymbaywl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2yefknwdv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hmyivdva.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2multmwdc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wssyywnt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2emjkkqex.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2unmxtade.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lrgteqsk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ttugoxxc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2szylofcf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dbbfnpwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ceihcsdz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pbnyquwj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2quthtxjr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2icjkhkoc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gvrjonjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oemqdibx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ahhrppem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqkonnxn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybngvzpx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ozcxhxgo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bercnqhf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aenolkcg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uajmruac.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2guaxpaxj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fhvdtewv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rscflsbr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mgvjmlur.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xamvtlcq.html


<!-- 参考信息 -->